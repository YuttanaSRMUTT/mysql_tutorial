# สอน MySQL: การสร้างและลบ database และ table (create/drop database and table)

```
$ mysqlsh root@localhost --sql
```

```
SQL > show databases;
```

```
SQL > create database product;
```

```
SQL > show databases;
SQL > use product;
SQL > create table gadget(id int primary key auto_increment,
    -> name varchar(50),
    -> price float);
SQL > create table customer (cust_id int,
    -> fname varchar(50),
    -> lanem varchar(50));
```
* ขั้นตอนการปรับแก้ตาราง 
```
 SQL > alter table customer
    -> add column email varchar(50);
```
```
SQL > describe customer;
```
```
SQL > insert into customer values(43, 'Peter', 'Parker', 'Peter@abc.com');
```
```
SQL > select * from customer;
```

* คำสั่งลบ table ทิ้ง
```
SQL > drop table customer;
```

* คำสั่งลบ database ทิ้ง
```
SQL > drop database product;
SQL > show databases;
SQL > \q
```