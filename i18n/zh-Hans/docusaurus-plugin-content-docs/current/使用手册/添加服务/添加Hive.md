在MySQL数据库中创建Hive相关库
```
CREATE DATABASE IF NOT EXISTS hive DEFAULT CHARACTER SET utf8;
grant all privileges on *.* to hive@"%" identified by 'hive' with grant option;
GRANT ALL PRIVILEGES ON *.* TO 'hive'@'%';
FLUSH PRIVILEGES;
```
点击【服务管理】【添加服务】选择 Hive

![hive-1.png](/i18n/zh-Hans/docusaurus-plugin-content-docs/current/使用手册/imgs/2/hive-1.png)

分配服务Master角色

![hive-2.png](/i18n/zh-Hans/docusaurus-plugin-content-docs/current/使用手册/imgs/2/hive-2.png)

在【服务配置】页面，注意数据库连接参数和数据库用户名密码，安装HiveServer2时会执行sql创建Hive的表，在个别情况下会因mysql配置导致sql执行失败，可根据实际失败原因修改mysql配置。

![hive-3.png](/i18n/zh-Hans/docusaurus-plugin-content-docs/current/使用手册/imgs/2/hive-3.png)

下一步开始安装

![hive-4.png](/i18n/zh-Hans/docusaurus-plugin-content-docs/current/使用手册/imgs/2/hive-4.png)

完成之后在【服务管理】Hive可用查看总览

![hive-5.png](/i18n/zh-Hans/docusaurus-plugin-content-docs/current/使用手册/imgs/2/hive-5.png)

配置页面可以再根据实际需要修改hive服务配置

![hive-6.png](/i18n/zh-Hans/docusaurus-plugin-content-docs/current/使用手册/imgs/2/hive-6.png)
