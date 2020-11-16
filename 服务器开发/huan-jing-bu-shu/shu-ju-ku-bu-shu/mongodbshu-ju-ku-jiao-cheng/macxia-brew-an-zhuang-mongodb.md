# Mac下brew安装Mongodb

直接brew install Mongodb有时候会报错

### 使用第三方仓库来安装Mongodb
```
brew tap mongodb/brew
```

### 安装Mongodb的社区版本，也可以加上版本号
```
brew install mongodb-community
```
```
brew install mongodb-community@4.2
```

### 查看是否安装成功
```
mongod --version
```
```xml
db version v4.4.1
Build Info: {
    "version": "4.4.1",
    "gitVersion": "ad91a93a5a31e175f5cbf8c69561e788bbc55ce1",
    "modules": [],
    "allocator": "system",
    "environment": {
        "distarch": "x86_64",
        "target_arch": "x86_64"
    }
}
```

### 创建数据库存放路径以及log路径
```
sudo mkdir -p /usr/local/var/mongodb
sudo mkdir -p /usr/local/var/log/mongodb
```

### 确保当前用户对以上两个目录有读写的权限
```
sudo chown dexter /usr/local/var/mongodb
sudo chown dexter /usr/local/var/log/mongodb
```


