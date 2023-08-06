---
layout: post
title:  一份不错的vue前端代码风格指南
date: 2023-08-06 22:00:00 +0800
description: You can learn front-end basics here . # Add post description (optional)
img: vue.png # Add image post (optional)
tags: [Vue,Project] # add tag
---


- [命名规范](#命名规范)
- [1：项目文件命名](#1项目文件命名)
  - [1.1 项目名](#11-项目名)
  - [1.2 文件目录名](#12-文件目录名)
  - [1.3 图像文件名](#13-图像文件名)
  - [1.4 HTML文件名](#14-html文件名)
  - [1.5 css文件名](#15-css文件名)
  - [1.6 JavaScript文件名](#16-javascript文件名)



## 命名规范

市面上常用的命名规范

+ `camelCase`（小驼峰试命名法——首字母小写）
+ `PascalCase` （大驼峰命名法——首字母大写）
+ `kebab-case` (短横线连接式)
+ `Snake` (下划线连接式)
  
## 1：项目文件命名
### 1.1 项目名
全部采用小写方式，以短横线分隔。例：`my-project-name`
### 1.2 文件目录名

**参照项目命名规则，有复数结构时，要采用复数命名法**。例如：docs，assets，components，directives，mixins，utils，views。
````
my-project-name
|- BuildScript // 流水线部署文件目录
|- docs //项目的细化文档目录 （可选）
|- nginx // 部署在容器上前端项目的nginx代理文件目录
|- node_modules // 下载的依赖包
|- public // 静态页面目录
    ｜- index.html // 项目入口
|- src // 源码目录
    ｜- api // Http请求目录
    ｜- assets // 静态资源目录，这里的资源会被webpack构建
        ｜- icon // icon存放目录
        ｜- img // 图片存放目录
        ｜- js // 公共js目录
        ｜- scss // 公共样式scss存放目录
            — frame.scss // 入口文件
            - global.scss // 公共样式
            - reset.scss // 重置样式
    ｜- components // 组件
    ｜- plugins // 插件
    ｜- router //路由
    ｜- routes // 详细路由拆分目录（可选）
        ｜- index.js
    ｜- store // 全局状态管理
    ｜- utils // 工具存放目录
        ｜- request.js // 公共请求目录
    ｜- views // 页面存放目录
    ｜- app.vue // 跟目录
    ｜- main.js // 入口文件
    ｜- tests // 测试用例
    ｜- .browserslistrc // 浏览器兼容配置文件
    ｜- .editorconfig // 编辑器配置文件
    ｜- .eslintignore // eslint 忽略规则
    ｜- eslintrc.js // eslint 规则
    ｜- .gitignore // git 忽略规则
    ｜- babel.config.js // babel 规则
    ｜- Dockerfile // Docker部署文件
    ｜- jest.config.js 
    ｜- package.json // 依赖
    ｜- README.md  // 项目MD
    ｜- vue.config.js // webpack 配置
````

### 1.3 图像文件名
全部采用小写方式，优先选择单个单词命名，多个单词命名以**下划线**分隔。
````
banner_sina.gif
menu_aboutus.gif
menutitle_news.gif
logo_police.gif
````
### 1.4 HTML文件名
全部采用小写方式，优先选择单个单词命名，多个单词命名以**下划线**分隔。
````
｜- error_report.html
｜- success_report.html
```` 
### 1.5 css文件名
全部采用小写方式，优先选择单个单词命名，多个单词命名以**短横线**分隔。
````
｜- normalize.less
｜- base.less
｜- date-picker.scss
｜- input-number.scss
```` 
### 1.6 JavaScript文件名
全部采用小写方式，优先选择单个单词命名，多个单词命名以**短横线**分隔。
````
｜- index.js
｜- plugins.js
｜- date-util.js
｜- account-module.js
```` 

> 上述规则可以快速记忆为静态文件下划线，编译文件短横线。