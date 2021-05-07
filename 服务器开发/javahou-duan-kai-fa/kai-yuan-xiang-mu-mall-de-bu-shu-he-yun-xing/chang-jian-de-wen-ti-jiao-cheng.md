# 常见的问题教程

#### docker中elasticsearch启动不了
需要修改内存
```
find /var/lib/docker/ -name jvm.options

```
将##-Xms4g改成-Xms512m
