## What is Docker

### 基本名詞解釋

- Image
- Container
	([What is a container](https://www.docker.com/what-container))
- Registry
- Volume
- Port
- Network


## 架構

![](https://github.com/softleader/maintain-tutorial/blob/master/structure.png)

## 過版指令

pull image

```
$ docker pull localhost:5000/${image}:${tag}
```

load image

```
$ docker load -i {image}.tar
```

列出 stack

```
$ docker stack ls
```

列出 service

```
$ docker service ls
```

檢查 service

```
$ docker service ps 
```

查看 service 的 log

```
$ docker service logs ${service id}
```

部署 stack

```
$ docker stack deploy -c ${docker-compose.yml} ${stack name}
```

移除 stack

```
$ docker stack rm $(stack name}
```

### 可能會用到的指令

查看 container log

```
$ docker logs ${container id}
```

查看 container 使用狀況

```
$ docker stats (container id)
```
