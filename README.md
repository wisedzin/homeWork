# My Family Tree Project

## Описание

Это приложение для проведения исследований с генеалогическим древом. Оно позволяет создавать генеалогическое древо, добавлять людей, устанавливать родственные связи между ними и проводить исследование, например, получение всех детей выбранного человека.

## Функционал

- Создание объектов человека (имя, возраст, родители, дети).
- Установка родственных связей между людьми.
- Добавление людей в генеалогическое древо.
- Проведение исследований, таких как получение всех детей выбранного человека.
- Вывод всей структуры генеалогического древа.

### `Person.java`

Класс `Person` представляет человека в генеалогическом древе. Он содержит следующие поля и методы:

- Поля:
  - `name` (имя)
  - `age` (возраст)
  - `father` (отец)
  - `mother` (мать)
  - `children` (список детей)

### `FamilyTree.java`

Класс `FamilyTree` представляет генеалогическое древо и содержит следующие поля и методы:

- Поля:
  - `people` (карта людей, где ключ — имя человека, значение — объект `Person`)

  ### `Main.java`

Основной класс, демонстрирующий использование классов `Person` и `FamilyTree`:

- Создание объектов `Person` с именами Daniyar, Alina, Safia и Amin.
- Установка родственных связей между ними.
- Добавление людей в генеалогическое древо.
- Получение и вывод всех детей Данияра.
- Вывод всей структуры генеалогического древа.

## Пример вывода

Программа выведет в консоль информацию о детях Данияра и структуру всего генеалогического древа:

Children of Daniyar: [Person{name='Safia', age=20}, Person{name='Amin', age=18}]

Person{name='Alina', age=48}

    Person{name='Safia', age=20}
    Person{name='Amin', age=18}

Person{name='Daniyar', age=50}

    Person{name='Safia', age=20}
    Person{name='Amin', age=18}