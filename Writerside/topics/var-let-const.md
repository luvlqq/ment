# var, let, const

> Переменные — это именованные контейнеры для хранения данных.
>

Для создания переменной используется ключевое слово **let**, **const** или **var**. Сразу за ключевым словом идёт
название
переменной либо перечень переменных через запятую. Создание переменной также называют объявлением переменной.

```javascript
var singleVariable

let firstVariable, secondVariable, thirdVariable

```

**Для имени переменной можно использовать следующие символы:**

- буквы латинского алфавита;
- цифры;
- символы $ и _.

### **Объявление**

Используя ключевое слово let, можно объявить переменную без присвоения ей начального значения. В таком случае она будет
равна undefined:

```javascript
let a
console.log(a)
// undefined

a = 5
console.log(a)
// 5

```

При помощи const нельзя объявлять переменные без значения:

```JavaScript
const a
// SyntaxError: Missing initializer in const declaration

// Правильно
const b = 5

```

### **Переменные var**

Переменные var можно объявлять без присвоения им значения, в таком случае они будут равны undefined:

```javascript
var a
console.log(a)
// undefined

var b = 5
console.log(b)
// 5

```

Переменные, объявленные через var, имеют функциональную область видимости. Они доступны только в пределах текущей
функции или глобального объекта, если функции нет:

```JavaScript
if (true) {
  var a = 5
}

function foo() {
  var b = 10
}

console.log(a)
// 5
console.log(b)
// ReferenceError: b is not defined

```

Объявление переменных вне функций делает их глобальными переменными. Они доступны как свойства глобального объекта:

```JavaScript
var varVariable = 5

console.log(window.varVariable)
// 5

```

*Подробнее:* [Variables var, let, const](https://doka.guide/js/var-let/)

### **Hoisting**

К переменным, объявленным при помощи ключевого слова var, можно обращаться до момента объявления. В отличие от let и
const, ошибки это не вызовет. Такое поведение называется hoisting - «всплытие»:

```JavaScript
console.log(a)
// undefined

var a = 5

console.log(a)
// 5

```

*Подробнее:* [Hoisting](https://www.dev-notes.ru/articles/what-is-hoisting-in-javascript/)