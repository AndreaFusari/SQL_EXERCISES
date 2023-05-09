SCHEMA

CREATE TABLE MEAL (
  NAME VARCHAR (255),
  PRICE DOUBLE,
  CALORIES INT
);
  
CREATE TABLE INGREDIENT (
  NAME VARCHAR(255),
  CONTAINS_LACTOSE BOOLEAN,
  VEGETARIAN BOOLEAN,
  VEGAN BOOLEAN,
  GLUTEN_FREE BOOLEAN
);
  
INSERT INTO MEAL (NAME,PRICE,CALORIES)
VALUES 
('Spaghetti Bolognese', 12.99, 600),
('Grilled Chicken Sandwich', 8.99, 400),
('Pesto Pasta', 10.99, 550),
('Steak and Mash', 19.99, 800),
('Sushi Platter', 15.99, 700); 

INSERT INTO INGREDIENT 
VALUES
('Eggs', false, true, false, true),
('Bread', false, true, true, false),
('Beef Patty', false, false, false, true),
('Lettuce', false, true, true, true),
('Yoghurt', true, true, false, true);

 ---------------------------------------------------------------------------------------------------------------------------------------------
 SQL
 
SELECT * FROM MEAL
WHERE PRICE <15;

SELECT * FROM INGREDIENT
WHERE VEGETARIAN;

SELECT * FROM MEAL
WHERE CALORIES > 500;

SELECT * FROM MEAL
WHERE PRICE > 15 AND PRICE < 16;

SELECT * FROM INGREDIENT
WHERE !CONTAINS_LACTOSE AND GLUTEN_FREE;

SELECT * FROM MEAL
WHERE PRICE < 15 OR CALORIES > 600;

SELECT * FROM INGREDIENT 
WHERE VEGAN OR GLUTEN_FREE;

SELECT * FROM MEAL
WHERE NAME ='Pesto Pasta';

SELECT * FROM INGREDIENT 
WHERE CONTAINS_LACTOSE;

SELECT * FROM MEAL
WHERE PRICE > 20 AND CALORIES < 800;

 
  
