# FastAdmin框架常见问题

## FastAdmin代码同步到git，再拉取后报错unserialize\(\): Error at offset 0 of 17039 bytes

从git拉取到本地在配置网址登录后出现 unserialize\(\): Error at offset 0 of 17039 bytes

找到**\thinkphp\library\think\cache\driver\Flie.php**中的
```
$content=substr($content,32)
```
改为
```
$content=substr($content,
17071);
```
若还报此错在加上对应的bytes值即可  
正常显示后可改回原来的值
>参考：https://blog.csdn.net/yqwwj001/article/details/88688675



