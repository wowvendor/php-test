Тестовое задание для PHP разботчика
===
Написать простой RestAPI для ecommerce, который:
1. Авторизирует по JSON Web Token;  
2. Позволяет добавить, удалить и отредактировать товар, добавлять новые поля с помощью RestAPI запроса;
3. Позволяет получить список полей товаров;
4. Позволяет получить полную или частичную информацию о товарах (ограничение по заданным полям, по количеству товаров).

Выполнение дополнительных заданий НЕ ЯВЛЯЕТСЯ ОБЯЗАТЕЛЬНЫМ пунктом тестового задания, однако их выполнение добавит вам дополнительные баллы. 

Дополнительное задание №1
---
Реализовать систему банов. Система должна отсеивать нежелательные IP адреса и добавлять любой IP адрес в бан после нескольких неправильных передач токена. CRUD забаненых IP должен осуществляться только CLI скриптом. 

Дополнительное задание №2
---
Реализовать страницу, отображающую добавления, изменения и редактирование последних 5 товаров в реальном времени (история также должна быть сохранена). Страница должна получать информацию только через RestAPI, прямой рендер запрещен. 
Например: При изменении заголовка товара по средствам RestAPI мы сразу должны увидеть оповещение на данной странице: 
```
Товар с ID *** был изменен. Поле title было изменено с Title на TITLE" ** секунд/минут/часов назад. 
```
Время должно динамически меняться. В случае, если ничего не изменялось, время должно меняться на клиенте, и запрос от сервера не должен содержать той информации, которая уже есть на странице. То же самое при добавлении и удалении товара. Оформлять внешний вид страницы не требуется, технологию обмена данными используйте на ваше усмотрение. Допустимая задержка не более 0.5 секунды.

Дополнительное задание №3
---
Реализовать запуск приложения через docker-compose.


Результат
---
Ссылка на публичный Github репозиторий с PHP кодом.

FAQ
---
> Какую версию PHP использовать?

На ваше усмотрение.

> Можно ли использовать фреймворки?

Да, можно.

> Есть ли ограничения по времени?

Нет, время не ограничено.
