---
title: 1py
date: 2023-02-01 08:43:08
tags: [python,django]
---

# Django

## 安装环境

```bash
https://bootstrap.pypa.io/get-pip.py
python get-pip.py
# https://xyuxf.com/archives/2114
@uncomment python3x._pth "import site"
@touch "import os,sys;sys.path.insert(0,os.path.dirname(sys.argv[0]));" > Lib\site-packages\fixed.pth
```

不需要的方案，`site`包含这个
```py
# https://blog.csdn.net/brian_keepwalking/article/details/106440489
echo "Lib\site-packages" > python311._pth
```

## 创建项目

本地创建

```bash
cd django-projects
python -m pip install -t site-packages -i http://pypi.douban.com/simple --trusted-host pypi.douban.com Django
cp site-packages/bin/django-admin.exe site-packages/django-admin.exe # 否则找不到 module
./site-packages/django-admin startproject HelloWorld
cd HelloWorld
```

也可以是FC创建

## 编码

`requirements.txt`
```bash
cryptography==39.0.0
pymysql==1.0.2
Django==4.1.5
djangorestframework==3.14.0
django-filter==22.1
django-crispy-forms==1.14.0
crispy_bootstrap5==0.7
```

```bash
python -m pip install -t vendor -i http://pypi.douban.com/simple --trusted-host pypi.douban.com -r requirements.txt
```

## 添加模块

`../s.yaml` （必须是 `.` 不能是 `vendor`）
```yaml
{
    pre-deploy:
        - run: pip3 install -r requirements.txt -t . -i http://pypi.douban.com/simple --trusted-host pypi.douban.com # 添加镜像
    triggers:
        methods:
            - GET
            - POST # 支持 POST
}
```

`.vscode/settings.json`
```json
{
    "python.analysis.extraPaths": ["./vendor"]
}
```

`.gitignore`
```
vendor
```

`manage.py` head
```py
sys.path.insert(0, 'vendor')
```

```bash
python manage.py migrate
python manage.py createsuperuser --email admin@example.com --username admin
python manage.py startapp web
python manage.py runserver
```

`python manage.py shell`
```bash
>>> from django.contrib.auth.models import User
>>> user = User.objects.create_user('dudongbi', 'dudongbi@qq.com', '?')
>>> user.save()
```

`HelloWorld/__init__.py`
```py
import pymysql
pymysql.install_as_MySQLdb()
```

`scf_bootstrap.bat`
```bash
python manage.py runserver 9000
```

`HelloWorld/settings.py` tail
```py
#
INSTALLED_APPS += ['web', 'rest_framework', 'crispy_forms', 'crispy_bootstrap5'] # 'django.contrib.admin', 
CRISPY_ALLOWED_TEMPLATE_PACKS = 'bootstrap5'
CRISPY_TEMPLATE_PACK = 'bootstrap5'
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'HOST': 'db4free.net',
        'PORT': 3306,
        'NAME': 'djangoname',
        'USER': 'djangouser',
        'PASSWORD': <DB_PASSWORD>
    }
}
```

`HelloWorld/urls.py`
```py
from django.urls import path, include
#from django.contrib import admin
from django.contrib.auth import views as auth_views

urlpatterns = [
    #path('page/admin/', admin.site.urls),
    # https://docs.djangoproject.com/zh-hans/4.1/topics/auth/default/#django.contrib.auth.views.LoginView
    path('accounts/login/', auth_views.LoginView.as_view(template_name='login.html'), name='login'),
    path('accounts/logout/', auth_views.LogoutView.as_view(), name='logout'),
    path('api/admin/', include('rest_framework.urls')),
]

from web.model import author, contact
from rest_framework import routers
router = routers.DefaultRouter()
#
urlpatterns += [ path('add/author/', author.controllers['add']) ]
urlpatterns += [ path('list/author/', author.controllers['list']) ]
router.register('author', author.ViewSet)
#
urlpatterns += [ path('add/contact/', contact.controllers['add']) ]
urlpatterns += [ path('list/contact/', contact.controllers['list']) ]
router.register('contact', contact.ViewSet)
#
urlpatterns += [ path('api/', include(router.urls)) ]
```

