schema
-- main.ingredient definition

CREATE TABLE `ingredient` (
  `NAME` varchar(255),
  `CONTAINS_LACTOSE` tinyint(1),
  `VEGETARIAN` tinyint(1) ,
  `VEGAN` tinyint(1),
  `GLUTEN_FREE` tinyint(1),
  `INGREDIENT_ID` bigint NOT NULL AUTO_INCREMENT,
  PRIMARY KEY (`INGREDIENT_ID`)
) ENGINE=InnoDB AUTO_INCREMENT=37 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
---------------------------------------------------------------------------------------------------------------------------------------
sql

alter table ingredient 
modify NAME VARCHAR(255)not null;

alter table ingredient 
modify CONTAINS_LACTOSE BOOLEAN not null;

alter table ingredient 
modify GLUTEN_FREE BOOLEAN not null;
