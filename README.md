# dvdrental_odev9
patika.dev dvdrental örnek veri tabanı ile INNER JOIN işlemleri ödev9

1) city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```
SELECT city,country FROM city
INNER JOIN country ON city.country_id = country.country_id ;
```
![1](sorgu_1.jpg)
***
2) customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```
SELECT payment.payment_id,customer.first_name, customer.last_name 
FROM payment
INNER JOIN customer ON payment.customer_id = customer.customer_id ;
```
![2](sorgu_2.jpg)
***
3) customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```
SELECT rental.rental_id,customer.first_name, customer.last_name 
FROM rental
INNER JOIN customer ON rental.customer_id = customer.customer_id ;
```
![3](sorgu_3.jpg)