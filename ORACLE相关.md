数据表的连接有:
1、内连接(自然连接): 只有两个表相匹配的行才能在结果集中出现
2、外连接: 包括
（1）左外连接(左边的表不加限制)
（2）右外连接(右边的表不加限制)
（3）全外连接(左右两表都不加限制)
3、自连接(连接发生在一张基表内)
有 (+) 的一方代表有可以为空，即副表 where 主表.? = 副表.?(+)
1.select trunc(sysdate) from dual --截取到日
2.select trunc(sysdate, 'mm') from dual --截取到当月第一天.
3.select trunc(sysdate,'yy') from dual --截取到当年第一天
4.select trunc(sysdate,'dd') from dual --截取到当前年月日
5.select trunc(sysdate,'yyyy') from dual --截取到当年第一天
6.select trunc(sysdate,'d') from dual --截取到星期天返回当前星期的第一天
7.select trunc(sysdate, 'hh') from dual --截取到当前时间为
8.select trunc(sysdate, 'mi') from dual --截取到yyyy-mm-dd hh:mi:00 TRUNC()函数没有秒的精确
TRUNC（number,num_digits） 
Number 需要截尾取整的数字。 
Num_digits 用于指定取整精度的数字。Num_digits 的默认值为 0。
TRUNC()函数截取时不进行四舍五入
9.select trunc(123.458) from dual --123
10.select trunc(123.458,0) from dual --123
11.select trunc(123.458,1) from dual --123.4
12.select trunc(123.458,-1) from dual --120
13.select trunc(123.458,-4) from dual --0
14.select trunc(123.458,4) from dual --123.458
15.select trunc(123) from dual --123
16.select trunc(123,1) from dual --123
17.select trunc(123,-1) from dual --120
