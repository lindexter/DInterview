# Docker下禅道部署

### 拉取镜像
```
sudo docker pull easysoft/zentao:15.0.3
```
### 创建docker网络驱动zentaonet
```
sudo docker network create --subnet=172.172.172.0/24 zentaonet
```
### 创建并启动容器
```
sudo docker run --name zentao -p 80:80 --network=zentaonet --ip 172.172.172.172 --mac-address 02:42:ac:11:00:00 -v /www/zentaopms:/www/zentaopms -v /www/mysqldata:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=123456 -d easysoft/zentao:15.0.3
```
### 根据install.php按步骤添加数据库和配置管理员用户
如果出现max_allowed_package
设置mysql的临时执行脚本大小
```
set global max_allowed_packet = 6*1024*1024;
```