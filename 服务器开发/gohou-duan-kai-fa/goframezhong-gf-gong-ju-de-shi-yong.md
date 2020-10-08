# GoFrame中gf-cli工具的使用

### 安装gf-cli工具

#### mac的gf-cli下载地址

Mac \(amd64\): [https://goframe.org/cli/darwin\_amd64/gf](https://goframe.org/cli/darwin_amd64/gf)

#### 执行安装命令

我使用的是zsh的SHELL工具  
cd到gf下载的目录  
先执行别名命令

```
alias gf=gf
```

```
wget https://goframe.org/cli/linux_amd64/gf && chmod +x gf && ./gf install
```

> 如果没有安装wget，可以使用brew install wget来安装wget工具

#### 查看是否安装成功

```
gf help COMMAND
```

![](/assets/服务器开发-Go后端开发-gf工具的使用-1.png)

> 参考自：[gf-cli的github文档](https://github.com/gogf/gf-cli)


