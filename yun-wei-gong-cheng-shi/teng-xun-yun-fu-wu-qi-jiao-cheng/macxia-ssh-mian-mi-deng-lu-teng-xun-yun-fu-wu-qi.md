# Mac下SSH免密登录腾讯云服务器

#### 云服务器创建SSH密钥

![](/assets/运维基础-腾讯云-免密登录-1.png)

#### 新建config文件
```
#腾讯云服务器
Host tencent
        #远程服务器的IP
        HostName 118.24.238.**
        #管理员用户名
        User root
        #登录的密钥
        IdentityFile ~/.ssh/tencent_key.pem                                          
```

#### 登录命令
登录主机名字就是config配置里的Host名字
```
ssh tencent
```



