# MySql

* install `docker pull mysql`
* 运行容器
```md
docker run -p 3306:3306 --name mysql --restart=always --privileged=true \
-v /usr/local/mysql/log:/var/log/mysql \
-v /usr/local/mysql/data:/var/lib/mysql \
-v /usr/local/mysql/conf:/etc/mysql/conf.d \
-v /etc/localtime:/etc/localtime:ro \
-e MYSQL_ROOT_PASSWORD=root -d mysql:latest
````


## 可选配置

* `-v /my/own/datadir:/var/lib/mysql:` 为 MySQL 数据持久化存储到主机目录。