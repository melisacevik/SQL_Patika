## SQL 

## Homework 1 

1) SELECT title,description FROM film; 
2) SELECT * FROM film WHERE length > 60 AND length < 75;  
3) SELECT * FROM film WHERE rental_rate = 0.99 AND replacement_cost = 12.99 OR replacement_cost = 28.99; 
4)   SELECT first_name, last_name FROM customer WHERE first_name = ‘Mary’;  
5) SELECT * from filmWHERE NOT length = 50 AND NOT (rental_rate = 2.99 OR rental_rate = 4.99);

## Homework 2 

1) SELECT * FROM film WHERE replacement_cost BETWEEN 12.99 AND 16.99;
2)  SELECT first_name, last_name FROM actor WHERE first_name IN(‘Penelope','Nick','Ed');
3) SELECT * FROM film WHERE rental_rate IN(0.99,2.99,4.99) AND replacement_cost IN(12.99, 15.99, 28.99);

## Homework 3

1) SELECT * from country WHERE country LIKE ‘A%a';
2) SELECT * from country WHERE LENGTH(country) > 6 AND country LIKE ‘%a';
3) SELECT title FROM film WHERE title LIKE ‘%t%t%t%t'
4) SELECT * FROM film WHERE title LIKE 'C%' AND LENGTH > 90 AND rental_rate = 2.99;
