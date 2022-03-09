SELECT rating,COUNT(*) FROM film
GROUP BY rating;

SELECT replacement_cost,COUNT(*) FROM film
GROUP BY replacement_cost
HAVING COUNT(*)>50
ORDER BY COUNT(*) ASC;

SELECT store_id, COUNT(*) FROM Customer
GROUP BY store_id; --store_id=1(326), store_id=2(273)

SELECT country_id, COUNT(city) from city
GROUP BY country_id
ORDER BY COUNT(city) DESC
LIMIT 1; --country_id=44,count=60
