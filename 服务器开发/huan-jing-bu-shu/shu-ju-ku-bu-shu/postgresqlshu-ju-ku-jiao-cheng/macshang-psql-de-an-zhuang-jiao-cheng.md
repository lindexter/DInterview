# Mac下PSQL安装与使用教程

### 安装postgresql
```
brew install postgresql
```
### 查看PSQL的版本
```
pg_ctl -V
```
### 安装路径
```
/usr/local/Cellar/postgresql/13.0
```
### 初始化数据库
```
initdb /usr/local/var/postgres -E utf8
```
指定 "/usr/local/var/postgres" 为 PostgreSQL 的配置数据存放目录，并且设置数据库数据编码是 utf8，更多配置信息可以 "initdb --help" 查看
### 设成开机启动 PostgreSQL
```
ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents
launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist
```

### 启动 PostgreSQL
```
pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start
```
### 关闭 PostgreSQL
```
pg_ctl -D /usr/local/var/postgres stop -s -m fast
```



