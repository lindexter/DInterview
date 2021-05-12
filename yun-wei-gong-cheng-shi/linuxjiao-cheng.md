# 常见问题

#### container bd459109e5c62cc792bf3be1e6f4b265ccd315c941d37fea1238723a9fc6d253: driver "overlay2" failed to remove root filesystem: unlinkat /var/lib/docker/overlay2/9829bcb5512040f61387e9b5449aa163899078c9325034c5eed5b8a615ae06fb/diff/tmp/xmrig: operation not permitted
先去该目录下，把该文件的权限修改，去除i属性
```
chattr -i /var/lib/docker/overlay2/9829bcb5512040f61387e9b5449aa163899078c9325034c5eed5b8a615ae06fb/diff/tmp/xmrig

```
然后删除该文件
```
rm -f /var/lib/docker/overlay2/9829bcb5512040f61387e9b5449aa163899078c9325034c5eed5b8a615ae06fb/diff/tmp/xmrig
```
最后再删除容器