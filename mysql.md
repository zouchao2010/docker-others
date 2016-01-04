# mysql

## pull
```shell
docker pull mysql

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name mysql \
            -h mysql \
            -p 3306:3306 \
            -v /data/mysql:/var/lib/mysql \
            -e MYSQL_ROOT_PASSWORD=root \
            -it --rm mysql
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name mysql \
            --restart=always \
            -h mysql \
            -p 3306:3306 \
            -v /data/mysql:/var/lib/mysql \
            -e MYSQL_ROOT_PASSWORD=root \
            -dt mysql
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart mysql

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it mysql /bin/bash

```
