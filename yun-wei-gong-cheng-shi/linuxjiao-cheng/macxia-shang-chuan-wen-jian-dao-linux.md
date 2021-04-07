# Mac上传文件到Linux

#### 安装lrzsz命令
```
brew install lrzsz
```
#### 安装iTerm2
https://www.iterm2.com/
#### 安装wget
```
brew install wget
```
#### 下载并安装automatic zmoderm for iTerm2
https://github.com/aikuyun/iterm2-zmodem
iterm2-recv-zmodem.sh
iterm2-send-zmodem.sh
两个文件放在/usr/local/bin/
改变脚本权限
```
sudo chmod 777 /usr/local/bin/iterm2-*
```
#### 配置iTerm2
打开iTerm终端
Profiles—>open Profiles—>Edit Profiles—>Advanced—>Edit Triggers—> 配置如下

| Regular expression | Action |Action |
| :----- | :-- |:--- |
| **B0100 | Run Silent Coprocess | /usr/local/bin/iterm2-send-zmodem.sh |
|**B00000000000000| Run Silent Coprocess	|/usr/local/bin/iterm2-recv-zmodem.sh|




