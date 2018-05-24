# SQL学习笔记

## 1、SQL语句的分类
* SQL方案语句：用于定义存储于数据库中的数据结构
* SQL数据语句：用于操作SQL方案语句所定义的数据结构
* SQL事物语句：用于开始、结束或回滚失误
## 2、SQL：非过程化语句
SQL执行语句的方式交由数据库引擎的一个组件，即优化器（optimizer）处理。
## 3、MySQL简介
* MySQL的默认端口号：`3306`
* MySQL的超级用户：`root`
* MySQL配置文件（Windows）：`安装目录\my.ini`
* 用root用户登录MySQL：`mysql -u root -p`
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
### 修改MySQL提示符
 **方法一：** 连接客户端时通过参数设定
```
shell> mysql -u root -p **** --prompt 提示符
```
 **方法二：** 连接上客户端之后，通过`prompt`命令修改
```
mysql> prompt 提示符
```
 **提示符中可用的转义符** 
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
|转义符|意义|
|:--:|:--:|
|`\D`|完整的日期|
|`\d`|当前数据库|
|`\h`|服务器名称|
|`\u`|当前用户|
