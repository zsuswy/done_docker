#创建网络
docker network create <xxxxx>

#创建镜像
docker build -t <镜像名字> <上下文路径>

#在网络中运行容器，并指定网络中的别名(network-alias参数)，可以通过name 也可以通过 network-alias访问
docker run -p 0.0.0.0:9000:9000 --name <容器名称> --network <运行网络名称> --network-alias <容器在网络中的别名> jeff_php

#安装ping工具
apt install iputils-ping

#创建数据卷
docker volume create webfiles

#安装PHP扩展
sudo apt-get install php-curl
sudo apt-get install php-xml
sudo apt-get install zip unzip

#mysql权限
grant all on *.* to 'jeff'@'%';