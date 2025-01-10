# Functions

В JavaScript функции являются фундаментальным строительным блоком, позволяющим организовывать и структурировать код для
выполнения определенных задач.

### **Function Declaration**

```javascript
function greet(name) {
  return "Привет, " + name + "!";
}

```

*Подробнее:* [Function Declaration](https://learn.javascript.ru/function-basics)

Функции, объявленные таким способом, могут быть вызваны до того, как код, содержащий их, выполнится.

### **Function Expression**

```javascript
const greet = function (name) {
  return "Привет, " + name + "!";
};

```

В этом случае, функция присваивается переменной. Такие функции могут быть вызваны только после того, как они были
определены.

*Подробнее:* [Function Expression](https://learn.javascript.ru/function-expressions)

### **Стрелочная функция**

```javascript
const greet = (name) => {
  return "Привет, " + name + "!";
};

```

Стрелочные функции представляют сокращенный синтаксис для функциональных выражений и предоставляют более лаконичный
способ определения функций.

*Подробнее:* [Стрелочная функция](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

### **IIFE (Immediately Invoked Function Expression)**

```javascript
(function () {
  // код
})();

```

Это функциональное выражение, которое вызывается сразу после объявления. Оно помогает изолировать переменные и функции
от глобальной области видимости.

*Подробнее:* [IIFE](https://developer.mozilla.org/ru/docs/Glossary/IIFE)

### **Генераторы**

```javascript
function* generateSequence() {
  yield 1;
  yield 2;
  yield 3;
}

const gen = generateSequence();
console.log(gen.next()); // { value: 1, done: false }
console.log(gen.next()); // { value: 2, done: false }
console.log(gen.next()); // { value: 3, done: false }
console.log(gen.next()); // { value: undefined, done: true }

```

Генераторы представляют специальный тип функций, который может приостанавливать и возобновлять свое выполнение. Они
возвращают объект-итератор, который позволяет пошагово получать значения.

*Подробнее:* [Генераторы](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Generator)

### **Продвинутая работа с функциями**

> Рекурсия – это термин в программировании, означающий вызов функцией самой себя. Рекурсивные функции могут быть
> использованы для элегантного решения определённых задач.
>

> Замыкание - это комбинация функции и лексического окружения, в котором она была определена. Это позволяет ей
> обращаться к переменным и функциям этого лексического окружения в дальнейшем.
>

*Подробнее:* [Продвинутая работа с функциями](https://learn.javascript.ru/advanced-functions)