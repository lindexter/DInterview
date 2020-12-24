| 功能 | 命令 |
| :--- | :--- |
| 列出指定目录下的所有文件 | ls -l / |
| 获取目前所在工作目录的绝对路径 | pwd |
| 改变当前工作目录 | cd /usr/local |
| 显示或修改系统时间与日期 | date '+%Y-%m-%d %H:%M:%S' |
| 设置用户密码 | passwd root |
| 输出系统中各个服务的状态 | systemctl list-units --type=service |
| 查看firewalld服务的运行状态 | systemctl status firewalld |
| 关闭firewalld服务 | systemctl stop firewalld |
| 启动firewalld服务 | systemctl start firewalld |
| 重新启动服务（不管当前服务是启动还是关闭） | systemctl restart firewalld |
| 重新载入配置信息而不中断服务 | systemctl reload firewalld |
| 禁止服务开机自启动 | systemctl disable firewalld |
| 设置服务开机自启动 | systemctl enable firewalld |


