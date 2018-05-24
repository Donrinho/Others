# SQL学习笔记

## 1、SQL语句的分类
* SQL方案语句：用于定义存储于数据库中的数据结构
* SQL数据语句：用于操作SQL方案语句所定义的数据结构
* SQL事物语句：用于开始、结束或回滚失误
## 2、SQL：非过程化语句
SQL执行语句的方式交由数据库引擎的一个组件，即优化器（optimizer）处理。
## 3、MySQL
* MySQL的默认端口号：`3306`
* MySQL的超级用户：`root`
* MySQL配置文件（Windows）：`安装目录\my.ini`
* 用root用户登录MySQL：
```
mysql -u root -p
```
### MySQL参数说明
|参数|意义|
|:--:|:--:|
|`-D` 或 `--database=name`|打开指定数据库|
|`--delimiter=name`|指定分隔符，默认为;|
|`-h` 或 `--host=name`|服务器名称|
|`-p` 或 `--password(=name)`|密码|
|`-P` 或 `--port=#`|端口号|
|`--prompt=name`|设置提示符|
|`-u` 或 `--user=name`|用户名|
|`-V` 或 `--version`|输出版本信息并退出|
