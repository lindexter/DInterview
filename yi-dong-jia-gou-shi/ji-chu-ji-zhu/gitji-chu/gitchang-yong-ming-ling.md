# Git常用命令

| 命令 | 功能 |
| :--- | :--- |
| git init | git初始化 |
| git add -A | 所有修改文件添加到git中 |
| git commit -m "初始化版本" | 提交代码和注释到本地仓库 |
| git remote -v | 查看远程仓库 |
| git remote rm origin | 删除远程仓库 |
| git remote add \[name\] \[url\] | 添加远程仓库 |
| git remote set-url --push \[name\] \[newUrl\] | 修改远程仓库 |
|git push -u origin master  | 将本地的master分支推送到origin主机 |
| git pull \[remoteName\] \[localBranchName\] | 拉取远程仓库 |
| git push \[remoteName\] \[localBranchName\] | 推送远程仓库 | 
| git branch -a | 查看全部分支 |
| git branch -r | 查看远程分支 |
| git branch -l | 查看本地分支 |
| git checkout \[branch-name\] | 切换分支 |
| git branch -d \[branch-name\] | 删除本地分支 |
| git branch -D \[branch-name\] | 强制删除本地分支 |
| git push origin --delete \[branch-name\] | 删除远程分支 |
| git log | 查看提交日记  q退出 |
| git pull origin next:master | 取回origin主机的next分支，与本地的master分支合并 |
| git stash | 暂存当前正在进行的工作 |
| git stash pop | 恢复未提交的工作 |
| git reset --hard | 放弃merge |
| git config --global --edit | 查看全局的配置文件 |
| git push --set-upstream origin 分支(远端的分支名) | 同步到github上 |
| git push --set-upstream gitlab 分支(远端的分支名) | 同步到gitlab上 |
| git config --global credential.helper store | 记住用户名,密码 |
| git merge master | 合并master到当前分支 |
| git branch --set-upstream-to=origin/master develop  | 为develop分支设置远程关联分支origin主机上的master |
| git checkout -b dev origin/dev | 在origin路径下创建新分支dev |
| git config --global http.sslBackend "openssl"  | 设置全局的配置参数sslbackend为'openssl' |
|  |  |
|  |  |
|  |  |



