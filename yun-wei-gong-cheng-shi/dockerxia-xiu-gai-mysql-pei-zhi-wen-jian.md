# Docker下修改mysql配置文件
进入mysql的镜像
docker exec -it mysql /bin/bash
进入要修改的文件目录
cd /etc/mysql
安装vim
如果不安装vim在使用vim的时候会报找不到，在修改docker中mysql的配置文件，无法使用vi命令。
apt-get update
apt-get install vim
修改my.cnf配置文件