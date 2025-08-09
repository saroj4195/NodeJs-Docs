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

Day 3: Booleans, Comparison & Logical Operators
✅ 1. Comparison Operators

These return a Boolean (true or false).
Operator	Meaning	Example	Result
==	Equal (loose)	5 == '5'	true
===	Equal (strict)	5 === '5'	false
!=	Not equal	5 != '5'	false
!==	Not equal (strict)	5 !== '5'	true
>	Greater than	10 > 5	true
<	Less than	3 < 1	false
>=	Greater than or equal	5 >= 5	true
<=	Less than or equal	4 <= 2	false

✅ 2. Logical Operators

Used to combine or negate conditions.
Operator	Name	Example	Result
&&	AND	true && false	false
`		`	OR
!	NOT	!true	false

let age = 20;
console.log(age >= 18); // true

let isAdult = age >= 18 && age < 60;
console.log(isAdult); // true

let isSenior = age >= 60 || age < 5;
console.log(isSenior); // false

console.log(!true); // false
console.log(!false); // true


4.Conditional Statements (if, else, else if, switch)

1. if Statement

Run a block of code if a condition is true.

let age = 18;

if (age >= 18) {
  console.log("You are an adult.");
}

let age = 16;

if (age >= 18) {
  console.log("You can vote.");
} else {
  console.log("You are too young to vote.");
}

 3. else if Chain

Test multiple conditions in order.

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

4. switch Statement

Used when you have many exact matches to test.

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

 5. Ternary Operator (shortcut for if...else)

let age = 20;
let message = age >= 18 ? "Adult" : "Minor";
console.log(message);


 Day 5: Loops – for, while, do...while, and loop control
 1. for Loop (most commonly used)

for (let i = 1; i <= 5; i++) {
  console.log("Count:", i);
}

✅ 2. while Loop

let i = 1;
while (i <= 5) {
  console.log("While count:", i);
  i++;
}

✅ 3. do...while Loop

let i = 1;
do {
  console.log("Do-While count:", i);
  i++;
} while (i <= 5);

✅ 4. Loop Control: break and continue
🔹 break: Exit the loop

for (let i = 1; i <= 10; i++) {
  if (i === 5) break;
  console.log(i);
}

 Day 6: Functions in JavaScript

✅ Example 1: Basic Function

function sayHello() {
  console.log("Hello, world!");
}

sayHello(); // Output: Hello, world!
