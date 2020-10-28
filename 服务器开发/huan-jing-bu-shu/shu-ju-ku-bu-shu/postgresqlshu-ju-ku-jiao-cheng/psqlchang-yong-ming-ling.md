# PSQL常用命令

| 常用的各种PSQL命令 |  |
| :--- | :------ |
| 查看版本 | pg_ctl -V |
| 初始化PSQL数据库 | initdb /usr/local/var/postgres -E utf8 |
| 启动PSQL | pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start|

<style>
table th:first-of-type {
    width: 20%;
}
table th:nth-of-type(2) {
    width: 30%;
}
</style>




