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

## Homework 4

1) SELECT DISTINCT(replacement_cost) FROM film;
2) SELECT COUNT(DISTINCT replacement_cost) FROM film;
3) SELECT COUNT(DISTINCT title = 'T%' AND rating = 'G') FROM film;
4) SELECT COUNT(*) FROM country WHERE LENGTH(country) = 5;
5) SELECT COUNT(city) FROM city WHERE city LIKE 'R%r';

## Homework 5
1) SELECT * FROM film WHERE title LIKE ‘%n' ORDER BY length LIMIT 20;
2) SELECT * FROM film WHERE title LIKE ‘%n' ORDER BY length offset 5 limit 5;
3) SELECT * FROM customer WHERE store_id = 1 ORDER BY last_name DESC limit 4;

## Homework 6
1) SELECT ROUND(AVG(rental_rate),4) FROM film;
2) SELECT COUNT(*) FROM film WHERE title LIKE ‘C%'
3) SELECT MAX(length) FROM film WHERE rental_rate = 0.99;
4) SELECT COUNT(replacement_cost) FROM film WHERE length > 150;

## Homework 7
1) SELECT rating,COUNT(*) FROM film GROUP BY rating;
2) SELECT replacement_cost, COUNT(*) FROM film GROUP BY replacement_cost  HAVING COUNT(*) > 50;
3) SELECT store_id,COUNT(*) FROM customer GROUP BY store_id;
4) SELECT country_id, COUNT(*) FROM city GROUP BY country_id ORDER BY COUNT(*) DESC LIMIT 1;

## Homework 8

1) CREATE TABLE employee(
	id INTEGER PRIMARY KEY, 
	name VARCHAR(50), 
	birthday DATE, 
	email VARCHAR(100)
);

2) insert into employee (id, name, birthday, email) values (1, 'Wally', '1990-10-16', 'wbusfield0@bloomberg.com');
insert into employee (id, name, birthday, email) values (2, 'Kelwin', '1990-11-05', 'kkynaston1@vinaora.com');
insert into employee (id, name, birthday, email) values (3, 'Madlin', '1997-05-10', 'moxbrough2@nydailynews.com');
insert into employee (id, name, birthday, email) values (4, 'Gabrielle', '1997-04-16', 'gcordon3@who.int');
insert into employee (id, name, birthday, email) values (5, 'Morty', '1993-05-15', 'msworder4@xing.com');
insert into employee (id, name, birthday, email) values (6, 'Innis', '2000-04-21', 'ipalmby5@drupal.org');
insert into employee (id, name, birthday, email) values (7, 'Walden', '1999-02-20', 'wmcilwreath6@vkontakte.ru');
insert into employee (id, name, birthday, email) values (8, 'Enrique', '1993-10-03', 'evanschafflaer7@mapy.cz');
insert into employee (id, name, birthday, email) values (9, 'Dimitry', '2000-03-17', null);
insert into employee (id, name, birthday, email) values (10, 'Tarra', '1997-04-17', 'tzannini9@mac.com');
insert into employee (id, name, birthday, email) values (11, 'Arman', '1992-06-16', 'amccreerya@hubpages.com');
insert into employee (id, name, birthday, email) values (12, 'Munroe', '1992-10-10', null);
insert into employee (id, name, birthday, email) values (13, 'Lidia', '1995-03-27', 'lhaggertyc@earthlink.net');
insert into employee (id, name, birthday, email) values (14, 'Ashla', '1995-12-25', 'alymerd@si.edu');
insert into employee (id, name, birthday, email) values (15, 'Margaretha', '1997-07-12', 'mcurnowe@xing.com');
insert into employee (id, name, birthday, email) values (16, 'Justen', '1992-06-24', 'jbrettorf@deliciousdays.com');
insert into employee (id, name, birthday, email) values (17, 'Tammie', '1999-05-15', 'tdottridgeg@163.com');
insert into employee (id, name, birthday, email) values (18, 'Viviana', '1999-06-17', 'vbensusanh@theglobeandmail.com');
insert into employee (id, name, birthday, email) values (19, 'Tina', '1990-09-10', 'tdollingi@abc.net.au');
insert into employee (id, name, birthday, email) values (20, 'Vergil', '1993-06-23', null);
insert into employee (id, name, birthday, email) values (21, 'Ralf', '1995-04-22', 'rdeyesk@epa.gov');
insert into employee (id, name, birthday, email) values (22, 'Floris', '1997-06-28', 'fwhebelll@umn.edu');
insert into employee (id, name, birthday, email) values (23, 'Lovell', '1992-07-16', 'lninnolim@cargocollective.com');
insert into employee (id, name, birthday, email) values (24, 'Lita', '1999-03-10', 'lfolliottn@nytimes.com');
insert into employee (id, name, birthday, email) values (25, 'Karee', '2000-02-15', 'klarmano@berkeley.edu');
insert into employee (id, name, birthday, email) values (26, 'Jeffie', '1994-10-01', 'jwoodroofp@bloglovin.com');
insert into employee (id, name, birthday, email) values (27, 'Freeland', '1997-03-22', 'fesilmonq@1und1.de');
insert into employee (id, name, birthday, email) values (28, 'Frasquito', '1997-10-20', 'fbrider@ucla.edu');
insert into employee (id, name, birthday, email) values (29, 'Muhammad', '1994-02-23', 'mjodlowskis@altervista.org');
insert into employee (id, name, birthday, email) values (30, 'Orelle', '1997-08-13', null);
insert into employee (id, name, birthday, email) values (31, 'Tiff', '1994-02-09', 'tcruikshanku@mozilla.com');
insert into employee (id, name, birthday, email) values (32, 'Sal', '2000-02-21', 'sgrosierv@loc.gov');
insert into employee (id, name, birthday, email) values (33, 'Corrinne', '1996-10-23', 'cgorioliw@bloomberg.com');
insert into employee (id, name, birthday, email) values (34, 'Meg', '1997-09-30', 'mserjeantsonx@vkontakte.ru');
insert into employee (id, name, birthday, email) values (35, 'Yevette', '1992-05-20', 'ykivelley@reverbnation.com');
insert into employee (id, name, birthday, email) values (36, 'Suellen', '1991-09-14', 'sburberyez@walmart.com');
insert into employee (id, name, birthday, email) values (37, 'Carline', '2000-03-28', 'cseckington10@amazon.co.jp');
insert into employee (id, name, birthday, email) values (38, 'Hakim', '1996-12-25', 'hlesarr11@mlb.com');
insert into employee (id, name, birthday, email) values (39, 'Kai', '1998-05-22', 'kcestard12@discuz.net');
insert into employee (id, name, birthday, email) values (40, 'Bethena', '1991-06-09', 'bmazey13@hugedomains.com');
insert into employee (id, name, birthday, email) values (41, 'Lilli', '1990-09-12', 'lradki14@jugem.jp');
insert into employee (id, name, birthday, email) values (42, 'Llywellyn', '1990-08-25', 'lglazebrook15@princeton.edu');
insert into employee (id, name, birthday, email) values (43, 'Janette', '1997-04-24', null);
insert into employee (id, name, birthday, email) values (44, 'Giana', '1996-01-18', 'gtellett17@loc.gov');
insert into employee (id, name, birthday, email) values (45, 'Ram', '1995-06-01', 'rmungin18@noaa.gov');
insert into employee (id, name, birthday, email) values (46, 'Britni', '1991-04-05', 'bkinglake19@google.com.au');
insert into employee (id, name, birthday, email) values (47, 'Nicola', '2000-02-18', 'nisaacson1a@twitpic.com');
insert into employee (id, name, birthday, email) values (48, 'Dorey', '1994-06-16', 'dadamthwaite1b@quantcast.com');
insert into employee (id, name, birthday, email) values (49, 'Brod', '1991-06-27', 'btomney1c@booking.com');
insert into employee (id, name, birthday, email) values (50, 'Sampson', '1991-02-18', 'syirrell1d@springer.com');
  

