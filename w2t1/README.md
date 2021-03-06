# Задание

Реализовать телефонную книгу с тремя простыми методами.

## Метод add для добавления записей:

* На вход принимает «Телефон», «Имя» и «Электронную почту».
* Возвращает true или false в зависимости от успеха операции.
* Телефоны принимаются только в формате 5556667788 (без кода).
* Не добавляет запись, если уже существует запись с таким телефоном (телефон – это уникальный идентификатор).
* Не добавляет запись без имени.

## Метод update для обновления записей:

* На вход принимает «Телефон», «Имя» и «Электронную почту».
* Обновляет «Имя» и «Электронную почту» по заданному «Телефону».
* Возвращает true или false в зависимости от успеха операции.
* «Электронную почту» можно стереть (не передав последний параметр), а «Имя» – нет.

## Метод find для поиска по записям:

* На вход принимает запрос в виде строки, например «Алексей».
* Ищет вхождение этой строки хотя бы в одно из полей «Телефон», «Имя» и «Электронную почту».
* Возвращает отсортированный по «Имени» массив строк в формате «name, phone, email».
* Пустой запрос не должен ничего находить.
* Запрос «*» находит все записи.

## Полезные ссылки

* Для решения задачи рекомендуем познакомиться с методами массивов, методами строк и регулярными выражениями.
* Знакомство с платформой Node.js можно начать со статьи «Getting Started With Node.js Tutorial».
* Знакомство с Mocha-тестами можно начать со статьи «Unit Test Your JavaScript Using Mocha and Chai» и раздела «Getting Started» в официальной документации.

## Ошибки

14 of 16 tests passed.
Failed tests: 
не должен обновлять несуществующую запись,
не должен находить записи по пустому запросу