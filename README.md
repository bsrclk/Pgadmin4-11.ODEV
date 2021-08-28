# Pgadmin4-11.ODEV
11.ÖDEV
--11.ÖDEV
--1.SORU actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım

(select first_name from actor
)
union
(select first_name from customer
)

--2.SORU actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.

(select first_name from actor
)
intersect
(select first_name from customer
)

--3.SORU actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.

(select first_name from actor
)
except
(select first_name from customer
)
