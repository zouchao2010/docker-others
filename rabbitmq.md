# rabbitmq

## pull
```shell
docker pull rabbitmq

```

## run(创建并运行一个容器，退出时删除容器)
```shell
docker run  --name rabbitmq \
            -h rabbitmq \
            -p 5672:5672 \
            -v /data/rabbitmq:/var/lib/rabbitmq \
            -e RABBITMQ_DEFAULT_USER=user \
            -e RABBITMQ_DEFAULT_PASS=password \
            -e RABBITMQ_LOGS=/var/lib/rabbitmq/logs/rabbitmq.log \
            -e RABBITMQ_SASL_LOGS=/var/lib/rabbitmq/logs/sasl.log \
            -it --rm rabbitmq
            
```

## run(创建并运行一个容器，以守护进程方式)
```shell
docker run  --name rabbitmq \
            --restart=always \
            -m 1024m \
            -h rabbitmq \
            -p 5672:5672 \
            -v /data/rabbitmq:/var/lib/rabbitmq \
            -e RABBITMQ_DEFAULT_USER=user \
            -e RABBITMQ_DEFAULT_PASS=password \
            -e RABBITMQ_LOGS=/var/lib/rabbitmq/logs/rabbitmq.log \
            -e RABBITMQ_SASL_LOGS=/var/lib/rabbitmq/logs/sasl.log \
            -dt rabbitmq
            
```

## start|stop|restart(已存在的容器)
```shell
docker start|stop|restart rabbitmq

```

## exec(使用已运行的容器执行命令)
```shell
docker exec -it rabbitmq /bin/bash

```
