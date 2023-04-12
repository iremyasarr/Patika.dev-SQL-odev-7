# Patika.dev-SQL-odev-7
Patika.dev &amp; FMSS İş Analisti Practicum SQL ödevi

### ödev sorguları ms sql server üzerinden yazılmıştır.

##### 1.film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
<code> select * from film group by rating; </code>

##### 2.film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
<<code> select * from film group by replacement_cost 
having count(replacement_cost) > 50
order by replacement_cost; </code>>

##### 3.customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?
<<code> select store_id, count(*) as musteri_sayisi from customer group by store_id; </code>>

##### 4.city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız. 
<<code> select top 1 country_id, count(*) as sehir_sayisi from city
group by country_id
order by sehir_sayisi desc; </code>>
