# sql-odev-3

--1-ülke tablosunda bulunan ülke sütunundaki ülke isimlerinden 'A' karakteri ile mimarisi 'a' karakteri ile sonlananları sıralayınız.
--2-ülke tablosunda bulunan ülke sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
--3-film tablosunda bulunan başlık sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
--4-film tablosunda bulunan tüm sütunlardaki bağlantılardan başlık 'C' karakteri ile başlangıç ​​ve uzunluk (uzunluk) 90 dan büyük olan ve rent_rate 2,99 olan verileri sıralayınız.

1
SELECT * FROM country WHERE country LIKE 'A%a';

2
SELECT * FROM country WHERE country LIKE '_____%n';

3
SELECT title FROM film WHERE title ILIKE '%t%t%t%t%' ;

4
SELECT * FROM film WHERE title ILIKE 'C%' AND rental_rate=2.99 AND length>90 ;
