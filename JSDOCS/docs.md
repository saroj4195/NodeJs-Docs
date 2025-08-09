# JavaScript Basics

## Topic 1: Variables (Storing Values)

```javascript
let age = 25; // Can change later
const name = "Bhavik"; // Cannot change once set
var city = "Mumbai"; // Old way, avoid using
```

- **let**: Use when the value might change  
- **const**: Use when the value should not change  
- **var**: Outdated — avoid it (explained in Day 5)

---

## Topic 2: Data Types

✅ **Basic Types:**

| Type      | Example         |
|-----------|----------------|
| String    | `"Hello"`      |
| Number    | `123`, `3.14`  |
| Boolean   | `true`, `false`|
| Null      | `null`         |
| Undefined | `undefined`    |

```javascript
let name = "John";          // string
let age = 30;               // number
let isOnline = true;        // boolean
let score = null;           // null (intentional empty)
let level;                  // undefined
```

---

## Day 2: Strings and Numbers in JavaScript

### Part 1: Strings
A string is a sequence of characters inside quotes.

### Part 2: Numbers
Numbers in JavaScript can be integers or decimals.

```javascript
let x = 10;
let y = 3.5;
```

---

## Day 3: Booleans, Comparison & Logical Operators

✅ **1. Comparison Operators**

These return a Boolean (true or false).

| Operator | Meaning                 | Example     | Result |
|----------|------------------------|-------------|--------|
| ==       | Equal (loose)           | 5 == '5'    | true   |
| ===      | Equal (strict)          | 5 === '5'   | false  |
| !=       | Not equal               | 5 != '5'    | false  |
| !==      | Not equal (strict)      | 5 !== '5'   | true   |
| >        | Greater than            | 10 > 5      | true   |
| <        | Less than               | 3 < 1       | false  |
| >=       | Greater than or equal   | 5 >= 5      | true   |
| <=       | Less than or equal      | 4 <= 2      | false  |

✅ **2. Logical Operators**

| Operator | Name  | Example          | Result |
|----------|-------|------------------|--------|
| &&       | AND   | true && false    | false  |
| \|\|   | OR    | true \|\| false | true   |
| !        | NOT   | !true            | false  |

```javascript
let age = 20;
console.log(age >= 18); // true

let isAdult = age >= 18 && age < 60;
console.log(isAdult); // true

let isSenior = age >= 60 || age < 5;
console.log(isSenior); // false

console.log(!true); // false
console.log(!false); // true
```

---

## Conditional Statements

### 1. if Statement

```javascript
let age = 18;
if (age >= 18) {
  console.log("You are an adult.");
}
```

### 2. if...else Statement

```javascript
let age = 16;
if (age >= 18) {
  console.log("You can vote.");
} else {
  console.log("You are too young to vote.");
}
```

### 3. else if Chain

```javascript
let score = 85;
if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 75) {
  console.log("Grade: B");
} else if (score >= 60) {
  console.log("Grade: C");
} else {
  console.log("Grade: Fail");
}
```

### 4. switch Statement

```javascript
let day = "Tuesday";
switch (day) {
  case "Monday":
    console.log("Start of the week.");
    break;
  case "Tuesday":
    console.log("Second day.");
    break;
  case "Friday":
    console.log("Weekend is coming!");
    break;
  default:
    console.log("Some other day.");
}
```

### 5. Ternary Operator

```javascript
let age = 20;
let message = age >= 18 ? "Adult" : "Minor";
console.log(message);
```

---

## Day 5: Loops – for, while, do...while, and Loop Control

### 1. for Loop

```javascript
for (let i = 1; i <= 5; i++) {
  console.log("Count:", i);
}
```

### 2. while Loop

```javascript
let i = 1;
while (i <= 5) {
  console.log("While count:", i);
  i++;
}
```

### 3. do...while Loop

```javascript
let i = 1;
do {
  console.log("Do-While count:", i);
  i++;
} while (i <= 5);
```

### 4. Loop Control: break

```javascript
for (let i = 1; i <= 10; i++) {
  if (i === 5) break;
  console.log(i);
}
```

---

## Day 6: Functions in JavaScript

### Example 1: Basic Function

```javascript
function sayHello() {
  console.log("Hello, world!");
}
sayHello();
```

### Parameters vs Arguments

- **Parameters**: Variables listed in the function definition.
- **Arguments**: Values passed to the function when called.

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}
greet("Bhavik");
```

### Example 2: Function with Return Value

```javascript
function add(a, b) {
  return a + b;
}
let result = add(5, 3);
console.log(result);
```

### Function Expressions

```javascript
const multiply = function(x, y) {
  return x * y;
};
```

### Arrow Functions

```javascript
const square = (n) => n * n;
console.log(square(6));
```

---

## Day 7: JavaScript Scope & Variable Declarations

### 1. What is Scope?

Scope refers to the accessibility of variables.

| Type         | Description |
|--------------|-------------|
| Global Scope | Declared outside any function/block. Accessible anywhere. |
| Function Scope | Declared inside a function. Only accessible inside that function. |
| Block Scope | Declared inside {}. Only accessible inside that block (applies to let and const). |

### 2. var, let, and const

| Feature        | var            | let             | const           |
|----------------|---------------|----------------|----------------|
| Scope          | Function scoped | Block scoped   | Block scoped   |
| Re-declaration | Allowed       | ❌ Not allowed  | ❌ Not allowed  |
| Reassignment   | ✅ Allowed    | ✅ Allowed     | ❌ Not allowed  |
| Hoisted?       | ✅ Yes        | ✅ Yes (TDZ)   | ✅ Yes (TDZ)   |

### Examples

#### Global Scope

```javascript
var a = 10;
function printA() {
  console.log(a);
}
printA();
```

#### Function Scope

```javascript
function test() {
  var b = 20;
  console.log(b);
}
test();
```

#### Block Scope

```javascript
{
  let x = 100;
  const y = 200;
  console.log(x, y);
}
```

#### var is NOT block-scoped

```javascript
{
  var z = 300;
}
console.log(z);
```

#### const Must Be Initialized

```javascript
const age; // ❌ Error
```

#### Hoisting Example

```javascript
console.log(score); // undefined
var score = 50;

console.log(num); // ❌ ReferenceError
let num = 10;
```
