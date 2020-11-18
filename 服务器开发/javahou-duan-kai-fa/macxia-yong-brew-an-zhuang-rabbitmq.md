# RabbitMQ教程

### brew命令安装RabbitMQ
```
brew install rabbitmq
```
### 启动RabbitMQ
```
brew services start rabbitmq
```
### 进入控制台

http://localhost:15672/
用户名和密码：guest,guest

### 其他命令
```
## 添加账号
./rabbitmqctl add_user admin admin
## 添加访问权限
./rabbitmqctl set_permissions -p "/" admin ".*" ".*" ".*"
## 设置超级权限
./rabbitmqctl set_user_tags admin administrator
```
