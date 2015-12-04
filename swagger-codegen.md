# swagger-codegen

## build
```shell
docker build -t zouchao2010/swagger-codegen .

```

## pull
```shell
docker pull zouchao2010/swagger-codegen

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name swagger-codegen \
            -h swagger-codegen \
            -it --rm sbellem/swagger-codegen /bin/bash
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name swagger-codegen \
            -h swagger-codegen \
            -dt zouchao2010/swagger-codegen /bin/bash
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart swagger-codegen

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it swagger-codegen /bin/bash

```
