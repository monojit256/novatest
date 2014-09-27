this is mono project.

Temp project
Tamaghna
Kano Amar project Chori Korli
besh korechi
dara dekachi moja
<?php echo "hello" ?>
create database samsung
use samsung

 o enable the Advanced help module, select the checkbox next to Advanced help. To
dules
Once you have enabled a new module, you should check to see if there are any
configuration options for the module. To do this, look in the OPERATIONS
column of the Modules page.

enable the Ctools module, select the checkbox next to Chaos tools. To enable the Views
module, select the checkboxes next to the Views and Views UI modules. Click on the
Save configuration button to save your settings and enable your modules. You will
receive a confirmation message at the top of the screen.

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
