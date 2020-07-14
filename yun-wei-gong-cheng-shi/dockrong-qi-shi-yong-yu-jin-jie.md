# MacOS Docker 安装

## 使用Homebrew安装docker

> Homebrew是一款Mac OS平台下的软件包管理工具，拥有安装、卸载、更新、查看、搜索等很多实用的功能。简单的一条指令，就可以实现包管理，而不用你关心各种依赖和文件路径的情况，十分方便快捷。

```xml
brew cask install docker
```

这种方式经常会卡住下载不了，建议使用国内大公司的下载地址  
阿里docker的下载地址  
[http://mirrors.aliyun.com/docker-toolbox/mac/docker-for-mac/](http://mirrors.aliyun.com/docker-toolbox/mac/docker-for-mac/)  
![](/assets/运维基础-docker-安装与使用-1.png)

> stable是稳定发布版本，beta是g公开测试版本功能新但是可能有bug

![](/assets/运维基础-docker-安装与使用-2.png)

输入系统密码安装完成



## 查看docker的版本

```xml
 docker --version
```

## 镜像加速



