select * from meal m 
left join ingredient i on m.MEAL_ID = i.MEAL_ID ;

select * from meal m
right join ingredient i on m.MEAL_ID = i.MEAL_ID  

select * 
from meal m
full outer join ingredient i 
on m.MEAL_ID = i.MEAL_ID; 

