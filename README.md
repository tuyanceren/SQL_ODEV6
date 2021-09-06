# SQL_ODEV6
**Patika SQL eğitimi kapsamında yaptığım ödev6**
----------
1._film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?_
```sql
SELECT ROUND(AVG(rental_rate),3) FROM film;
```

2._film tablosunda bulunan filmlerden kaçtanesi 'C' karekteri ile başlar?_
```sql
SELECT COUNT(*) FROM film
WHERE title LIKE 'C%';
```

3._film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?_
```sql
SELECT MAX(length) FROM film
WHERE rental_rate = 0.99;
```

4._film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?_
```sql
SELECT DISTINCT replacement_cost FROM film
WHERE length>150;
```
--------
Sorgu senaryolarını [dvdrental.tar](https://www.postgresqltutorial.com/wp-content/uploads/2019/05/dvdrental.zip) isimli dosyayı indirerek gerçekleştirebilirsiniz.
