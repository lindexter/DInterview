| 功能 | 命令 |
| :--- | :--- |
| 查看IP | ifconfig |
| 查看使用端口进程 | lsof -i: 端口号 |
| 释放进程 | kill 你的PID |
|开启Apache|sudo apachectl start|
|关闭Apache|sudo apachectl stop|
|重启Apache | sudo apachectl restart|
| 进入保护模式 | 重启过程中按住`command+R`，打开终端输入`csrtil disable` |
| 退出保护模式 | csrtil enable |
| 查看当前目录下文件的权限 | ls -l |
| 显示隐藏文件快捷键 | Command+Shift+. |
|显示隐藏文件|defaults write com.apple.finder AppleShowAllFiles -bool true|
|不显示隐藏文件|defaults write com.apple.finder AppleShowAllFiles -bool false|
|重启Nginx|sudo /usr/local/Cellar/nginx/1.19.2/bin/nginx reload|














