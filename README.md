Задание 1.
Анализ продаж интернет‑магазина

Условие

Есть интернет‑магазин по продаже электроники. 

Необходимо с помощью SQL‑запросов проанализировать продажи за последний месяц и ответить на ключевые бизнес‑вопросы.

Структура БД
Три связанные таблицы:

products (товары):

sql
product_id INT PRIMARY KEY,
name VARCHAR(100),
category VARCHAR(50),
price DECIMAL(10,2)
orders (заказы):

sql
order_id INT PRIMARY KEY,
user_id INT,
order_date DATE,
status VARCHAR(20)  -- 'completed', 'cancelled'
order_items (позиции в заказах):

sql
item_id INT PRIMARY KEY,
order_id INT,
product_id INT,
quantity INT


Напишите SQL‑запросы для решения следующих вопросов:

Сколько всего заказов было оформлено за последний месяц?

Какова общая выручка за последний месяц (только по завершённым заказам)?

Какой товар был самым популярным (по количеству проданных единиц)?


