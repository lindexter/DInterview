# PSQL表继承和视图基础

### 表继承和视图的定义

PSQL支持多表继承

### 如果是字段几乎一样的多表，建议使用表继承

> [PostgreSQL使用表继承实现分区表](http://www.jydba.net/postgresql使用表继承实现分区表/)

![](/assets/服务器后端开发-数据库-PSQL-继承和视图的优缺点-1.png)

> [PostgreSQL表的继承和分区](https://www.cnblogs.com/orangeform/archive/2012/04/27/2291814.html)

### 新建视图命令

```
CREATE VIEW view_hero_order AS
(SELECT * FROM hero_order_8001
UNION
SELECT * FROM hero_order_8002
UNION
SELECT * FROM hero_order_8003)
ORDER BY bet_time DESC
```

### 删除视图

```
DROP VIEW  view_hero_order
```

### 查询视图

```
SELECT * FROM view_hero_order
```



