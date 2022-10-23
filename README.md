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