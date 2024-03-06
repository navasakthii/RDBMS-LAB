## create table borrow
```

create table borrow
	(b_name		varchar2(30),
	 c_name		varchar2(30),
	 l_no		varchar2(3),
	 amt number(10) 
    );
``` 
## inserting values
```
insert into borrow values
('e.palayam','nakul','l1',100000);
insert into borrow values
('v.palayam','krishna','l2',100000);
insert into borrow values
('sb colony','bheem','l3',4000);
insert into borrow values
('k.palayam','arjun','l4',20000);
```
## displaying table 
```
select * from borrow
```
##  create updatable view
```
create view bdetails as (select b_name,c_name from deposit);
```
## display view 
```
select * from bdetails
```
## inserting values in view 
```
insert into bdetails values ('pothanur','addhi');
```
## non updaptable view
```
create view cdetails as 
(select b_name,c_name from deposit) union 
(select b_name,c_name from borrow);
```
## displaying view
```
select * from cdetails
```
## inserting values in non updatable view
```
insert into cdetails values 
('sirumugai','rubi');
```



