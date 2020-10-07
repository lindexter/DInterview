# 用Brew包管理工具安装go1.15.2

### 如果有旧版本，先卸载

```
brew uninstall go
```

或者用升级命令

```
brew upgrade go
```

### 安装go

```
brew install go
```

### 如果出现卸载不了或者升级不了

直接删除路径下的go文件夹，重新安装最新版本go

### 查看brew安装的go文件路径

```
brew info go
```

### 然后再配置goroot和gopath的环境变量

打开.bash\_profile文件

```
open .bash_profile
```

在.bash\_profile文件中添加如下配置文件

```
# Setting go path
export GOROOT=/usr/local/Cellar/go/1.15.2
export GOPATH=/Users/Dexter/Documents/codingTools/go
export PATH=${PATH}:${GOPATH}/bin:${GOROOT}
# 启用 Go Modules 功能
export GO111MODULE=on
# 配置 GOPROXY 环境变量
export GOPROXY=https://goproxy.io
```



