## Задача 1

*Ако имате написан string, използвайте него.*

Напишете програма за управление на автосервиз.

В нашия автосервиз могат да бъдат обслужвани автомобили и микробуси. При влизането на всяко превозно средство в сервиза, за него бива въведена следната информация:

- Марка на превозното средство
- Модел на превозното средство
- Година на производство
- Проблем - проблемът е описан в низ, като свободен текст
- Сериозност на проблема - Нисък, Среден, Висок

За автомобилът се въвежда и допълнителна информация:

- Дали автомобилът е на частно лице или на фирма

За микробуса се въвежда и допълнителна информация:

- Дали микробусът превозва пътници или не

Напишете клас, който да пази необходимата информация на сервиз. Направете методи за въвеждане на ново превозно средство, което влиза в сервиза. Направете метод, който показва дали сервиза има капацитет да поеме нов ремонт. Капацитета се изчислява по следния начин, спрямо сериозността на проблема:

- Ниска сериозност на проблема носи 1 точка
- Средна сериозност на проблема носи 3 точки
- Висока сериозност на проблема носи 5 точки

Сервиза може да има най-много 10 точки в даден момент.

## Задача 2

*Не е позволено използването на STL. Позволено е използването на библиотеката `<exception>`, при необходимост*

Напишете клас `ProtectedValue`, който съдържда като член данни:

- Стойност (value), чийто тип е избран от потребителя
- Код за сигурност (code), който е цяло положително число, зададено от потребителя

Достъпът до `value` на `ProtectedValue` се случва само през метод, в който е подаден код от потребителя. Този код трябва да се сравни с `code` на текущата инстанция. Ако двата кода са равни, само тогава трябва да се върне стойността. В противен случай, се връща стойност по подразбиране или се хвърля `std::invalid_argument` (И двата подхода ще се приемат за верни). 

Задаването на `value` се случва само при създаването на обекта, като тогава също се подава и кода за сигурност. 

Напишете клас `ProtectedArray` - разширяващ се масив от `ProtectedValue`. Потребителят може да добавя нови елементи към масива чрез стойност и код, като се спазват същите правила за създаване, както при `ProtectedValue`. Потребителят може да достъпва елементите на `ProtectedArray` чрез метод, който приема два аргумента:

- Индекс, който да бъде достъпен в масива
- Код за сигурност

Ако кодът за сигурност съвпадне, да се върне стойността. Ако кодът за сигурност не съвпадне, да се покаже подходящо съобщение и да се върне стойност по подразбиране.

### Задача 3

[Практически изпит на спец. КН 2020/2021 г.](https://github.com/pvarna/OOP/blob/main/Exam/Task/%D0%9F%D1%80%D0%B0%D0%BA%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%20%D0%B8%D0%B7%D0%BF%D0%B8%D1%82%20%D0%BE%D1%82%2008_00%20%D0%BD%D0%B0%202021-07-07_%20%D0%9F%D1%80%D0%B5%D0%B3%D0%BB%D0%B5%D0%B4%20%D0%BD%D0%B0%20%D0%BE%D0%BF%D0%B8%D1%82.pdf)
