SCHEMA

CREATE TABLE MEAL_ORDER (
  TIME_MEAL_ORDERED TIMESTAMP DEFAULT NOW(),
  MEAL_NAME VARCHAR(255)
);
  
INSERT INTO MEAL_ORDER 
VALUES 
(NOW(), 'Spaghetti Bolognese'),
(DATE_ADD(NOW(), INTERVAL 1 HOUR), 'Grilled Chicken Sandwich'),
(DATE_ADD(NOW(), INTERVAL 2 HOUR), 'Pesto Pasta'),
(DATE_ADD(NOW(), INTERVAL 3 HOUR), 'Pesto Pasta'),
(DATE_ADD(NOW(), INTERVAL 4 HOUR), 'Grilled Chicken Sandwich'),
(DATE_ADD(NOW(), INTERVAL 5 HOUR), 'Pesto Pasta'),
(DATE_ADD(NOW(), INTERVAL 6 HOUR), 'Spaghetti Bolognese'),
(DATE_ADD(NOW(), INTERVAL 7 HOUR), 'Pesta Pasta'),
(DATE_ADD(NOW(), INTERVAL 8 HOUR), 'Pesto Pasta'),
(DATE_ADD(NOW(), INTERVAL 9 HOUR), 'Spaghetti Bolognese');

CREATE TABLE NUMBERS (
  NUMBER DOUBLE
  );
  
INSERT INTO NUMBERS (NUMBER)
VALUES 
(1.50),
(2),
(3),
(4.78),
(5.892),
(6.10202),
(7),
(8.456),
(9),
(10);
----------------------------------------------------------------------------------------------------------------------------------------------
SQL

# cancatena gli elementi passati come parametri
SELECT
CONCAT(MEAL_NAME, TIME_MEAL_ORDERED) AS STRING_CONCAT FROM MEAL_ORDER;

#ritorna la stringa in lowercase
SELECT 
LOWER(MEAL_NAME) AS LOWERCASE FROM MEAL_ORDER;

# ritorna la stringa in uppercase
SELECT
UPPER(MEAL_NAME) AS UPPERCASE FROM MEAL_ORDER;

# trimma la stringa 
SELECT
TRIM(MEAL_NAME) AS TRIM_NAME FROM MEAL_ORDER;

#ritorna la lunghezza della stringa 
SELECT
LENGTH(MEAL_NAME) AS MEAL_LENGTH FROM MEAL_ORDER;

# ritorna una sottostringa della stringa passata come primo parametro
SELECT
SUBSTRING(MEAL_NAME,1,3) AS FIRST_3_CHAR_MEAL_NAME FROM MEAL_ORDER;

# arrotonda il numero passato nel primo parametro lasciando le cifre decimali specificate nel secondo parametro
SELECT
ROUND(NUMBER, 2) AS ROUNDED_NUMBER FROM NUMBERS;

# formatta i numeri come una stringa specificata dal secondo parametro
SELECT 
FORMAT(NUMBER,'$ #,##') AS FORMATTED_NUMBERS FROM NUMBERS;

# mia data di nascita date_sub sottrae alla data nel primo parametro il tempo specificato nel secondo, date_add aggiunge
SELECT DATE_SUB(DATE_SUB(DATE_SUB(DATE_ADD(DATE_SUB(NOW(),INTERVAL 31 YEAR),INTERVAL 2 MONTH),INTERVAL 1 DAY),INTERVAL 16 HOUR),INTERVAL 23 MINUTE) AS MY_BIRTHDAY_DATE;
