Write insert statements to insert the following 5 ingredients:
Eggs
Bread
Beef Patty
Lettuce
Yoghurt
Write a SELECT statement to select the NAME of all the ingredients.
Write a SELECT statement to select the NAME and the PRICE of the ingredients
Write a SELECT statement to select all columns of ingredients, ordered by NAME
Write a SELECT statement to select all columns of ingredients, ordered by "GLUTEN_FREE" with the "true" items on top
--------------------------------------------------------------------------------------------------------------------------------------

SCHEMA

CREATE TABLE INGREDIENT (
  NAME VARCHAR (255),
  CONTAINS_LACTOSE BOOLEAN,
  VEGETARIAN BOOLEAN,
  VEGAN BOOLEAN,
  GLUTEN_FREE BOOLEAN);
  
 INSERT INTO INGREDIENT (NAME,CONTAINS_LACTOSE,VEGETARIAN,VEGAN,GLUTEN_FREE)
 VALUES 
 ('eggs',false,true,false,true),
 ('bread',false,true,true,false),
 ('beef paty',false,false,false,true),
 ('lettuce',false,true,true,false),
 ('yoghurt',true,true,false,true)
 --------------------------------------------------------------------------------------------------------------------------------------
 SQL
 
SELECT NAME FROM INGREDIENT;

SELECT NAME, VEGAN FROM INGREDIENT;

SELECT * FROM INGREDIENT
ORDER BY NAME;

SELECT * FROM INGREDIENT
ORDER BY GLUTEN_FREE DESC;
