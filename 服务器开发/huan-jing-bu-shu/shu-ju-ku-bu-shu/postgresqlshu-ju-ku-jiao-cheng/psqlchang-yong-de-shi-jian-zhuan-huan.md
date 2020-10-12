# psql常用的时间转换函数

| 函数 | 返回类型 |描述|例子|
| :--- | :---: |:--- |:--- |
| to_char(timestamp, text) | text	|把时间戳转换成字串	|to_char(current_timestamp, 'HH12:MI:SS')|
|to_char(interval, text)	|text	|把时间间隔转为字串	|to_char(interval '15h 2m 12s', 'HH24:MI:SS')|
|to_char(int, text)	|text	|把整数转换成字串	|to_char(125, '999')
|to_char(double precision, text)	|text|	把实数/双精度数转换成字串	|to_char(125.8::real, '999D9')|
|to_char(numeric, text)	|text|	把numeric转换成字串|	to_char(-125.8, '999D99S')|
|to_date(text, text)	|date|	把字串转换成日期|	to_date('05 Dec 2000', 'DD Mon YYYY')|
|to_timestamp(text, text)	|timestamp|	把字串转换成时间戳	to|_timestamp('05 Dec 2000', 'DD Mon YYYY')
|to_timestamp(double)	|timestamp|	把UNIX纪元转换成时间戳|	to_timestamp(200120400)
|to_number(text, text)	|numeric|	把字串转换成numeric|	to_number('12,454.8-', '99G999D9S')|