| 功能 | 命令 |
| :--- | :--- |
| 查看IP | ifconfig |
| 查看使用端口进程 | lsof -i: 端口号 |
| 释放进程 | kill 你的PID |
| 开启Apache | sudo apachectl start |
| 关闭Apache | sudo apachectl stop |
| 重启Apache | sudo apachectl restart |
| 进入保护模式 | 重启过程中按住`command+R`，打开终端输入`csrtil disable` |
| 退出保护模式 | csrtil enable |
| 查看当前目录下文件的权限 | ls -l |
| 显示隐藏文件快捷键 | Command+Shift+. |
| 显示隐藏文件 | defaults write com.apple.finder AppleShowAllFiles -bool true |
| 不显示隐藏文件 | defaults write com.apple.finder AppleShowAllFiles -bool false |
| 重启Nginx | sudo /usr/local/Cellar/nginx/1.19.2/bin/nginx -s reload |
| 查看电脑最大允许连接数 | ulimit -n |
| 当前电脑已建立的连接数 | netstat -n \| grep ESTABLISHED \| wc -l |
| 关掉macbook的USB使用进程 |sudo killall -STOP -c usbd |
|Android代码模板路径 | /Applications/Android Studio.app/Contents/plugins/android/lib/templates/activities |
| 授权路径的权限给用户 | sudo chown -R "用户名" 路径 |
| 启动redis | redis-server |























