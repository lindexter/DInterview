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
| 列出当前目录(/)下的所有文件 | ls -l / |
| 获取目前所在工作目录的绝对路径 | pwd |
| 改变当前工作目录 | cd /usr/local |
| 显示或修改系统时间与日期 | date '+%Y-%m-%d %H:%M:%S' |
| 设置用户密码 | passwd root |
| 改变用户身份（切换到超级用户） | su - |
| 用于清除屏幕信息 | clear |
|  |  |
| 输出系统中各个服务的状态 | systemctl list - units -- type = service |
| 查看服务的运行状态 | systemctl status firewalld |
| 关闭服务 | systemctl stop firewalld |
| 启动服务 | systemctl start firewalld |
| 重新启动服务（不管当前服务是启动还是关闭） | systemctl restart firewalld |
| 重新载入配置信息而不中断服务 | systemctl reload firewalld |
| 禁止服务开机自启动 | systemctl disable firewalld |
| 设置服务开机自启动 | systemctl enable firewalld |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |



































