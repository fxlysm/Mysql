##Mysql 学习##
###创建数据库###
create database testdb;
###删除数据库###
drop database testdb;

###创建表###
create table tbl_user(
id int(3),
name varchar(8),
password varchar(20)
);

###修改表名(重命名）###
alter table tb1_user to tbl_menber

rename table tbl_menber to tb1_user 

###添加字段###
alter table tbl_user add email varchar(255) not null;

###修改字段定义###
alter table tb1_user change id newid int(3);

###删除字段###
alter table tbl_user drop email;

###删除表###
alter table tbl_user;


###获取数据库###

###显示数据库###
show databases;

###使用数据库###
use testdb;

###显示表###
show tables from testdb;

###describe 命令###

###查看表的结构###
describe testdb;

###插入数据###
insert into tbl_user (id, name) values(1,"lambert");

###选择某一数据###
select * from tbl_user  where id=1;

###删除某一数据###
select  from tbl_user  where id=1;

###更新修改数据###
update tbl_user   set name="alice" where id=1;

###逆序排列数据###
select * from tbl_user  order by id desc;
###正序排列数据###
select * from tbl_user  order by id asc;



