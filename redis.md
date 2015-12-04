# mongo

## pull
```shell
docker pull redis

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name redis \
            -h redis \
            -p 6379:6379 \
            -v /data/redis:/data \
            -it --rm redis
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name redis \
            --restart=always \
            -h redis \
            -p 6379:6379 \
            -v /data/redis:/data \
            -dt redis
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart redis

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it redis /bin/bash

```
