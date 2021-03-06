## Задача 1

Наели са ви да работите за голяма гейминг компания по следващото ѝ голямо заглавие на пазара. Трябва да разработите инвентарна система. След дискусии със дизайнери си нахвърляте в тефтера следните класове, описващи всички видове предмети, които трябва да се поддържат:

#### UpgradeableItem

* level (get)
* upgrade(): level++
* name (get): "{името} ({нивото} LVL)"

#### EquippableItem

* isEquipped (get)
* equip()
* unequip()
* name (get): [{+ или -}] {името} (+, ако е екипиран; - иначе)

#### UpgradeableAndEquippableItem

* level (get)
* upgrade(): level++
* isEquipped (get)
* equip()
* unequip()
* name (get): "[{+ или -}] {името} ({нивото} LVL)"

#### LimitedUpgradeableItem

* maxLevel
* level (get)
* upgrade(): if (level < maxLevel) level++
* name (get): "{името} ({нивото или MAX} LVL)"

#### LimitedUpgradeableAndEquippableItem

* maxLevel
* level (get)
* upgrade(): if (level < maxLevel) level++
* isEquipped (get)
* equip()
* unequip()
* name (get): "[{+ или -}] {името} ({нивото* или MAX} LVL)"

Имплементирайте тези класове като избегнете сблъскването с проблема на диаманта. Създайте още каквито искате допълнителни помощни класове по ваш избор.

## Задача 2.

Създайте опростен калкулатор, при който:

* Всяка константа е израз.
* Всичко от вида `-(израз)` е израз.
* Всичко от вида `(израз)^(константа)` е израз.
* Всичко от вида `(израз + израз)` е израз.
* Всичко от вида `(израз * израз)` е израз.

## Задача 3.

Да се състави складова програма за мебелна къща. Мебелите, които произвежда, са маса, стол и легло. Мебелите имат следните характеристики:

 - маса - идентификатор, височина, широчина, дължина, количество, цена, тип (холова, кухненска)
 - стол - идентификатор, височина, широчина, дължина, количество, цена, тип (дървен, метален, пластмасов)
 - легло - идентификатор, височина, широчина, дължина, количество, цена

 Цената на всеки вид мебел се определя по следния начин:
 - маса - `широчина * дължина * 15`
 - стол - `височина * широчина * 9`
 - легло - `дължина * височина * 22` 

 Всяка мебел да има метод, даващ пълна информация за нейните характеристики.
 
 Нека програмата има опции за:
 - добавяне на нова мебел
 - премахване по идентификатор (намаляване на количеството, а ако стане = 0, премахване на артикула)
 - показване на характеристики на дадена мебел по идентификатор
 - показване на характеристики на най-скъпата мебел
