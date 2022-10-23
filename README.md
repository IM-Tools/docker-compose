### im-services 环境服务配置

[![OSCS Status](https://www.oscs1024.com/platform/badge/IM-Tools/Im-Services.svg?size=small)](https://www.oscs1024.com/project/IM-Tools/Im-Services?ref=badge_small)

  1.安装使用
```shell
  git clone https://github.com/IM-Tools/docker-compose.git
  cd docker
  docker-compose up -d nsqlookupd nsqd nsqadmin redis mysql
```  
  2.查看容器
```shell
  docker-compose ps
```
  3.配置 .env 文件
  
```shell
MYSQL_VERSION=5.7
MYSQL_DIR=./mysql
REAL_MYSQL_PORT=3306
MYSQL_ROOT_PASSWORD=123456
MYSQL_ROOT_HOST=%

REDIS_VERSION=latest
REDIS_DIR=/redis
REAL_REDIS_PORT=6379

NSQLOOKUPD_TCP_POST=4160
NSQLOOKUPD_HTTP_POST=4161
NSQD_TCP_PORT=4150
NSQD_HTTP_PORT=4151
NSQD_ADMIN_HTTP_PORT=4171

ETCD_PORT=2379
ETCD_MANAGE_PORT=7000
```