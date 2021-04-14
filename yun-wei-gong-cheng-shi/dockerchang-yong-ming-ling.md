# 常用命令
| 功能 | 命令 |
| :--- | :--- |
| 查看docker的版本 | docker --version |
| 查看docker-compose的版本 | docker-compose --version |
| 查看已下载的镜像 | docker image ls |
| 查看当前正在运行的容器 | docker ps |
| 查看所有容器 | docker ps -a |
| 查看帮助 | docker --help |
| 拉取并运行 nginx 网页服务器，并命名为 webserver | docker run --detach --publish 80:80 --name webserver nginx |
| 进入运行MySQL的docker容器 | docker exec -it mysql /bin/bash |
| 移除容器 | docker rm 容器id |
| 输出系统中各个服务的状态 | systemctl list - units -- type = service |
| 查看服务的运行状态 | systemctl status firewalld |
| 关闭服务 | systemctl stop firewalld |
| 启动服务 | systemctl start firewalld |
| 重新启动服务（不管当前服务是启动还是关闭） | systemctl restart firewalld |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |



































