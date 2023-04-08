1#SORU - film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.

1#CEVAP - SELECT * FROM film
WHERE title LIKE '%n'
ORDER BY length DESC
LIMIT 5;

1#<img width="960" alt="1" src="https://user-images.githubusercontent.com/129968939/230722855-8826127f-0424-4a5e-9068-a37478ae4257.png">

2#SORU - film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.

2#CEVAP - SELECT * FROM film
WHERE title LIKE '%n'
ORDER BY length
OFFSET 5
LIMIT 5;

2#<img width="960" alt="2" src="https://user-images.githubusercontent.com/129968939/230723240-11de53f8-1307-4558-a248-6290f23d291b.png">

3#SORU - customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.

3#CEVAP - SELECT * FROM customer
WHERE store_id = 1
ORDER BY last_name DESC
LIMIT 4;

3#<img width="960" alt="3" src="https://user-images.githubusercontent.com/129968939/230723568-1316df3b-7930-4d91-9222-709bfb881fc1.png">
