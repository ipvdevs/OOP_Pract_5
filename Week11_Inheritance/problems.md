## Задача 1 - Inheritance Intro

> По изключение в тази задача е разрешено използването на std::string

Много платформи разчитат на това хем да имат потребители, които ползват системата безплатно, хем да се наложи потребителите да си платят, когато искат да използват повече предложени функционалности.

Като много прост пример може да имаме такава система, в която всички потребители могат да влагат от парите си, но само "премиум" потребителите да ги теглят след това.

Напишете клас `User`, който съдържа:
* `username`
* `email`
* `balance`
* метод `depositMoney(double amount)`, който увеличава `balance` с `amount`.

Напишете клас `PremiumUser`, който освен че съдържа абсолютно всичко изброено за `User`, има още:
* `bankAccountIBAN`
* `subscriptionStartTimestamp` (тип `long`, get-only)
* метод `withdrawMoney(double amount)`, който намалява `balance` с `amount`
* метод `chargeForSubscription()`, който нямалява `balance` с `42`.

## Задача 2 - Refactor

Рефакторирайте кода от задача 1 като използвате използвате `char *` вместо `std::string`.