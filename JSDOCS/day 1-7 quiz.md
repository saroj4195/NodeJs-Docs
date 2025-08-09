
# JavaScript Quiz – Day 1 to Day 7 (50 Questions)


## **Day 1: Introduction to JavaScript**
1. JavaScript is primarily used for:
   - a) Database management  
   - b) Styling web pages  
   - c) Making web pages interactive  
   - d) Operating system development  

2. Where does JavaScript code usually run?
   - a) In the server only  
   - b) In the browser only  
   - c) In the browser or on a server (Node.js)  
   - d) In MS Word  

3. Which HTML tag is used to include JavaScript?
   - a) `<java>`  
   - b) `<script>`  
   - c) `<javascript>`  
   - d) `<code>`

4. Who invented JavaScript?
   - a) Tim Berners-Lee  
   - b) Brendan Eich  
   - c) Bill Gates  
   - d) Mark Zuckerberg  

5. JavaScript is:
   - a) Compiled language  
   - b) Interpreted language  
   - c) Both compiled and interpreted  
   - d) None of these  

---

## **Day 2: Variables & Data Types**
6. Which keyword is block-scoped in JavaScript?
   - a) var  
   - b) let  
   - c) const  
   - d) Both b and c  

7. Which data type is NOT primitive in JavaScript?
   - a) String  
   - b) Number  
   - c) Object  
   - d) Boolean  

8. What will `typeof null` return?
   - a) "null"  
   - b) "object"  
   - c) "undefined"  
   - d) "string"  

9. Which is the correct way to declare a constant?
   - a) var PI = 3.14;  
   - b) const PI = 3.14;  
   - c) let PI = 3.14;  
   - d) fixed PI = 3.14;  

10. What is the default value of an uninitialized variable?
    - a) null  
    - b) 0  
    - c) undefined  
    - d) NaN  

---

## **Day 3: Operators**
11. Which operator checks both value and type?
    - a) ==  
    - b) !=  
    - c) ===  
    - d) >=  

12. What will `5 + "5"` return?
    - a) 10  
    - b) "55"  
    - c) 55  
    - d) NaN  

13. Which of the following is NOT a logical operator?
    - a) &&  
    - b) ||  
    - c) !==  
    - d) !  

14. What is the result of `10 % 3`?
    - a) 3  
    - b) 1  
    - c) 0  
    - d) 0.3  

15. What will `"5" == 5` return?
    - a) true  
    - b) false  
    - c) NaN  
    - d) Error  

---

## **Day 4: Conditionals**
16. What keyword starts a conditional block?
    - a) for  
    - b) if  
    - c) while  
    - d) switch  

17. Which statement allows multiple choice branches?
    - a) if...else  
    - b) loop  
    - c) switch  
    - d) case  

18. In `if (false) { console.log("Hi"); }`, what happens?
    - a) Prints "Hi"  
    - b) Nothing happens  
    - c) Throws an error  
    - d) Prints false  

19. In `switch` statement, what keyword exits the case?
    - a) break  
    - b) continue  
    - c) exit  
    - d) stop  

20. What will this output?
```js
let x = 10;
if (x > 5) {
  console.log("Big");
} else {
  console.log("Small");
}
````

* a) Big
* b) Small
* c) Error
* d) undefined

---

## **Day 5: Loops**

21. Which loop runs at least once?

    * a) for
    * b) while
    * c) do...while
    * d) repeat

22. What will this output?

```js
for (let i = 0; i < 3; i++) {
  console.log(i);
}
```

* a) 0 1 2
* b) 1 2 3
* c) 0 1 2 3
* d) 3 2 1

23. What does `break` do in a loop?

    * a) Skips iteration
    * b) Stops the loop completely
    * c) Restarts loop
    * d) None of the above

24. What does `continue` do?

    * a) Skips current iteration
    * b) Stops loop completely
    * c) Restarts loop
    * d) Exits function

25. Which loop is best when the number of iterations is unknown?

    * a) for
    * b) while
    * c) do...while
    * d) repeat

---

## **Day 6: Functions**

26. How do you declare a function?

    * a) function myFunc() {}
    * b) def myFunc() {}
    * c) func myFunc() {}
    * d) function\:myFunc() {}

27. What will this output?

```js
function sum(a, b) {
  return a + b;
}
console.log(sum(2, 3));
```

* a) 23
* b) 5
* c) undefined
* d) Error

28. Which is the arrow function?

    * a) function() {}
    * b) () => {}
    * c) => {}
    * d) function => {}

29. If a function does not return anything, it returns:

    * a) null
    * b) undefined
    * c) 0
    * d) NaN

30. Which scope is created when a function is called?

    * a) Global
    * b) Local
    * c) Block
    * d) Static

---

## **Day 7: Arrays Basics**

31. How do you create an array?

    * a) let arr = \[];
    * b) let arr = {};
    * c) let arr = ();
    * d) let arr = <>;

32. What will this output?

```js
let arr = [1, 2, 3];
console.log(arr[1]);
```

* a) 1
* b) 2
* c) 3
* d) undefined

33. Which method adds an element at the end?

    * a) shift()
    * b) unshift()
    * c) push()
    * d) pop()

34. Which method removes the last element?

    * a) shift()
    * b) pop()
    * c) remove()
    * d) splice()

35. Which loop works best for iterating arrays?

    * a) for...of
    * b) while
    * c) switch
    * d) do...while

36. What will this output?

```js
let fruits = ["Apple", "Banana"];
fruits.push("Mango");
console.log(fruits.length);
```

* a) 2
* b) 3
* c) 4
* d) undefined

37. What does `shift()` do?

    * a) Removes first element
    * b) Adds first element
    * c) Removes last element
    * d) Adds last element

38. What does `unshift("Lemon")` do?

    * a) Adds "Lemon" to start
    * b) Adds "Lemon" to end
    * c) Removes "Lemon"
    * d) Replaces first element

39. What will this output?

```js
let nums = [1, 2, 3];
console.log(nums.includes(2));
```

* a) true
* b) false
* c) undefined
* d) Error

40. Which method joins array elements into a string?

    * a) concat()
    * b) join()
    * c) toString()
    * d) stringify()

---

## **Mixed Practice**

41. What is `typeof []`?

    * a) "array"
    * b) "object"
    * c) "list"
    * d) "undefined"

42. Which operator is used to assign a value?

    * a) =
    * b) ==
    * c) ===
    * d) :=

43. What will `"5" + 2` return?

    * a) "52"
    * b) 7
    * c) NaN
    * d) Error

44. Which method can remove elements from an array by index?

    * a) slice()
    * b) splice()
    * c) pop()
    * d) shift()

45. Which method combines two arrays?

    * a) merge()
    * b) concat()
    * c) join()
    * d) push()

46. Which loop can be infinite if condition is always true?

    * a) for
    * b) while
    * c) do...while
    * d) All of these

47. Which keyword is used for constants?

    * a) var
    * b) const
    * c) let
    * d) static

48. Which statement ends function execution?

    * a) break
    * b) exit
    * c) return
    * d) stop

49. How do you check if variable `x` is an array?

    * a) typeof x === 'array'
    * b) Array.isArray(x)
    * c) x instanceof Array
    * d) Both b and c

50. What does `NaN` mean?

    * a) Not a Number
    * b) New array number
    * c) Null and Null
    * d) None and None

---