3) UPDATE employee
SET name = 'Çağrı',
	birthday = '1997-08-30',
	email = 'cagri@cagri'
WHERE id = 10;

UPDATE employee
SET name = 'Melisa',
	birthday = '1998-10-03',
	email = 'melisa@melisa'
WHERE id = 5;	

4) DELETE FROM employee
WHERE id= 2;

DELETE FROM employee
WHERE id= 3;

## Homework 9

1) SELECT country,city FROM country INNER JOIN city ON country.country_id = city.country_id;
2) SELECT payment_id, first_name,last_name FROM customer INNER JOIN payment ON payment_id = payment.payment_id;
3) SELECT rental_id, first_name, last_name FROM customer INNER JOIN rental ON customer.customer_id = rental.customer_id;

## Homework 10

1) SELECT country,city FROM country LEFT JOIN city ON country.country_id = city.country_id;
2) SELECT payment_id, first_name,last_name FROM customer  RIGHT JOIN payment ON payment_id = payment.payment_id;
3) SELECT rental_id, first_name, last_name FROM customer  FULL JOIN rental ON customer.customer_id = rental.customer_id;

## Homework 11

1)   (SELECT first_name FROM actor)UNION(SELECT first_name FROM customer)
2) (SELECT first_name FROM actor) INTERSECT (SELECT first_name FROM customer)
3) (SELECT first_name FROM actor)EXCEPT(SELECT first_name FROM customer)
4)  ALL 

## Homework 12

1) SELECT COUNT(*) FROM film
WHERE length > ( SELECT AVG(length) FROM film);  
2) SELECT COUNT(*) FROM film
WHERE rental_rate = (SELECT MAX(rental_rate) FROM film)

3) SELECT * FROM film 
WHERE rental_rate = (SELECT MIN(rental_rate) FROM film) AND replacement_cost = (SELECT MIN(replacement_cost) FROM film);

4) SELECT * FROM customer  INNER JOIN (SELECT COUNT(*) A, customer_id FROM payment
GROUP BY customer_id
) count_purchases
ON customer.customer_id = count_purchases.customer_id
ORDER BY A DESC
LIMIT 3;
