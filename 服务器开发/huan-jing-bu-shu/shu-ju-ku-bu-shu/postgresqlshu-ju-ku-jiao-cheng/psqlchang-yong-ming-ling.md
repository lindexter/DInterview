# PSQL常用命令

| 常用的各种PSQL命令 |  |
| :--- | :------ |
| 查看版本 | pg_ctl -V |
| 初始化PSQL数据库 | initdb /usr/local/var/postgres -E utf8 |
| 启动PSQL | pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start|
| 创建数据库用户 | createuser admin |
| 创建一个新数据库lggdb | createdb lggdb -O admin -E UTF-8 -e |





