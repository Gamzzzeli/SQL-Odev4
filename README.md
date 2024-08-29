# SQL - Odev4

## 1. film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.

``` ruby
SELECT DISTINCT replacement_cost FROM film;
```

## 2. film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?

``` ruby
SELECT COUNT(DISTINCT replacement_cost) FROM film;
```

## 3. film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?

``` ruby
SELECT COUNT(*) FROM film
WHERE title LIKE 'T%' AND rating = 'G';
```

## 4. country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

``` ruby
SELECT COUNT(*) FROM counrty
WHERE country LIKE '_____'; 
```

## 5. city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?

``` ruby
SELECT COUNT(*) FROM city
WHERE city ILIKE '%r';
```