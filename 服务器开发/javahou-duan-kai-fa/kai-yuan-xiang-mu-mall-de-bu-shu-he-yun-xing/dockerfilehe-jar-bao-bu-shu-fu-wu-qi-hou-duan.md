# DockerFile和jar包部署服务器后端

在Dockerfile所在目录执行以下命令
-t 表示指定镜像仓库名称/镜像名称:镜像标签 
.表示使用当前目录下的Dockerfile
```
docker build -t mall-portal/mall-portal-docker-file:0.0.1-SNAPSHOT .
```