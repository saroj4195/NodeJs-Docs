
# JavaScript Zero to Hero - Days 1 to 5

Welcome to your journey of mastering JavaScript from zero to hero! This document covers detailed explanations of all topics from Day 1 to Day 5.

---

## ✅ Day 1: Introduction to JavaScript

### 📌 What is JavaScript?
JavaScript is a powerful programming language used to make web pages interactive. It can update and change both HTML and CSS, calculate, manipulate, and validate data.

### 📚 Key Concepts
- **Variables**: Containers for storing data values.
- **Data Types**: `String`, `Number`, `Boolean`, `undefined`, `null`, `object`.
- **Console.log()**: Used to print output in the browser console.

### 🔤 Example:
```js
let name = "John";
console.log(name); // John
```

---

## ✅ Day 2: Variables and Data Types

### 📌 Variable Declarations
- `var`: Function-scoped (older usage)
- `let`: Block-scoped, preferred in modern JS
- `const`: Block-scoped, read-only after initialization

### 📚 Data Types
- **String**: `"Hello"`
- **Number**: `123`, `3.14`
- **Boolean**: `true`, `false`
- **undefined**: a variable declared but not assigned
- **null**: intentional absence of value

### 🔤 Examples:
```js
let age = 30;              // Number
const name = "Alice";      // String
var isStudent = true;      // Boolean
let address;               // undefined
let nothing = null;        // null
```

---

## ✅ Day 3: Operators and Expressions

### 📌 Types of Operators
- **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
- **Assignment Operators**: `=`, `+=`, `-=`, etc.
- **Comparison Operators**: `==`, `===`, `!=`, `>`, `<`
- **Logical Operators**: `&&`, `||`, `!`

### 🔤 Examples:
```js
let a = 10;
let b = 5;
console.log(a + b);      // 15
console.log(a > b);      // true
console.log(true && false); // false
```

---

## ✅ Day 4: Conditional Statements

### 📌 If-Else Statements
Used to execute different code blocks based on conditions.

```js
let age = 18;
if (age >= 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}
```

### 📌 Else If Ladder
```js
let score = 85;
if (score >= 90) {
  console.log("A");
} else if (score >= 80) {
  console.log("B");
} else {
  console.log("C");
}
```

### 📌 Ternary Operator
```js
let isMember = true;
let fee = isMember ? 10 : 20;
console.log(fee); // 10
```

---

## ✅ Day 5: Loops (Iteration)

### 📌 For Loop
```js
for (let i = 0; i < 3; i++) {
  console.log(i);
}
```

### 📌 While Loop
```js
let i = 0;
while (i < 3) {
  console.log(i);
  i++;
}
```

### 📌 Do...While Loop
```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 3);
```

### 📌 Break and Continue
- `break`: Exits the loop completely
- `continue`: Skips current iteration

```js
for (let i = 1; i <= 5; i++) {
  if (i === 3) continue;
  console.log(i); // skips 3
}
```

---

🎉 Keep going! You've already built a solid foundation in JavaScript!
Next up is **Day 6: Functions**.
