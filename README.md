# PostgresSQL MyCheatSheet


### 1. Creating a Table

````sql
CREATE TABLE customer(
first_name VARCHAR(30) NOT NULL,
last_name VARCHAR(30) NOT NULL,
email VARCHAR(60) NOT NULL,
company VARCHAR(60) NOT NULL,
street VARCHAR(50) NOT NULL,
city VARCHAR(40) NOT NULL,
state CHAR(2) NOT NULL,
zip SMALLINT NOT NULL,
phone VARCHAR(20) NOT NULL,
birth_date DATE NULL,
sex CHAR(1) NOT NULL,
date_entered TIMESTAMP NOT NULL,
id SERIAL PRIMARY KEY);
````

### 1. Adding Data to Table

````sql
INSERT INTO customer(first_name, last_name, email, company, street, city, state, zip, phone, birth_date, sex, date_entered)
VALUES ('Jerome', 'Encinares', 'rome@gmail.com', 'AGC', 'Kalayaan Ave','Manila', 'Tondo', '1012', '09510515932', '01-15-1998', 'M', current_timestamp)
````

### 3. Displaying Data from Table

````sql
SELECT * FROM customer
````


