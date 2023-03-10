---
title: 1git
date: 2022-12-27 11:24:43
tags: git
---

# git

`git clone https://<ghp>@github.com/<user>/<repo>.git`
`git clone https://git.sinacloud.com/ddww`

## 使用已有仓库

```
git branch
git remote -v
git remote add origin https://gitee.com/<username>/<repo>.git
git push -f origin master
```

## 更新已有仓库

```
git remote -v
```

```
git remote rm origin
git remote add origin https://gitee.com/dudongbi/css.git
或者
git remote set-url origin https://<你的钥匙>@github.com/dudongbi/pwa-dist.git
```

```
git push -u origin master
```

## 回退版本

```
git log
git reset --hard HEAD^
```

## 删除历史

```
# 新建无历史分支
git checkout --orphan latest_branch
git add -A
git commit -am "init"
git branch
# -D 是 --delete --force
git branch -D master
# -m 是 --move
git branch -m master
git remote
git push -f origin master
```

## 原样保存

```
git config --global core.autocrlf false
```

## 保存密码

保存永久
```
git config --global credential.helper store
```

保存一天（Win），新的已经被`ManagerCore`替代，以下代码失效
```
git config --global credential.helper wincred
git config --global credential.helper 'wincred --timeout=3600'
```

保存一天（Linux）
```
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=86400'
```

清除密码（新Win）
```
git credential-manager-core erase
protocol=https
host=gitee.com
```

清除密码（旧）
```
git config --system --unset credential.helper
git config --edit --system
```

## 修改生效 `.gitignore`

```
git rm -r --cached .
git add .
git commit -m 'update .gitignore'
```
