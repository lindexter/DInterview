# MacbookPro修改睡眠耗电教程

### 查看休眠模式的耗电模式

```
pmset -g
```

![](/assets/工具-MacBook-休眠模式耗电修改-1.png)

### 修改hibernatemode的数值
```
sudo pmset -a hibernatemode 25
```
如果想达到合盖上屏幕和关机的效果
```
sudo pmset -b tcpkeepalive 0
```
>该设置会停止合上屏幕的下载文件，合盖即断网
