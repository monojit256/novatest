This is mono project.

Temp project
Tamaghna
Kano Amar project Chori Korli
besh korechi
dara dekachi moja
<?php echo "hello" ?>
create database samsung
use samsung


create table engineer
(
emp_id int identity(100,1),
sname varchar(100),
addr varchar(100),
salary varchar(100),
job_status varchar(100)
)
create table customer
(
cust_id int identity(1,1),
sname varchar(100),
addr varchar(100),
phone varchar(100),
problem varchar(max)
)

--customer insert proc

create proc insertcproc
(
@sname varchar(100),
@addr varchar(100),
@phone varchar(100),
@problem varchar(100))
with encryption
as
insert into customer (sname,addr,salary,job_status
)
values
(@sname,@addr,@phone,@problem)


--customer update proc

create proc updatecproc
(@cust_id int,
@sname varchar(100),
@addr varchar(100),
@phone varchar(100),
@problem varchar(100)
)
with encryption
as
update customer set sname=@sname,addr=@addr,phone=@phone,problem=@problem
where cust_id=@cust_id


//drop table engineer
//drop table customer


--engineer insert proc

create proc insertproc
(
@sname varchar(100),
@addr varchar(100),
@salary varchar(100),
@job_status varchar(100))
with encryption
as
insert into engineer (sname,addr,salary,job_status
)
values
(@sname,@addr,@salary,@job_status)

--engineer update proc

create proc updateproc
(@emp_id int,
@sname varchar(100),
@addr varchar(100),
@salary varchar(100),
@job_status varchar(100)
)
with encryption
as
update engineer set sname=@sname,addr=@addr,salary=@salary,job_status=@job_status
where emp_id=@emp_id