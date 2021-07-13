# 常用命令
| 功能 | 命令 |
| :--- | :--- |
| 启动容器 | docker start 容器ID |
| 停止容器 | docker stop 容器ID |
| 移除容器 | docker rm 容器id |
| 移除镜像 | docker rmi 镜像id |
| 进入容器-1 | docker attach 容器ID |
| 进入容器-2 | docker exec -it 容器ID /bin/bash  |
| 进入容器-3 | docker exec -it 容器的name bash |
| 查看docker的版本 | docker --version |
| 退出容器 | exit |
| 查看容器的日志 | docker logs 容器 |
| 查看docker-compose的版本 | docker-compose --version |
| 查看已下载的镜像 | docker image ls |
| 查看当前正在运行的容器 | docker ps |
| 查看所有容器 | docker ps -a |
| 查看帮助 | docker --help |
| 拉取并运行 nginx 网页服务器，并命名为 webserver | docker run --detach --publish 80:80 --name webserver nginx |
| 进入运行MySQL的docker容器 | docker exec -it mysql /bin/bash |
| 重新加载配置 | systemctl daemon-reload |
| 重启docker | systemctl restart docker |
| 清除没有使用的无效镜像 | docker image prune |
| 部署禅道 | sudo docker pull easysoft/zentao:15.0.3 |




































