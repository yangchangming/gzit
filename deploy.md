# 部署相关

## 概要

   基于开源社区symphony的本地IT社区，部署在digetalocean中

## 说明

   1. 修改my.cnf，binlog_format=row

   2. 保持latke为开发模式 runtimeMode=DEVELOPMENT，否则资源文件加载时需要min等资源文件

   3. latke中修改serverPort=8080，保持和jetty一致

   4. init中修改管理员email，admin.email=neocode@126.com

   5. 执行mvn install， 拷贝target下的symphony中的所有文件至jetty/webapps/ROOT中

   6. 启动jetty, java -jar start.jar