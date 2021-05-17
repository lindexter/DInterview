# DockerFile和jar包部署服务器后端

在Dockerfile所在目录执行以下命令  
-t 表示指定镜像仓库名称/镜像名称:镜像标签   
.表示使用当前目录下的Dockerfile

```
docker build -t mall-portal/mall-portal-docker-file:1.0-SNAPSHOT .
```
```
docker run -p 8085:8085 --name mall-portal \
--link mysql:db \
--link redis:redis \
--link mongo:mongo \
--link rabbitmq:rabbit \
-v /etc/localtime:/etc/localtime \
-v /mydata/app/portal/logs:/var/logs \
-d mall-portal/mall-portal-docker-file:1.0-SNAPSHOT
```





