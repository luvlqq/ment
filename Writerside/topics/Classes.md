# Classes

Классы в JavaScript представляют собой специальный тип объекта, который позволяет создавать объекты с определенными
свойствами и методами. Они используются для организации кода в более понятном и модульном стиле, особенно в
объектно-ориентированном программировании (ООП). Введение классов в стандарте ECMAScript 2015 (ES6) значительно
упростило и стандартизировало работу с объектами и наследованием в JavaScript.

### Определение класса

**Класс** определяется с использованием ключевого слова class, за которым следует имя класса и тело класса с его
свойствами и методами.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    return `Привет, меня зовут ${this.name} и мне ${this.age} лет.`;
  }
}

```

### Создание экземпляров класса

После определения класса можно создать его экземпляр с помощью оператора new.

```javascript
const person1 = new Person("Иван", 20);
console.log(person1.greet()); // Вывод: Привет, меня зовут Иван и мне 20 лет.

```

### Конструктор

**Конструктор** - это метод, который вызывается при создании нового экземпляра класса. В нем обычно устанавливаются
начальные значения свойств объекта.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }
}

```

### Методы класса

**Методы класса** - это функции, которые определены внутри тела класса и предназначены для выполнения определенных
действий с объектом.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    return `Привет, меня зовут ${this.name} и мне ${this.age} лет.`;
  }
}

```

### Наследование

```javascript
class Student extends Person {
  constructor(name, age, grade) {
    super(name, age);
    this.grade = grade;
  }

  study() {
    return `${this.name} учится в ${this.grade} классе.`;
  }
}

```

В примере выше класс Student наследует свойства и методы класса Person.

### Свойства и методы класса

Свойства и методы класса могут быть **публичными (public)**, **приватными (private)** или **защищенными (protected)**. В
JavaScript до версии ES6 не было официальной поддержки приватных свойств и методов. Однако с ES6 в классах JavaScript
появилась поддержка приватных членов класса с использованием символа # перед именем свойства или метода.

```javascript
class MyClass {
  #privateProperty = 10; // Приватное свойство

  constructor() {
    this.publicProperty = 20; // Публичное свойство
  }

  #privateMethod() {
    // Приватный метод
    return this.#privateProperty + this.publicProperty;
  }

  publicMethod() {
    // Публичный метод
    return this.#privateMethod();
  }
}

```

### Статические методы

Статические методы принадлежат самому классу, а не его экземплярам, и вызываются через сам класс, а не через его
экземпляры.

```javascript
class MathHelper {
  static add(a, b) {
    return a + b;
  }
}

console.log(MathHelper.add(5, 3)); // Вывод: 8

```

*Подробнее:* [Classes](https://learn.javascript.ru/classes)