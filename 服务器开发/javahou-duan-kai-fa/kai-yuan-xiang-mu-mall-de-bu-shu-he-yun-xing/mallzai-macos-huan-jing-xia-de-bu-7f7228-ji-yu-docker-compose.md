# mall在MacOS环境下的部署(基于Docker Compose)


#### 下载所有需要安装的Docker镜像
这些配置跟linux下一模一样

#### 创建/mydata/elasticsearch/data目录
```
# 创建目录
mkdir /Users/Dexter/Documents/codingTools/docker/mydata/elasticsearch/data/
# 创建并改变该目录权限
chmod 777 /Users/Dexter/Documents/codingTools/docker/mydata/elasticsearch/data
```
#### 需要拷贝nginx配置文件，否则挂载时会因为没有配置文件而启动失败。
创建nginx文件夹
```
mkdir /Users/Dexter/Documents/codingTools/docker/mydata/nginx/
```
#### 创建logstash文件夹
mkdir /Users/Dexter/Documents/codingTools/docker/mydata/logstash

#### 执行docker-compose-env.yml脚本

