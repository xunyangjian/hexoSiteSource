---
layout: post
title: Heroku
subtitle:   ""
date:       2016-07-25
author:     "shijian.yang"
header-img: "heroku.jpg"
tags:
	-  server 
	-  heroku
---

> Heroku[官网](https://www.heroku.com/)
> 本文主要记录个人在使用heroku的过程中遇到的问题及解决方案，如有问题欢迎回复邮件讨论。

### 持续更新中

#### 1.heroku数据库服务mLab的用户及密码

>	heroku config -s -a [project_name]
>	out:$ mongodb://<dbuser>:<dbpassword>@[标识].mlab.com:21922/[dataBase]

#### 2.heroku 部署（Deploy）
  
> 部署方式：heroku支持[Github](https://github.com/),DropBox,Hero Git的方式部署代码。首次部署成功之后，选择自动部署【Automatic deploys】Github上提交代码之后heroku会自动部署最新的代码；

![deploy method](./deploy_method.png)

> 停止服务：<项目>/<Settings>打开【Maintenance mode】

![stop server](./stop_server.png)

