## MYSQL使用

## 一、安装

1. 找到cmd文件，以管理员身份运行，不然很容易报错。

2. “cd C:\xxxxxx”，更改目录到bin的那个文件夹。

3. “mysqld --initialize –console”输入这句话，然后就会得到自己的初始密码。

4. “mysqld install”安装，“net start mysql”运行。

5. “mysql -u root –p”登入本机数据库。会显示“Enter password”，将刚刚的初始密码输入进去即可，会弹出一大段文字，表示成功运行。

## 二、创建、删除数据库

1. 创建语句 "create DATABASE 名字;"

2. 删除语句 "drop database 名字;"

## 三、创建表并且写入内容

1. 创建语句 

create TABLE 名字（

元素1，数据类型，赋值，

元素2，数据类型，赋值,

元素3，数据类型，赋值,

…

PRIMARY KEY(　元素x )

）ENGINE=InnoDB DEFAULT CHARSE=utf8;

2. 键入内容语句

INSERT INTO 名字

(元素1,元素2,元素3…)

VALUES

(值1，值2，值3…)

## 四、查询表格

使用“select*from 名字;”的语句即可

## 五、删除表格、数据库并且退出

1. 删除表格 "drop TABLE 名字"

2. 删除数据库 "drop DATABASE 名字"

   

# SQLite使用

## 一、安装

  在官网下载解压后，需将文件夹放到path环境下进行操作。

## 二、创建数据库和表

1. 使用".open 文件名"，如果是想打开原有数据库，输入源数据库名即可；如果想新建数据库，输入一个新的名字，就会在sqlite3.exe的同目录下自动生成文件。

2. 创建表格语句

   "CREATE TABLE 名字(

   元素1 数据类型 赋值，

   元素2 数据类型 赋值，

   元素3 数据类型 赋值，)"

3. 测试是否创建成功

   ".tables"语句即可显示

## 三、删除表并退出

1. "drop table 名字"即可删除
2. 再次输入".tables"看是否还有结果，无结果即删除成功
3. ".quit"即可关闭界面退出。