`web/model/_model.py`
```py
MakeChoices = lambda arr: list(map(lambda i:(i,i), arr))

def MakeMVC(model_module, model_name, model_columns):
    from django.db import models
    Model = type(model_name, (models.Model,), {
        '__module__': model_module,
        **{k:v[0] for k,v in model_columns.items()}
    })

    from django.forms import ModelForm
    class Form(ModelForm):
        class Meta:
            model = Model
            fields = '__all__'
            widgets = {k:v[1] for k,v in model_columns.items() if None!=v[1]}

    from rest_framework import serializers
    class Serializer(serializers.HyperlinkedModelSerializer):
        class Meta:
            model = Model
            fields = '__all__'

    from rest_framework import viewsets
    class ViewSet(viewsets.ModelViewSet):
        queryset = Model.objects.all()
        serializer_class = Serializer
        # permission_classes = [permissions.IsAuthenticated]

    from django.contrib.auth.decorators import login_required
    from django.shortcuts import render, HttpResponse
    # FOR ?action=1&action=2
    # request.GET.get('action') = '2'
    # request.GET.getlist('action') = ['1', '2']
    @login_required
    def controller_add(request):
        template = 'bootstrap5_add.html'
        if request.method == 'GET':
            form = Form()
            # action = request.GET.get('action', '')
            return render(request, template, {'form':form})
        elif request.method == 'POST':
            form = Form(request.POST)
            if form.is_valid():
                form.save()
                return HttpResponse('OK')
            else:
                return render(request, template, {'form':form})
        return HttpResponse('unknown method')
    @login_required
    def controller_list(request):
        template = 'bootstrap5_list.html'
        list_all = Model.objects.all().values()
        return render(request, template, {'list':list_all})

    print('创建模型', model_module, model_name)
    return Model, Form, {'add':controller_add,'list':controller_list}, ViewSet
```

`web/model/author.py`
```py
# Create your views here.
from django import forms
from django.db import models
from django.core import validators
from ._model import MakeChoices, MakeMVC

model_mod = __name__
model_name = 'author'
model_columns = {
    'input': (
        models.CharField(max_length=100),
        forms.EmailInput(),
    ),
    'password': (
        models.CharField(max_length=20),
        forms.PasswordInput(),
    ),
    'age': (
        models.IntegerField(validators=[validators.MaxValueValidator(99)]),
        forms.NumberInput(),
    ),
    'city': (
        models.CharField(max_length=3, default=None, choices=MakeChoices(['北京', '上海', '广州', '深圳'])),
        None
    ),
    'switch': (
        models.BooleanField(),
        forms.CheckboxInput(attrs={'lay-skin': 'switch'}),
    ),
    'radio': (
        models.CharField(max_length=3, default=None, choices=MakeChoices(['男', '女'])),
        forms.RadioSelect(),
    ),
    'status': (
        models.CharField(max_length=3, default=None, choices=MakeChoices(['写作', '阅读', '发呆'])),
        forms.CheckboxSelectMultiple(),
    ),
}
Model, Form, controllers, ViewSet = MakeMVC(model_mod, model_name, model_columns)
```

`web/model/contact.py`
```py
# Create your views here.
from django import forms
from django.db import models
from django.core import validators
from ._model import MakeChoices, MakeMVC

_phoneNumberRegex = validators.RegexValidator(regex = r"^\+?1?\d{8,15}$")
_units = [
    '北京', '天津', '河北',
    '山西', '内蒙古', '辽宁',
    '吉林', '黑龙江', '上海',
    '江苏', '浙江', '安徽',
    '福建', '江西', '山东',
    '河南', '湖北', '湖南',
    '广东', '广西', '海南',
    '重庆', '四川', '贵州',
    '云南', '西藏', '陕西',
    '甘肃', '青海', '宁夏',
    '新疆', '兵团'
]

model_mod = __name__
model_name = 'contact'
model_columns = {
    'name': (
        models.CharField(max_length=100),
        None,
    ),
    'email': (
        models.EmailField(),
        None,
    ),
    'landline': (
        models.CharField(max_length=20, validators=[_phoneNumberRegex]),
        None,
    ),
    'cellphone': (
        models.CharField(max_length=20, validators=[_phoneNumberRegex]),
        None,
    ),
    'unit': (
        models.CharField(max_length=3, default=None, choices=MakeChoices(_units)),
        None,
    ),
}
Model, Form, controllers, ViewSet = MakeMVC(model_mod, model_name, model_columns)
```

