# example-of-creating-customer-database-table-in-MySQL
show databases;
create database rcvonlineshop;
use rcvonlineshop;
create table customer 
(   cust_id varchar(8) not null primary key,
    cust_name varchar(40) not null,
	street varchar(250),
    city varchar(50),
    country varchar(20) not null,
    zip_code varchar(8),
    phone varchar(10),
    email varchar(30)
);
select *from customer; 
INSERT INTO customer (cust_id, cust_name, street, city, country, zip_code, phone, email) VALUES
('A12', 'Sam P', 'Melbourne St', 'Cambridge', 'UK', '86736', '234455232', 'sam@rcvacademy.com'),
('A34', 'Ali K', 'Sydney St', 'New York', 'USA', '56236', '4565255232', 'alik@rcvacademy.com'),
('A56', 'Priya S', 'MG St', 'New Delhi', 'India', '659236', '989555232', 'priyas@rcvacademy.com'),
('A78', 'Nitin S', 'Sydney St', 'New York', 'USA', '90989', '98085232', 'nitins@rcvacademy.com'),
('A90', 'Ravi T', 'Sydney St', 'New York', 'USA', '56236', '4565255232', 'alik@rcvacademy.com');
