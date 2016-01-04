# memcached

## pull
```shell
docker pull memcached

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name memcached \
            -h memcached \
            -p 11211:11211 \
            -it --rm memcached
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name memcached \
            --restart=always \
            -h memcached \
            -p 11211:11211 \
            -dt memcached
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart memcached

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it memcached /bin/bash

```
