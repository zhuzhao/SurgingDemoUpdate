# SurgingDemoUpdate
https://github.com/billyang/SurgingDemo    更新Update


让surging 微服务框  demo 跑起来的准备工作     看这个文章  https://www.cnblogs.com/alangur/p/8339905.html
1、下载 安装 erlang：https://www.erlang.org/  最新版就可以  


2、下载并 RabbitMQ    http://www.rabbitmq.com/     

　 cmd 进入rabbitmq安装目录中的sbin目录执行 

　 rabbitmq-plugins enable rabbitmq_management

　 重启rabbitmq服务生效

　 打开http://localhost:15672/即可看到管理后台 （默认的用户名跟密码均是guest，guest不能用于远程访问）


3、下载 consul    地址：https://www.consul.io/downloads.html     
   解压后    consul  路径放到环境变量path 中，cmd 目录下  运行 consul agent -dev  

4、本机数据库，建一个库surging，用sql语句建一个表 ，sql文件在： SurgingDemo\SurgingDemo-master\src\sql
    修改一下，Bill.Demo.DapperCore项目下的 DataBaseConfig.cs 里的数据库连接字符串



打开  这个 SurgingDemo\SurgingDemo-master\src\Bill.Demo.Solutions，还原包    看这篇文章
  https://www.jianshu.com/p/6324626c87b7?tdsourcetag=s_pctim_aiomsg
 设置三个启动项Surging.ApiGateway，Bill.Demo.Services.Server，Bill.Demo.Web
