# mongo

## pull
```shell
docker pull postgres

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name postgres \
            -h postgres \
            -p 5432:5432 \
            -v /data/postgres:/var/lib/postgresql/data \
            -e POSTGRES_USER=postgres \
            -e POSTGRES_PASSWORD=postgres \
            -it --rm postgres
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name postgres \
            --restart=always \
            -m 1024m \
            -h postgres \
            -p 5432:5432 \
            -v /data/postgres:/var/lib/postgresql/data \
            -e POSTGRES_USER=postgres \
            -e POSTGRES_PASSWORD=postgres \
            -dt postgres
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart postgres

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it postgres /bin/bash

```
