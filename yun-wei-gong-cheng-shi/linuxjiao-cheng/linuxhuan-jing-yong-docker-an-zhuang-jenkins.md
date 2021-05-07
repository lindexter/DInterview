# Linux环境用Docker安装Jenkins

#### 先重启docker

```
systemctl restart  docker
```

#### 再次安装的需要使用这条命令

```
docker run -p 8080:8080 -p 50000:5000 --name jenkins -u root -v /mydata/jenkins_home:/var/jenkins_home -d jenkins/jenkins:lts
```

#### 安装Jenkins推荐的插件

如果安装不了，显示无法连接Jenkins，设置代理后再重试

![](/assets/运维基础-linux教程-安装Jenkins-1.png)

#### Jenkins修改时区
```
System.setProperty('org.apache.commons.jelly.tags.fmt.timeZone', 'Asia/Shanghai')
```

