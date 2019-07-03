  让surging 微服务框  demo 跑起来的准备工作     看这个文章  https://www.cnblogs.com/alangur/p/8339905.html
1、下载 安装 erlang：https://www.erlang.org/  最新版就可以  


2、下载并 RabbitMQ    http://www.rabbitmq.com/


3、 下载 consul    地址：https://www.consul.io/downloads.html       解压后    consul  路径放到环境变量path 中，cmd 目录下  运行 consul agent -dev  

4、本机数据库，建一个库surging，用sql语句建一个表 ，sql文件在： SurgingDemo\SurgingDemo-master\src\sql




打开  这个 SurgingDemo\SurgingDemo-master\src\Bill.Demo.Solutions，还原包    看这篇文章
  https://www.jianshu.com/p/6324626c87b7?tdsourcetag=s_pctim_aiomsg
 设置三个启动项