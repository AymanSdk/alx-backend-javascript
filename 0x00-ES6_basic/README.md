# ES6 Basics

![ES](https://angularjsbeginnerguide.files.wordpress.com/2021/06/learn-es6-basic-concept-every-js-developer-should-know-about-es6.jpg?w=1400)
ES6, also known as ECMAScript 2015, introduced several new features and syntax enhancements to JavaScript, making it more powerful and expressive. This README provides an overview of some of the fundamental ES6 features.

## Table of Contents

1. [let and const](#let-and-const)
2. [Arrow Functions](#arrow-functions)
3. [Template Literals](#template-literals)
4. [Destructuring Assignment](#destructuring-assignment)
5. [Spread and Rest Operators](#spread-and-rest-operators)
6. [Classes](#classes)
7. [Modules](#modules)

## let and const

ES6 introduced two new variable declaration keywords: `let` and `const`.

- `let` allows declaring block-scoped variables that can be reassigned.
- `const` allows declaring variables with constant values, which cannot be reassigned.

```javascript
let count = 10;
const pi = 3.14;
```

## Arrow Functions

Arrow functions provide a more concise syntax for writing anonymous functions. They automatically bind to the scope in which they are defined.

```javascript
const add = (a, b) => a + b;
```

## Template Literals

Template literals allow embedding expressions inside strings using backticks (\`).

```javascript
const name = 'John';
console.log(`Hello, ${name}!`);
```

## Destructuring Assignment

Destructuring assignment allows unpacking values from arrays or objects into distinct variables.

```javascript
const [x, y] = [1, 2];
const { name, age } = { name: 'Alice', age: 30 };
```

## Spread and Rest Operators

The spread operator (`...`) allows expanding iterable objects into individual elements. The rest parameter syntax also uses `...` but is used in function parameters to collect arguments into an array.

```javascript
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5];

function sum(...numbers) {
  return numbers.reduce((acc, curr) => acc + curr, 0);
}
```

## Classes

ES6 introduced class syntax for defining constructor functions and inheritance, making object-oriented programming more intuitive.

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  sayHello() {
    console.log(`Hello, my name is ${this.name}!`);
  }
}
```

## Modules

ES6 modules provide a standardized way of organizing and importing/exporting code between files.

```javascript
// math.js
export const add = (a, b) => a + b;

// app.js
import { add } from './math.js';
console.log(add(2, 3)); // Output: 5
```

This README covers some of the basic ES6 features. However, ES6 introduced many more enhancements and syntactic sugar, empowering developers to write cleaner and more maintainable code. Familiarizing yourself with these features can significantly improve your JavaScript coding experience.
