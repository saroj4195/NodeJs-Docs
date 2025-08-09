````markdown
# JavaScript Learning Notes – Day 1 to Day 7

---

## **Day 1: Introduction to JavaScript**
**Topics Covered:**
- JavaScript is a scripting language for creating dynamic web content.
- Runs in the browser's JavaScript engine (e.g., V8 in Chrome).
- Can also run outside browsers using Node.js.
- Added to HTML using `<script>` tags.

**Example:**
```html
<!DOCTYPE html>
<html>
<body>
<h1>My First JavaScript</h1>
<script>
  console.log("Hello, JavaScript!");
</script>
</body>
</html>
````

---

## **Day 2: Variables and Data Types**

**Topics Covered:**

* Declaring variables:

  * `var` (old way)
  * `let` (block scoped, modern)
  * `const` (block scoped, constant)
* Primitive Data Types:

  * String
  * Number
  * Boolean
  * Null
  * Undefined

**Example:**

```js
let name = "John";     // String
const age = 25;        // Number
var isStudent = true;  // Boolean
let x = null;          // Null
let y;                 // Undefined
```

---

## **Day 3: Operators**

**Topics Covered:**

* Arithmetic: `+`, `-`, `*`, `/`, `%`
* Assignment: `=`, `+=`, `-=`, etc.
* Comparison: `==`, `===`, `!=`, `!==`, `<`, `>`, `<=`, `>=`
* Logical: `&&` (AND), `||` (OR), `!` (NOT)

**Example:**

```js
let a = 10, b = 5;
console.log(a + b); // 15
console.log(a > b); // true
console.log(a === 10 && b < 10); // true
```

---

## **Day 4: Conditional Statements**

**Topics Covered:**

* `if`, `else if`, `else`
* `switch` statement

**Example:**

```js
let age = 18;
if (age >= 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}

let day = 2;
switch(day) {
  case 1: console.log("Monday"); break;
  case 2: console.log("Tuesday"); break;
  default: console.log("Other day");
}
```

---

## **Day 5: Loops (Detailed)**

### 1. **For Loop**

Used when you know how many times you want to repeat something.

```js
for (let i = 0; i < 5; i++) {
  console.log("Iteration:", i);
}
```

### 2. **While Loop**

Runs while the condition is true.

```js
let count = 0;
while (count < 5) {
  console.log("Count:", count);
  count++;
}
```

### 3. **Do...While Loop**

Runs **at least once**, then checks the condition.

```js
let num = 0;
do {
  console.log("Number:", num);
  num++;
} while (num < 5);
```

### 4. **Break Statement**

Stops the loop early.

```js
for (let i = 1; i <= 10; i++) {
  if (i === 5) break;
  console.log(i);
}
```

### 5. **Continue Statement**

Skips the current iteration and moves to the next.

```js
for (let i = 1; i <= 5; i++) {
  if (i === 3) continue;
  console.log(i);
}
```

---

## **Day 6: Functions**

**Topics Covered:**

* Function Declaration
* Function Expression
* Arrow Functions
* Parameters and Return Values

**Example:**

```js
function greet(name) {
  return "Hello, " + name;
}
console.log(greet("Alice"));

const add = (x, y) => x + y;
console.log(add(5, 3));
```

---

## **Day 7: Arrays Basics**

**Topics Covered:**

* Creating arrays
* Accessing elements
* Adding/Removing elements
* Looping through arrays

**Example:**

```js
let fruits = ["Apple", "Banana", "Cherry"];
fruits.push("Mango"); // Add at end
fruits.pop();         // Remove last
fruits.unshift("Lemon"); // Add at start
fruits.shift();       // Remove first

for (let fruit of fruits) {
  console.log(fruit);
}

