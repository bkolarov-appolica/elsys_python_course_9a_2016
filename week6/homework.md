## Задача 1 ##

Разработвате сайт. Направена е форма за регистрация и трябва да напишете скрипт, който валидира никнейма на потребителя. 
Напишете функция ```validate_nickname(nickname)```, която връща ```True``` или ```False``` в зависимост от това 
дали е валидно името. Условията са:
* буквите могат да са и големи и малки и да са от A до Z
* може да има цифрте от 0 до 9
* позволени са само символите '.', '-', '_'

## Задача 2 ##

Формата съдържа и поле за имейл, който също трябва да бъде проверен. Напишете функция ```validate_email(email)```, 
която връща  ```True``` или ```False```, в зависимост от това дали е валиден мейлът. 
Условията са:
* Преди символа '@' е името на имейла. То трябва да спазва следните неща:
    * буквите от a до z (и малки и големи)
    * цифрите от 0 до 9
    * и символите '.', '-', '_'
* След името на имейла трябва да следва знак '@'
* След знака '@' идва името на домейна. Нека то да може да съдържа само:
    * буквите от a до z (само малки)
    * цифрите от 0 до 9
* След домейна трябва да имате '.'
* След точката трябва да имате от 2 до 3 малки букви от a до z.

## Задача 3 ##

След като сте изпълнили задача 1 и задача 2, направете една главна функция на име ```validate_form(nickname, email)```
Направете ```validate_email()``` и ```validate_nickname()``` да бъдат вътрешни за ```validate_form(nickname, email)```. 
Нека ```validate_nickname()``` и ```validate_email()``` вече не приемат аргументи, а вместо това ще ползват тези 
от главната функция.
Направете ```validate_form(nickname, email)``` да връща tuple от двете вътрешни функции като обекти.

#Изисквания към изпълнението:#

* Използвайте Regular Expressions
* Името на файла ви да е &lt;FirstName&gt;_&lt;LastName&gt;_FormValidator.py, където замествате &lt;FirstName&gt; с вашето първо име и &lt;LastName&gt; с вашата фамилия. Имената ги пишете на латиница.

### Hint ###
Точката в regular expressions трябва да бъде ескейпната.
