![alt text](image.png)
...

# Что такое New Date ?

## New Date() в JavaScript используется для создания нового объекта даты.

# Оно делится на 4 типа :

...

## 1. New Date(): Создает новый объект даты с текущей датой и временем.

```js
let d = new Date();
console.log(d);
// Output : 2024-05-09T08:53:57.016Z
```

## 2. New Date(milliseconds): Создает новый объект даты как количество миллисекунд, прошедших с 1 января 1970 года.

```js
let d = new Date(1000000000000);
console.log(d);
// Output : 2001-09-09T01:46:40.000Z
```

## 3. New Date(dateString): Создает новый объект даты из строки даты.

```js
let d = new Date("May 05 , 2024 00:00:00");
console.log(d);
// Output : 2024-05-04T19:00:00.000Z
```

## 4. new Date(year, month, day, hours, minutes, seconds, milliseconds): Создает новый объект даты с указанными значениями.

```js
let d = new Date(2024, 4, 11, 20, 20, 0);
console.log(d);
// Output : 2024-05-11T15:20:00.000Z
```

...

# Date Methods Get :

## 1. getFullYear() : Возвращает год (4 цифры для 4-значных лет) указанной даты.

```js
let d = new Date("2024-05-11");
console.log(d.getFullYear());

// Output : 2024
```

## 2. getMonth() : Возвращает месяц (от 0 до 11) для указанной даты.

```js
let d = new Date("2024-05-11");
console.log(d.getMonth());

// Output : 4
```

## 3. getDate() : Возвращает день (от 1 до 31) для указанной даты.

```js
let d = new Date("2024-05-11");
console.log(d.getDate());

// Output :
```

## 4. getDay() : Возвращает день недели (от 0 до 6) для указанной даты.

```js
let d = new Date("2024-05-11");
console.log(d.getDay());

// Output : 6
```

## 5. getHours(): Возвращает час (от 0 до 23) указанной даты.

```js
let d = new Date("2024-05-11T06:10:22");
console.log(d.getHours());

// Output : 6
```

## 6. getMinutes(): Возвращает минуты (от 0 до 59) указанной даты.

```js
let d = new Date("2024-05-11T06:10:22");
console.log(d.getMinutes());

// Output : 10
```

## 7. getSeconds(): Возвращает секунды (от 0 до 59) указанной даты.

```js
let d = new Date("2024-05-11T06:10:22");
console.log(d.getSeconds());

// Output : 22
```

## 8. getSeconds(): Возвращает миллисекунды (от 0 до 999) указанной даты.

```js
let d = new Date("2024-05-11T06:10:22");
console.log(d.getSeconds());

// Output : 0
```

## 9. getTime(): Метод getTime() в JavaScript используется для получения времени (в миллисекундах) от определенной даты и времени. Это время представляет собой количество миллисекунд, прошедших с полуночи 1 января 1970 года по Гринвичу (GMT), не считая високосные секунды.

```js
let date = new Date();
console.log(date.getTime());

// Output : 1715332252556
```
...

# Что такое new Map ?
## Map в JavaScript - это встроенный объект, который хранит пары ключ-значение и помнит оригинальную последовательность вставки ключей. В отличие от обычных объектов JavaScript, ключи в Map могут быть объектами.

```js
let students = new Map();

students.set('Ismail', 5);
students.set('Abubakrshoh', 4);
students.set('Bilol', 3);

console.log(students.get('Ismail')); // Output: 5


if (students.has('Abubakrshoh')) {
  console.log('Abubakrshoh has in list of students');
}

students.delete('Bilol');

console.log(students.size);

students.forEach((value, key) => {
  console.log(`Студент ${key} имеет оценку ${value}`);
});

```
# Что такое new Set() ?
## Set в JavaScript - это встроенный объект, который позволяет хранить уникальные значения любого типа, будь то примитивные значения или объекты.

```js
let set = new Set();

set.add(1);
set.add(2);
set.add(3);
set.add(2); // Это значение не будет добавлено, так как оно уже есть в наборе

console.log(set.has(1)); // Выводит: true
console.log(set.has(4)); // Выводит: false

console.log(set.size); // Выводит: 3

```