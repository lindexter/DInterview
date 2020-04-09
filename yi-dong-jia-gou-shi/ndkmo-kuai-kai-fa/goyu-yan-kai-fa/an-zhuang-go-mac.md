# 安装go语言的开发环境

官网：[https://golang.google.cn/](https://golang.google.cn/)

下载安装包![](/assets/移动架构师-NDK开发-go开发-安装golang-1.png)安装完成，测试是否成功：go version

![](/assets/移动架构师-NDK开发-go开发-安装golang-2.png)

查看golang的环境配置：go env

![](/assets/移动架构师-NDK开发-go开发-安装golang-3.png)

###配置go环境变量
```
# Setting go path
export GOROOT=/usr/local/go
export GOPATH=/Users/Dexter/Documents/codingTools/go
export PATH=${PATH}:${GOPATH}/bin:${GOROOT}
# 启用 Go Modules 功能
export GO111MODULE=on
# 配置 GOPROXY 环境变量
export GOPROXY=https://goproxy.io
```





