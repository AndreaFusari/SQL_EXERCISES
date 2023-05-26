schema

CREATE TABLE Customers (
 customer_id INT NOT NULL AUTO_INCREMENT,
 first_name VARCHAR(255) NOT NULL,
 last_name VARCHAR(255) NOT NULL,
 email VARCHAR(255) NOT NULL,
 PRIMARY KEY (customer_id)
);

insert into customers (first_name,last_name,email)
values ('Paolo','Rossi','paolo.rossi@gmail.com'),
('Mario','Pagano','mario.pagano@hotmail.it'),
('Giuseppe','Mazzini','giuseppe.mazzini@yahooo.it'),
('Pietro','Mascagni','pietro.mascagni@alice.it');
-------------------------------------------------------------------------------------------
sql

update customers 
set FIRST_NAME = 'Luca'
where customer_id = 4;

delete from customers 
where customer_id = 1;

truncate customers ;


per delle buone primary keys si possono usare sempre gli id
