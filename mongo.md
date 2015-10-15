# mongo

## pull
```shell
docker pull mongo

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name mongo \
            -h mongo \
            -p 27017:27017 \
            -v /data/mongo:/data/db \
            -it --rm mongo
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name mongo \
            -h mongo \
            -p 27017:27017 \
            -v /data/mongo:/data/db \
            -dt mongo
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart liquibook

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it mongo /bin/bash

```
