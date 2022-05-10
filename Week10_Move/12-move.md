### NamedObject

Даден е клас `NamedObject`, който ще пази даден обект под някакво име. Всеки `NamedObject` ще съдържа и id (цяло, неотрицателно число, уникално за всеки NamedObject), име (низ с произволна дължина) и обект (който може да бъде от произволен тип).

Създайте подходящ конструктор с параметри, както и подходящи методи за достъп до член-данните на класа. Стойностите на NamedObject се задават само при създаването на обекта.

Придържайте се към "The Rule of Five".

### NamedObjectArray

Даден е клас NamedObjectArray, който ще пази неограничен (до колкото стига паметта) брой инстанции от NamedObjectArray.

- Създайте метод за добавяне на нов NamedObject обект към колекцията. 
- Създайте метод, който връща броя обекти в колекцията. 
- Предефинирайте оператора [], който да връща обекта, съответстващ на даден индекс. 
- Ако индекса е невалиден, да се хвърли изключение out_of_range

---

> Не е позволено използването на STL.
> Спазвайте принципите на ООП. Придържайте се към добрите практики за писане на код.