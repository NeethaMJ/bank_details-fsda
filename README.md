# bank_details-fsda
Basic operations create table insert values 
show databases
create database if not exists practise_fsda
use practise_fsda

create table bank_details (
age int,
job varchar(35),
marital varchar(35),
education varchar(35),
`default` varchar(15),
balance int,
housing varchar(35),
loan varchar(35),
contact varchar(35),
`day` int,
`month` varchar(35),
duration int,
campaign int,
pdays int,
previous int,
poutcome varchar(35),
y varchar(35) )


insert into bank_details values (30,"unemployed","married","primary","no",1787,"no","no","cellular",19,"oct",79,1,-1,0,"unknown","no")

insert into bank_details values(33,"services","married","secondary","no",4789,"yes","yes","cellular",11,"may",220,1,339,4,"failure","no"),
(35,"management","single","tertiary","no",1350,"yes","no","cellular",16,"apr",185,1,330,1,"failure","no"),
(30,"management","married","tertiary","no",1476,"yes","yes","unknown",3,"jun",199,4,-1,0,"unknown","no"),
(59,"blue-collar","married","secondary","no",0,"yes","no","unknown",5,"may",226,1,-1,0,"unknown","no"),
(35,"management","single","tertiary","no",747,"no","no","cellular",23,"feb",141,2,176,3,"failure","no"),
(36,"self-employed","married","tertiary","no",307,"yes","no","cellular",14,"may",341,1,330,2,"other","no"),
(39,"technician","married","secondary","no",147,"yes","no","cellular",6,"may",151,2,-1,0,"unknown","no"),
(41,"entrepreneur","married","tertiary","no",221,"yes","no","unknown",14,"may",57,2,-1,0,"unknown","no"),
(43,"services","married","primary","no",-88,"yes","yes","cellular",17,"apr",313,1,147,2,"failure","no"),
(39,"services","married","secondary","no",9374,"yes","no","unknown",20,"may",273,1,-1,0,"unknown","no"),
(43,"admin.","married","secondary","no",264,"yes","no","cellular",17,"apr",113,2,-1,0,"unknown","no"),
(36,"technician","married","tertiary","no",1109,"no","no","cellular",13,"aug",328,2,-1,0,"unknown","no"),
(20,"student","single","secondary","no",502,"no","no","cellular",30,"apr",261,1,-1,0,"unknown","yes"),
(31,"blue-collar","married","secondary","no",360,"yes","yes","cellular",29,"jan",89,1,241,1,"failure","no"),
(40,"management","married","tertiary","no",194,"no","yes","cellular",29,"aug",189,2,-1,0,"unknown","no"),
(56,"technician","married","secondary","no",4073,"no","no","cellular",27,"aug",239,5,-1,0,"unknown","no"),
(37,"admin.","single","tertiary","no",2317,"yes","no","cellular",20,"apr",114,1,152,2,"failure","no"),
(25,"blue-collar","single","primary","no",-221,"yes","no","unknown",23,"may",250,1,-1,0,"unknown","no")

select * from bank_details

select count(*) from bank_details

select age, education, job, loan from bank_details

select * from bank_details where education = 'unknown' or marital = 'single'

select * from bank_details where (education = 'unknown' or marital = 'single') and balance <500
