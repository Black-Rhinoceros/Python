# Python And Mysql
---
### mysql安装和使用

### sql基本语法
~~~sql
select * from city 
update city set Name="wwj" where ID=1
~~~

### 使用pymysql
打开数据库
~~~python
# 打开数据库连接
conn = pymysql.connect(host='127.0.0.1', user='root', passwd='root', db='world', charset='utf8')
# 创建游标对象
cur = conn.cursor()
~~~

**Python查询Mysql使用 fetchone() 方法获取单条数据, 使用fetchall() 方法获取多条数据**
* fetchone(): 该方法获取下一个查询结果集。结果集是一个对象
* fetchall(): 接收全部的返回结果行.
* rowcount: 这是一个只读属性，并返回执行execute()方法后影响的行数。



