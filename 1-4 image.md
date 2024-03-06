## create table 

```
create table deposit
	(b_name		varchar2(30),
	 c_name		varchar2(30),
	 a_no		varchar2(3),
	 bal number(10) 
    );
``` 

## table description

```
desc deposit;
```
## inserting values 

```
insert into deposit values ('kase','Abimanyu','A1',20000);
insert into deposit values ('palayam','Arjun','A2',10000);
insert into deposit values ('sb colony','Bheem','A3',40000);
```


<!-- below sql is not working in oracle -->
<!-- ### another method to insert multiple values
```
insert into deposit values 
('kase','Abimanyu','A1',20000),
 ('palayam','Arjun','A2',10000),
('sb colony','Bheem','A3',40000);
``` -->



## delete data from a table

```
delete from deposit
```
## displaying table
```
select *  from deposit;
```
## maximum of balance
```
select max(bal) from deposit;
```

## minimum of balance
```
select min(bal) from deposit;
```

## average of balance
```
select avg(bal) from deposit;
```

## sum of balance
```
select sum(bal) from deposit;
```

## count of balance
```
select count(bal) from deposit;
```

## count of c_name
```
select count(c_name) from deposit;
```


## group by value
```
select b_name,max(bal) from deposit group by b_name;
``` 

## group by value
```
select b_name,count(a_no) from deposit group by b_name;
``` 
## having
```
select b_name,max(bal) from deposit group by b_name having max(bal)>15000;
``` 


