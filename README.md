# java-shareit
Тестовая разработка сервиса для шеринга вещей (share - делиться). Это приложение пригодится тем, кому, например, нужна 
вещь для единичного использования. 
Сервис позволяет:
1) Узнать какими вещами готовы поделиться пользователи;
2) Бронировать вещи на определенный срок;
3) Оставлять запрос на определенную вещь, которую не удалось найти в приложении;
4) Оставлять отзывы о вещах, если ими пользовались.
Приложение максимально приближено к рабочей среде - предусмотрено 3 модуля: шлюз для приема запросов, сервер для их
обработки и база данных для хранения данных. Каждый модуль смоделирован на отдельной машине с помощью Docker.

Структура базы данных:
![plot](./ShareIt-ER.png)

Ссылка на ER диаграмму базы данных программы: https://dbdiagram.io/d/650051cb02bd1c4a5e6b13ba

В ветке add-item-requests реализованы интеграционные тесты и мок тестирование каждого слоя приложения: контроллеров, 
сервисов и базы данных.