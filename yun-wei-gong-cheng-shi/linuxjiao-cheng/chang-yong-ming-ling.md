# 常用命令
| 功能 | 命令 |
| :--- | :--- |
| ssh root@118.24.238.82 | 远程登录linux服务器 |
| mkdir test | 新建test文件夹 |
| mv a b c d | 将abc三个文件移动到d文件夹 |
| 创建text.txt文件 | touch text.txt |
| 删除文件 | rm text.txt |
| 强制删除某个目录及其子目录 | rm -rf testdir/ |
| 将test1目录复制到test2目录 | cp -r /mydata/tes1 /mydata/test2 |
| 压缩与解压 | tar |
| 列出当前目录(/)下的所有文件 | ls -l / |
| 获取目前所在工作目录的绝对路径 | pwd |
| 改变当前工作目录 | cd /usr/local |
| 显示或修改系统时间与日期 | date '+%Y-%m-%d %H:%M:%S' |
| 设置用户密码 | passwd root |
| 改变用户身份（切换到超级用户） | su - |
| 用于清除屏幕信息 | clear |
| 显示指定命令的帮助信息 | man ls |
| 查询系统处于什么运行级别 | who -r |
| 显示目前登录到系统的用户 | who -buT |
| 显示系统内存状态（单位MB） | free -m |
| 显示系统进程运行动态 | ps -ef |
| 查看sshd进程的运行动态 | ps -ef \|grep sshd |
| 输出系统中各个服务的状态 | systemctl list - units -- type = service |
| 查看服务的运行状态 | systemctl status firewalld |
| 关闭服务 | systemctl stop firewalld |
| 启动服务 | systemctl start firewalld |
| 重新启动服务（不管当前服务是启动还是关闭） | systemctl restart firewalld |
| 重新载入配置信息而不中断服务 | systemctl reload firewalld |
| 禁止服务开机自启动 | systemctl disable firewalld |
| 设置服务开机自启动 | systemctl enable firewalld |
