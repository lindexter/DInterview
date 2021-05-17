# Mac下用Docker部署Mall项目
#### 容器创建
由于macOS系统跟linux有一些区别，需要将/mydata路径改成绝对路径/Users/Dexter/Documents/codingTools/docker/mydata，并把
/Users/Dexter/Documents/codingTools/docker/mydata添加到docker的Preferences->Resources->FILE SETTING中

##### sql容器创建
```
docker run -p 3306:3306 --name mysql \
-v /Users/Dexter/Documents/codingTools/docker/mydata/mysql/log:/var/log/mysql \
-v /Users/Dexter/Documents/codingTools/docker/mydata/mysql/data:/var/lib/mysql \
-v /Users/Dexter/Documents/codingTools/docker/mydata/mysql/conf:/etc/mysql \
-e MYSQL_ROOT_PASSWORD=root  \
-d mysql:5.7
```