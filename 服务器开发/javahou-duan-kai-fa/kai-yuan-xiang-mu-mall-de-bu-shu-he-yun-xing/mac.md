# Mac下用Docker部署Mall项目

#### 容器创建

由于macOS系统跟linux有一些区别，需要将/mydata路径改成绝对路径/Users/Dexter/Documents/codingTools/docker/mydata，并把  
/Users/Dexter/Documents/codingTools/docker/mydata添加到docker的Preferences-&gt;Resources-&gt;FILE SETTING中

##### sql容器创建

```
docker run -p 3306:3306 --name mysql \
-v /Users/Dexter/Documents/codingTools/docker/mydata/mysql/log:/var/log/mysql \
-v /Users/Dexter/Documents/codingTools/docker/mydata/mysql/data:/var/lib/mysql \
-v /Users/Dexter/Documents/codingTools/docker/mydata/mysql/conf:/etc/mysql \
-e MYSQL_ROOT_PASSWORD=root  \
-d mysql:5.7
```

#### 拷贝表文件进入docker

```
docker cp /Users/Dexter/Documents/codingTools/JavaProjects/mall/document/sql/mall.sql mysql:/
docker cp /Users/Dexter/Documents/codingTools/JavaProjects/mall/document/sql/lotto.sql mysql:/
```

#### 进入mysql容器，执行mall

```
docker exec -it mysql /bin/bash
mysql -uroot -proot --default-character-set=utf8
show tables;
use mall;
source /mall.sql;
docker run -p 8085:8085 --name mall-portal \
--link mysql:db \
--link redis:redis \
--link mongo:mongo \
--link rabbitmq:rabbitmq \
-v /etc/localtime:/etc/localtime \
-v /mydata/app/portal/logs:/var/logs \
-d mall/mall-portal:1.0-SNAPSHOT
```



