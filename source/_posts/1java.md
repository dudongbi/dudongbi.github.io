---
title: 1java
date: 2023-01-10 17:01:08
tags: java
---

# Spring Boot

## 安装环境

### 运行环境 jdk-11

打开

https://jdk.java.net/java-se-ri/11

下载

https://download.java.net/openjdk/jdk11/ri/openjdk-11+28_windows-x64_bin.zip

### 开发环境 jdk-17

打开

https://jdk.java.net/java-se-ri/17

下载

https://download.java.net/openjdk/jdk17/ri/openjdk-17+35_windows-x64_bin.zip

### vscode 插件

安装

* `Java Extension Pack`

* `Spring Boot Extension Pack`

* `Gradle for Java`

## 脚手架

`Ctrl+Shift+P`，然后输入 `Spring Initializr` 选择 `gradle` 开始

选择

1. Spring Web

1. Thymeleaf

1. Lombok

1. Spring Boot DevTools

1. MySQL Driver

1. Spring Configuration Processor

## 工程设置

### 运行环境 `.vscode/settings.json`

`Ctrl+Shift+P` 输 `json` 选工作区

```json
{
    "java.configuration.runtimes": [
        {
            "name": "JavaSE-11",
            "path": "D:\\app\\jdk-11",
            "default":  true
        },
    ],
    "java.configuration.updateBuildConfiguration": "interactive",
    "java.jdt.ls.java.home": "D:\\app\\jdk-17", // server at least 17+
    "java.compile.nullAnalysis.mode": "automatic",
    "boot-java.rewrite.reconcile": true,
}
```

### 数据库 `application.yml`

```yml
server:
    port: 5173

spring:
    datasource:
        url: jdbc:mysql://db4free.net:3306/springboottest
        username: springbootuser
        password: <password>

mybatis-plus:
    configuration:
        log-impl: org.apache.ibatis.logging.stdout.StdOutImpl
        map-underscore-to-camel-case: true
```

### 仓库 `build.gradle`

```gradle
repositories {
    maven { url 'https://maven.aliyun.com/repository/public/' }
}
dependencies {
    // import javax.persistence.{ Id, Table }
    // implementation 'org.hibernate.javax.persistence:hibernate-jpa-2.1-api:1.0.2.Final'
    // import tk.mybatis.mapper.annotation.{ KeySql }
    // implementation 'tk.mybatis:mapper-spring-boot-starter:4.2.2'
    // maven { url 'https://oss.sonatype.org/content/repositories/snapshots/' }
    implementation 'org.mybatis:mybatis-spring:2.1.0'
    implementation 'com.baomidou:mybatis-plus-boot-starter:3.5.1'
}
```

## 代码

### 主进程 `Application.java`

```java
package com.example.springmvc;

import org.mybatis.spring.annotation.MapperScan;
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
@RestController
@MapperScan("com.example.springmvc.mapper")
public class SpringmvcApplication {

    public static void main(String[] args) {
        SpringApplication.run(SpringmvcApplication.class, args);
    }

    @RequestMapping(value = "/")
    public String hello() {
        return "Hello World";
    }
}
```

### 模型 `bean/UserModel.java`

```java
package com.example.springmvc.bean;

import com.baomidou.mybatisplus.annotation.IdType;
import com.baomidou.mybatisplus.annotation.TableId;
import com.baomidou.mybatisplus.annotation.TableName;
import lombok.Builder;
import lombok.Data;

@Data
@Builder
@TableName(value = "user")//指定表名
public class UserModel {
    // private static final long serialVersionUID = -5644799954031156649L;
    //value与数据库主键列名一致，若实体类属性名与表主键列名一致可省略value
    @TableId(value = "id", type = IdType.AUTO)//指定自增策略
    private Integer id;
    private String name;
    private String sex;
    private String pwd;
    private String email;
}
```

### DAO `mapper/UserMapper.java`

```java
package com.example.springmvc.mapper;
import com.example.springmvc.bean.UserModel;
import org.apache.ibatis.annotations.Mapper;
// import tk.mybatis.mapper.common.BaseMapper;
import com.baomidou.mybatisplus.core.mapper.BaseMapper;

@Mapper
public interface UserMapper extends BaseMapper<UserModel> {
}
```

### 服务+控制 `control/UserController.java`

```java
package com.example.springmvc.control;
import com.example.springmvc.bean.UserModel;
import com.example.springmvc.mapper.UserMapper;
import java.util.List;
import javax.annotation.Resource;

import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.GetMapping; // PostMapping
import org.springframework.web.bind.annotation.ResponseBody;

@Service
class UserService {
    @Autowired
    private UserMapper userMapper;

    public List<UserModel> listAll() {
        return userMapper.selectList(null);
    }
}

@Controller
public class UserController {
    @Resource
    private UserService userService;

    //第一种方式对应的Controller
    @GetMapping(value = "/listUser")
    @ResponseBody
    public List<UserModel> listAll() {
        return userService.listAll();
    }

    //跳转到主页
    @GetMapping(value = "index")
    public String index(){
        return "index";
    }

    //跳转到登录页面
    @GetMapping(value = "login")
    public String login(){
        return "login";
    }
}
```
