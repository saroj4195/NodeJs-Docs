
````markdown
# JavaScript Learning Notes – Day 8 to Day 14  
*(Concepts + Examples, no quizzes)*

---

## **Day 8 – Advanced Arrays**

### 1. forEach()
- Executes a provided function once for each array element.
```javascript
const nums = [1, 2, 3];
nums.forEach(num => console.log(num * 2)); // 2, 4, 6
````

### 2. map()

* Returns a new array with the results of applying a function to each element.

```javascript
const doubled = nums.map(num => num * 2);
console.log(doubled); // [2, 4, 6]
```

### 3. filter()

* Returns a new array with only the elements that pass a test.

```javascript
const evens = nums.filter(num => num % 2 === 0);
console.log(evens); // [2]
```

### 4. reduce()

* Reduces an array to a single value.

```javascript
const sum = nums.reduce((total, num) => total + num, 0);
console.log(sum); // 6
```

### 5. find()

* Returns the first element that matches a condition.

```javascript
const found = nums.find(num => num > 1);
console.log(found); // 2
```

### 6. findIndex()

* Returns the index of the first element that matches a condition.

```javascript
const index = nums.findIndex(num => num > 1);
console.log(index); // 1
```

### 7. some()

* Returns `true` if at least one element matches a condition.

```javascript
console.log(nums.some(num => num > 2)); // true
```

### 8. every()

* Returns `true` if all elements match a condition.

```javascript
console.log(nums.every(num => num > 0)); // true
```

### 9. sort()

* Sorts the array in place.

```javascript
const arr = [4, 2, 1, 3];
arr.sort((a, b) => a - b);
console.log(arr); // [1, 2, 3, 4]
```

---

## **Day 9 – Objects (Deep Dive)**

### 1. Creating Objects

```javascript
const person = { name: 'Alice', age: 25 };
```

### 2. Accessing Properties

```javascript
console.log(person.name); // Alice
console.log(person['age']); // 25
```

### 3. Nested Objects

```javascript
const user = {
  name: 'John',
  address: { city: 'NY', zip: 10001 }
};
console.log(user.address.city); // NY
```

### 4. Adding & Deleting Properties

```javascript
user.email = 'john@example.com';
delete user.zip;
```

### 5. Object Methods & `this`

```javascript
const car = {
  brand: 'Toyota',
  start: function() {
    console.log(`${this.brand} started`);
  }
};
car.start(); // Toyota started
```

### 6. Destructuring

```javascript
const { name, age } = person;
console.log(name, age);
```

---

## **Day 10 – Functions (In-depth)**

### 1. Function Declaration

```javascript
function greet(name) {
  return `Hello, ${name}`;
}
```

### 2. Function Expression

```javascript
const greet2 = function(name) {
  return `Hello, ${name}`;
};
```

### 3. Arrow Functions

```javascript
const greet3 = name => `Hello, ${name}`;
```

### 4. Default Parameters

```javascript
function sum(a, b = 5) {
  return a + b;
}
```

### 5. Rest Parameters

```javascript
function addAll(...nums) {
  return nums.reduce((acc, num) => acc + num, 0);
}
```

### 6. Scope

* Local vs Global variables

```javascript
let globalVar = 'I am global';
function test() {
  let localVar = 'I am local';
}
```

---

## **Day 11 – Scope & Closures**

### 1. Scope Types

* **Global Scope**
* **Function Scope**
* **Block Scope**

### 2. Hoisting

```javascript
console.log(a); // undefined
var a = 5;
```

### 3. Closures

* A closure is a function that remembers variables from its outer scope.

```javascript
function outer() {
  let count = 0;
  return function inner() {
    count++;
    return count;
  }
}
const counter = outer();
console.log(counter()); // 1
console.log(counter()); // 2
```

---

## **Day 12 – Arrays Deep Dive / Iteration Methods**

### 1. Multi-dimensional Arrays

```javascript
const matrix = [
  [1, 2],
  [3, 4]
];
console.log(matrix[1][0]); // 3
```

### 2. Iterating Arrays

```javascript
for (let num of [1, 2, 3]) console.log(num);
[1, 2, 3].forEach(n => console.log(n));
```

### 3. Performance Note

* `for` loop is fastest, `forEach` is easier to read.

---

## **Day 13 – Higher-Order Functions**

### 1. Functions as Arguments

```javascript
function greetUser(name, formatter) {
  return formatter(name);
}
console.log(greetUser('John', name => `Hello, ${name}`));
```

### 2. Functions Returning Functions

```javascript
function multiplier(factor) {
  return num => num * factor;
}
const double = multiplier(2);
console.log(double(5)); // 10
```

### 3. Callback Functions

```javascript
setTimeout(() => console.log('Done!'), 1000);
```

---

## **Day 14 – JavaScript Objects (Advanced)**

### 1. Object.keys / Object.values / Object.entries

```javascript
const obj = { a: 1, b: 2 };
console.log(Object.keys(obj)); // ['a', 'b']
console.log(Object.values(obj)); // [1, 2]
console.log(Object.entries(obj)); // [['a', 1], ['b', 2]]
```

### 2. Merging Objects

```javascript
const obj1 = { a: 1 };
const obj2 = { b: 2 };
const merged = { ...obj1, ...obj2 };
```

### 3. Object.freeze / Object.seal

```javascript
const frozen = Object.freeze({ name: 'Bob' });
// frozen.name = 'Alice'; // won't work
```

### 4. Shallow vs Deep Copy

```javascript
// Shallow copy
const copy = { ...obj };
// Deep copy
const deepCopy = JSON.parse(JSON.stringify(obj));
```

---