`web/templates/base.html`
```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
    <meta name="description" content="django"/>
    <meta name="author" content="du"/>
    <title>开始使用</title>
    {% block style %}{% endblock %}
</head>

<body>
    {% block content %}{% endblock %}
    {% block script %}{% endblock %}
</body>
</html>
```

`web/templates/login.html`
```html
{% extends "base.html" %}

{% block content %}

{% if form.errors %}
<p>Your username and password didn't match. Please try again.</p>
{% endif %}

{% if next %}
    {% if user.is_authenticated %}
    <p>Your account doesn't have access to this page. To proceed,
    please login with an account that has access.</p>
    {% else %}
    <p>Please login to see this page.</p>
    {% endif %}
{% endif %}

<form method="post" action="{% url 'login' %}">
{% csrf_token %}
<table>
<tr>
    <td>{{ form.username.label_tag }}</td>
    <td>{{ form.username }}</td>
</tr>
<tr>
    <td>{{ form.password.label_tag }}</td>
    <td>{{ form.password }}</td>
</tr>
</table>

<input type="submit" value="login">
<input type="hidden" name="next" value="{{ next }}">
</form>

{# Assumes you set up the password_reset view in your URLconf #}
<p><a href="{# url 'password_reset' #}">Lost password?</a></p>

{% endblock %}
```

`web/templates/bootstrap5_add.html`
```html
{% extends 'base.html' %}

{% block style %}
    <link href="//unpkg.com/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
{% endblock %}

{% block content %}
    {% load crispy_forms_tags %}
    <div id="app" class="container">
        <form ref="form" method="post">
        {% csrf_token %}
        {{ form|crispy }}
        <button @click.prevent="HandleStage">暂存</button>
        <button type="submit" @click="HandleSubmit">保存</button>
        </form>
    </div>
{% endblock %}

{% block script %}
    <script src="//unpkg.com/vue@3.2.45/dist/vue.global.js"></script>
    <script src="//unpkg.com/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
    <script>
    // 使用 x-template
    // <script type="x-template" id="TemMain">
    // const App = { template: '#TemMain' }
    // const el = document.body.appendChild(document.createElement('div'))
    const App = {
        delimiters: ['${', '}'],
        components: {},
        data(){
            return {
            };
        },
        mounted(){
            const form = this.$refs['form'];
            const model_name = this.GetModelName(form);
            const jsondata = sessionStorage.getItem(model_name);
            if (null !== jsondata){
                const data = JSON.parse(jsondata);
                Object.entries(data).map(([k,v]) => {
                    form[k].value = v;
                });
            }
        },
        methods: {
            GetModelName: form => form.action.split('/').filter(v => 0<v.length).at(-1),
            HandleStage(ev){
                const form = this.$refs['form']; // as HTMLFormElement
                //blog.csdn.net/qq_41614928/article/details/107533717
                let data = {};
                new FormData(form).forEach((v,k) => data[k]=v); // v,k not k,v
                const model_name = this.GetModelName(form);
                sessionStorage.setItem(model_name, JSON.stringify(data));
            },
            HandleSubmit(){
                const form = this.$refs['form'];
                const model_name = this.GetModelName(form);
                sessionStorage.removeItem(model_name);
            }
        },
    };
    const el = document.getElementById('app');
    if (el){
        Vue.createApp(App).mount(el);
    }
    </script>
{% endblock %}
```

`web/templates/bootstrap5_list.html`
```html
{% extends 'base.html' %}

{% block style %}
    <link href="//unpkg.com/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet">
{% endblock %}

{% block content %}
    <div class="container">
        <table class="table table-striped table-hover">
            <thead>
                <tr>
                    {% for column,v in list.0.items %}
                    <th scope="col">{{ column }}</th>
                    {% endfor %}
                </tr>
            </thead>
            <tbody>
                {% for record in list %}
                <tr>
                    {% for column,v in record.items %}
                    <td>{{ v }}</td>
                    {% endfor %}
                </tr>
                {% endfor %}
            </tbody>
        </table>
    </div>
{% endblock %}

{% block script %}
    <script src="//unpkg.com/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"></script>
{% endblock %}
```
