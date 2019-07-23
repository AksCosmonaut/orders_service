Прототип сервиса заказов
=====================
Заказ состоит из двух полей: описание (строка) и стоимость(целое число).
Сервис предоставляет возможность через API:
- создать заказ;
***
    POST /ordersapp/orders/
- удалить заказ;
***
    DELETE /ordersapp/orders/{id заказа}/
- заменить (отредактировать) заказ; 
***
    PUT /ordersapp/orders/{id заказа}/
- посмотреть список заказов;
***
    GET /ordersapp/orders/
- посмотреть отдельный заказ.
***
    GET /ordersapp/orders/{id заказа}/

Запуск
-----------------------------------
1\.  Установка требуемых пакетов
***
    pip install -r requirements.txt
    
2\. 3апуск сервера
***
    python manage.py runserver
    

Тестирование API
-----------------------------------
Tестирование осуществляется с помощью:
***
    python manage.py test