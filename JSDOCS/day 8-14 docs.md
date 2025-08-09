# JavaScript Learning Notes – Day 8 to Day 14

## **Day 8: Advanced Arrays**
**Topics Covered:**
- forEach
- map
- filter
- reduce
- find & findIndex
- some & every
- sort
- Chaining methods

**Examples:**
```js
let numbers = [1, 2, 3, 4, 5];

// forEach
numbers.forEach(num => console.log(num));

// map
let doubled = numbers.map(num => num * 2);
console.log(doubled);

// filter
let evens = numbers.filter(num => num % 2 === 0);
console.log(evens);

// reduce
let sum = numbers.reduce((acc, curr) => acc + curr, 0);
console.log(sum);

// find
let firstEven = numbers.find(num => num % 2 === 0);
console.log(firstEven);

// some
console.log(numbers.some(num => num > 4)); // true

// every
console.log(numbers.every(num => num > 0)); // true

// sort
let sortedDesc = [...numbers].sort((a, b) => b - a);
console.log(sortedDesc);

// Chaining
let processed = numbers
  .filter(num => num % 2 !== 0)
  .map(num => num * 3)
  .reduce((a, b) => a + b, 0);
console.log(processed);
```

---

## **Day 9: Objects Deep Dive**
**Topics Covered:**
- Object creation
- Accessing properties
- Adding/updating/deleting properties
- Methods in objects
- `this` keyword
- Object destructuring
- Nested objects

**Examples:**
```js
let person = {
  name: "Alice",
  age: 25,
  greet: function() {
    console.log(`Hello, my name is ${this.name}`);
  },
  address: {
    city: "New York",
    zip: 10001
  }
};

// Access
console.log(person.name);
console.log(person["age"]);

// Update
person.age = 26;

// Add
person.job = "Developer";

// Delete
delete person.job;

// Method call
person.greet();

// Destructuring
let { name, age } = person;
console.log(name, age);

// Nested
console.log(person.address.city);
```

---

## **Day 10: DOM Manipulation**
**Topics Covered:**
- Selecting elements (`getElementById`, `querySelector`, etc.)
- Changing content
- Changing styles
- Creating and appending elements
- Removing elements

**Examples:**
```html
<div id="demo">Hello</div>
<script>
let element = document.getElementById("demo");
element.textContent = "Hello, JavaScript!";
element.style.color = "blue";

// Create element
let newDiv = document.createElement("div");
newDiv.textContent = "I am new here!";
document.body.appendChild(newDiv);

// Remove element
element.remove();
</script>
```

---

## **Day 11: Events & Event Listeners**
**Topics Covered:**
- Adding event listeners
- Event object
- Event bubbling
- Event delegation

**Examples:**
```html
<button id="btn">Click Me</button>
<ul id="list">
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<script>
document.getElementById("btn").addEventListener("click", function(event) {
  console.log("Button clicked!");
  console.log(event.type);
});

// Event delegation
document.getElementById("list").addEventListener("click", function(e) {
  if (e.target.tagName === "LI") {
    console.log("List item clicked:", e.target.textContent);
  }
});
</script>
```

---

## **Day 12: ES6+ Features**
**Topics Covered:**
- Template literals
- Spread and Rest operators
- Destructuring
- Default parameters
- ES6 modules (import/export)

**Examples:**
```js
// Template literals
let name = "John";
console.log(`Hello, ${name}!`);

// Spread
let arr1 = [1, 2, 3];
let arr2 = [...arr1, 4, 5];
console.log(arr2);

// Rest
function sum(...numbers) {
  return numbers.reduce((a, b) => a + b, 0);
}
console.log(sum(1, 2, 3));

// Destructuring
let user = { username: "alice", age: 22 };
let { username, age } = user;
console.log(username, age);

// Default parameter
function greet(msg = "Hi") {
  console.log(msg);
}
greet();
```

---

## **Day 13: Higher-Order Functions**
**Topics Covered:**
- Functions as arguments
- Functions returning functions
- Closures
- Practical use of higher-order functions

**Examples:**
```js
function greet(name) {
  return function(message) {
    console.log(`${message}, ${name}`);
  };
}

let greetJohn = greet("John");
greetJohn("Hello"); // Hello, John

// Callback
function processUserInput(callback) {
  let name = "Alice";
  callback(name);
}
processUserInput(function(name) {
  console.log("Hello " + name);
});
```

---

## **Day 14: Asynchronous JavaScript**
**Topics Covered:**
- setTimeout & setInterval
- Promises
- async/await
- Fetch API

**Examples:**
```js
// setTimeout
setTimeout(() => console.log("Hello after 2s"), 2000);

// setInterval
let counter = 0;
let interval = setInterval(() => {
  counter++;
  console.log(counter);
  if (counter === 5) clearInterval(interval);
}, 1000);

// Promise
let myPromise = new Promise((resolve, reject) => {
  let success = true;
  if (success) resolve("Done!");
  else reject("Error!");
});
myPromise.then(res => console.log(res)).catch(err => console.log(err));

// async/await with fetch
async function getData() {
  let response = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  let data = await response.json();
  console.log(data);
}
getData();
```
