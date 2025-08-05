
# JavaScript Learning: Day 1 to Day 5

Welcome to your JavaScript learning journey from **Zero to Hero**. This document covers detailed lessons from Day 1 to Day 5 along with quizzes and your submitted answers.

---

## 🟢 Day 1: Introduction to JavaScript

### ✅ Topics Covered:
- What is JavaScript?
- Why use JavaScript?
- Adding JS to HTML
- Using `console.log()`
- Writing and executing JS in the browser

### 🧠 Key Concepts:
- JavaScript is a client-side scripting language used to make web pages interactive.
- You can include JS in an HTML file using the `<script>` tag.
- The `console.log()` method prints output to the browser's console.

### 📝 Example:
```html
<script>
  console.log("Hello, JavaScript!");
</script>
```

---

### 📚 Quiz – Day 1:
1. What is JavaScript primarily used for?  
   a) Styling web pages  
   **b) Making web pages interactive** ✅  
   c) Structuring web content  
   d) Creating databases

2. How do you print something to the console in JS?  
   a) print()  
   **b) console.log()** ✅  
   c) log.console()  
   d) show()

3. Where do you usually see the output of `console.log()`?  
   a) On the web page  
   **b) In the browser's console** ✅  
   c) In the alert box  
   d) In the database

4. Which HTML tag is used to include JavaScript?  
   a) `<style>`  
   b) `<meta>`  
   **c) `<script>`** ✅  
   d) `<js>`

5. Which company developed JavaScript?  
   **a) Netscape** ✅  
   b) Microsoft  
   c) Sun Microsystems  
   d) Google

6. JavaScript is...  
   a) Server-side only  
   **b) Client-side mostly** ✅  
   c) Only used for mobile apps  
   d) A database language

---

## 🟢 Day 2: Variables & Data Types

### ✅ Topics Covered:
- Declaring variables: `var`, `let`, `const`
- Primitive data types: `string`, `number`, `boolean`, `undefined`, `null`

### 🧠 Key Concepts:
```js
let name = "John";
const age = 30;
var isOnline = true;
```

---

### 📚 Quiz – Day 2:
1. Which keyword allows block-level scope?  
   a) var  
   **b) let** ✅  
   c) const  
   d) block

2. What is the output of `typeof null`?  
   a) null  
   b) **object** ✅  
   c) undefined  
   d) string

3. Which of the following is a correct variable name?  
   **a) myName** ✅  
   b) 1name  
   c) my-name  
   d) var

4. `const` variables:  
   a) Can’t be reassigned ✅  
   b) Can be reassigned  
   c) Must be strings  
   d) Are global

5. Which of the following is a primitive data type?  
   **a) string** ✅  
   b) array  
   c) function  
   d) object

6. What is the result of `typeof undefined`?  
   a) null  
   **b) undefined** ✅  
   c) object  
   d) boolean

---

## 🟢 Day 3: Operators & Conditionals

### ✅ Topics Covered:
- Arithmetic operators (`+`, `-`, `*`, `/`, `%`)
- Comparison operators (`==`, `===`, `!=`, `<`, `>`, `<=`, `>=`)
- Logical operators (`&&`, `||`, `!`)
- If/else and switch statements

### 🧠 Key Example:
```js
if (score > 90) {
  console.log("Excellent!");
} else {
  console.log("Keep trying!");
}
```

---

### 📚 Quiz – Day 3:
1. What is the result of `5 + "5"`?  
   **a) "55"** ✅  
   b) 10  
   c) "10"  
   d) Error

2. `true && false` returns...?  
   a) true  
   **b) false** ✅  
   c) "truefalse"  
   d) undefined

3. Which operator checks **both value and type**?  
   a) **===** ✅  
   b) ==  
   c) !=  
   d) =

4. What is the result of `10 % 3`?  
   **a) 1** ✅  
   b) 3  
   c) 0  
   d) 10

5. What is the result of `!(true)`?  
   a) false ✅  
   b) true  
   c) undefined  
   d) Error

6. Which one is a comparison operator?  
   a) =  
   b) &&  
   **c) >=** ✅  
   d) !

---

## 🟢 Day 4: Strings & Template Literals

### ✅ Topics Covered:
- Declaring strings with `" "`, `' '`, and `` ` ` ``
- Template literals: `${expression}`
- Common string methods: `.length`, `.toUpperCase()`, `.toLowerCase()`, `.slice()`, `.replace()`, `.includes()`

### 🧠 Key Example:
```js
let name = "Alice";
console.log(`Hello, ${name}!`); // Template literal
```

---

### 📚 Quiz – Day 4:
1. What does `.length` return?  
   a) Last character  
   **b) Number of characters** ✅  
   c) Type of string  
   d) Uppercase version

2. How do you embed a variable in a template literal?  
   a) %var%  
   b) **${var}** ✅  
   c) (var)  
   d) @var

3. `let s = "hello".toUpperCase();` → `s` is:  
   a) hello  
   b) Hello  
   **c) HELLO** ✅  
   d) hELLO

4. What does `"abc".includes("b")` return?  
   a) false  
   **b) true** ✅  
   c) undefined  
   d) "b"

5. Which syntax uses template literals?  
   **d) \`Hello, ${name}\`** ✅

6. `let str = "JavaScript"; str.slice(4, 10)` → Result?  
   a) Java  
   **b) Script** ✅  
   c) cript  
   d) avaScript

---

## 🟢 Day 5: Loops – for, while, do…while

### ✅ Topics Covered:
- `for` loop, `while` loop, `do...while` loop
- Keywords: `break`, `continue`
- Looping through numbers

### 🧠 Example:
```js
for (let i = 1; i <= 5; i++) {
  if (i === 4) break;
  console.log(i);
}
```

---

### 📚 Quiz – Day 5:
1. Which loop is best when the number of iterations is known?  
   a) while  
   b) do...while  
   **c) for** ✅  
   d) loop

2. `while(true)` will run:  
   a) Once  
   **c) Forever unless stopped** ✅  
   b) Never  
   d) With an error

3. What does `continue` do?  
   **a) Skips to the next iteration** ✅  
   b) Exits loop  
   c) Ends program  
   d) Nothing

4. What is the output of this?
```js
let i = 0;
while (i < 3) {
  console.log(i);
  i++;
}
```  
   a) 1 2 3  
   **c) 0 1 2** ✅  
   b) 0 1 2 3  
   d) Error

5. What does this print?
```js
for (let i = 0; i < 3; i++) {
  console.log(i);
}
```  
   **c) 0 1 2** ✅

6. What is the output?
```js
for (let i = 1; i <= 5; i++) {
  if (i === 4) break;
  console.log(i);
}
```  
   a) 1 2 3 4 5  
   b) 1 2 3 4  
   **c) 1 2 3** ✅

---

## 🚀 Keep Going!
You’ve completed 5 days with perfect or near-perfect scores. The path ahead includes arrays, functions, objects, and DOM manipulation.

Next up: **Day 6 – Arrays in JavaScript** 🧺

Keep learning, keep building. You're doing amazing!
