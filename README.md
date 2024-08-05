![gh_17810254f3db_258](https://github.com/user-attachments/assets/8b51baca-a8f5-4932-87b5-cf6d9fca4ec8)

**郑重声明：项目经过本地测试，确保可以运行。项目仅供学习和毕业设计参考~**

#### 1.项目介绍

技术栈+工具：SpingBoot + RabbitMQ + MySQL5.7 + Maven + IDEA2022 + 微信开发工具

系统功能：图书分类、图书归还、图书删除、图书在线阅读（需授权）、图书借阅、座位预约、预约签到、预约签退等

admin-book ：图书管理端

admin-reserve： 座位预约管理端

mini-app：原生微信小程序

#### 2.项目部署

##### 2.1 后端部署

- 创建数据库，导入项目中的sql文件

- 创建本地RabbitMQ服务，安装比较简单，地址参考：https://blog.csdn.net/qq_25919879/article/details/113055350

- 打开IDEA，open->pom.xml 导入项目admin-book和admin-reserve （打开两个项目）

- 进入 src/main/resources/application.yml 14-18行，根据本地数据库的环境修改数据库连接（两个项目都要改）

- 启动项目即可，无后台管理web

##### 2.2 小程序部署

- 打开微信开发工具， 导入项目mini-app

- 选择测试号即可

- 启动后，微信授权登录，然后用测试号登录， 测试账号/密码： xs001/123456  或者参考user表
