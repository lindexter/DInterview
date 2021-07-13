# Linux中清空docker容器日志
### 新建文件docker-clear-log,放在/usr/local/bin/目录下，文件内容如下：
```
#!/bin/bash -e

if [[ -z $1 ]]; then
    echo "No container specified"
    exit 1
fi

if [[ "$(docker ps -aq -f name=^/${1}$ 2> /dev/null)" == "" ]]; then
    echo "Container \"$1\" does not exist, exiting."
    exit 1
fi

log=$(docker inspect -f '{{.LogPath}}' $1 2> /dev/null)
truncate -s 0 $log
```

### 赋予文件相应的权限，我仅仅给了它所有者读写执行的权限，其他人无权限执行
```
chmod 700 /usr/local/bin/docker-clear-log
```
### 最后，执行命令即可清空相应容器的日志内容
```
docker-clear-log <container>
```