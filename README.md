# bbrkrw
лабораторная по базам данных
таблица orders
1) Выберите из таблицы orders все заказы
Решение:
SELECT * FROM orders;
![1](https://github.com/user-attachments/assets/50d31762-e5bb-4eb6-9c2c-3379427353f7)

2) Выберите из таблицы orders все заказы кроме новых. У новых заказов status равен "new". Использовать in
Решение:
SELECT * FROM orders
WHERE STATUS IN ('cancelled', 'in_progress', 'delivery');
![2](https://github.com/user-attachments/assets/a05c4d07-5f7d-4d57-9d9e-e4b5f46bc7ae)

3) Выберите из таблицы orders все новые и отмененные заказы. У отмененных заказов status равен "cancelled". У новых заказов status равен "new".
Решение:
SELECT * FROM orders
WHERE STATUS IN ('cancelled', 'new');
![3](https://github.com/user-attachments/assets/7a125a5a-e8cd-48a4-a6b5-b263a4ba46a1)

4) Выберите из таблицы orders все заказы содержащие более 3 товаров (products_count).
Вывести нужно только номер (id) и сумму (sum) заказа.
Решение:
SELECT id, sum FROM orders
WHERE products_count > 3;
![4](https://github.com/user-attachments/assets/3ffc277b-78d6-4870-86f3-41a4eb6c4f55)
