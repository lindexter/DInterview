# Goland配置Dockerfile运行环境

### goland中添加docker配置

![](/assets/服务器后端开发-Go后端开发-Goland用docker部署-2.png)

### 使用命令生成main的docker镜像

```
docker build -t main .
```

![](/assets/服务器后端开发-Go后端开发-goland中docker部署-1.png)

### 运行镜像程序

```
docker run main
```



