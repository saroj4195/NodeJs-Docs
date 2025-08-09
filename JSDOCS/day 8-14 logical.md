# 100 Practical JavaScript Challenges — Day 8 → Day 14

## Day 8 — Advanced Arrays (1–15)
1. Use `.map()` to create a new array where each number is doubled.
2. Use `.filter()` to return only odd numbers from an array.
3. Use `.reduce()` to compute the product of all numbers in an array.
4. Use `.find()` to get the first number greater than 50.
5. Use `.findIndex()` to locate the first negative number’s index.
6. Use `.some()` to check if any element in an array is `0`.
7. Use `.every()` to confirm all elements are strings in an array.
8. Sort an array of numbers ascending using a compare callback.
9. Create a new array with each element squared, using `.map()` chained after `.filter()` to only include positive numbers.
10. Remove duplicates from an array (return a new array with unique values).
11. Merge two arrays and sort the resulting array ascending.
12. Using `.reduce()`, count how many times each value appears in an array (return an object of counts).
13. Using `.reduce()`, flatten a two-level nested array (e.g. `[[1,2],[3,4]]` → `[1,2,3,4]`).
14. Using only array methods, return the top 3 largest numbers from an array.
15. Using `.map()` and `.filter()` together, transform an array of numbers into strings of even numbers only (e.g. `[1,2,3,4]` → `["2","4"]`).

## Day 9 — Objects Deep Dive (16–30)
16. Create an object `person` with `name`, `age`, `city`. Log all keys.
17. Add a method `greet()` to `person` that logs `"Hello, NAME"`.
18. Delete the `city` property from `person`.
19. Given an object, write a function that returns `true` if it has **no** own properties.
20. Given an object, produce an array of its `[key, value]` pairs **without** using `Object.entries()` (use a loop).
21. Write a function to shallow-clone an object (return new independent object at top level).
22. Merge two objects into a new object (later keys overwrite earlier ones).
23. Given a nested object, read a deeply nested value safely (check intermediate properties).
24. Write a function to rename a key in an object (keep value).
25. Convert an object of key→value into an array of values sorted by key name.
26. Count how many properties of an object have values that are strings.
27. Given an array of objects `{id, name}`, convert to a lookup object keyed by `id` (id → object).
28. Remove all properties from an object whose values are falsy (`0`, `""`, `null`, `undefined`, `false`, `NaN`).
29. Write a function that merges an array of objects into one object (later objects override earlier keys).
30. Implement a function that prints all nested keys of an object (depth-first traversal, keys only).

## Day 10 — Functions (In-depth) (31–45)
31. Write a function `add(a,b)` that returns a + b.
32. Write a function `isEven(n)` that returns true/false.
33. Write a function that returns the greater of two numbers without using `Math.max`.
34. Create a function accepting an array and returning the sum of elements.
35. Write a function `range(n)` that returns an array `[0,1,2,...,n-1]`.
36. Write a function that accepts two numbers and swaps them (return swapped pair).
37. Implement `power(base, exp)` using a loop (no `Math.pow`).
38. Make a function that checks whether a number is prime.
39. Create a function that returns factorial of `n` (iteratively).
40. Write a function that takes a function and an argument, invokes the function with that argument, and returns the result.
41. Write a function `once(fn)` that returns a wrapper which only allows `fn` to run once.
42. Build `memoize(fn)` for a pure one-argument function using a simple cache object.
43. Implement `compose(f, g)` that returns a function applying `g` then `f`.
44. Write a function that times execution of another function and returns the elapsed milliseconds.
45. Create `rangeSum(a,b)` that sums integers from `a` to `b` inclusive.

## Day 11 — Scope & Closures (46–60)
46. Demonstrate difference between function scope and block scope with `var` vs `let`. (Write code that shows `var` escaping a block.)
47. Show hoisting: access a `var` declared variable before declaration and explain output. (Code only.)
48. Show TDZ: access a `let` before initialization (produce error).
49. Build a counter closure `makeCounter()` that returns an object with `inc()` and `value()` methods.
50. Write a function that returns another function that remembers a greeting message (closure).
51. Implement a private variable inside a module-like function (IIFE pattern) and expose getter only.
52. Write code to demonstrate that closures capture variables by reference (mutating outer variable affects inner).
53. Create a function `createSecretHolder(secret)` that returns `{getSecret, setSecret}` for storing secret.
54. Build a function `limitCalls(fn, n)` that allows `fn` to be called at most `n` times.
55. Implement a function that returns an array of functions each printing its index (avoid the classic loop closure trap).
56. Build a function `bindContext(fn, ctx)` that returns a function invoking `fn` with `this` = `ctx`.
57. Write code proving that global variables are accessible inside functions (and their pitfalls).

## Day 12 — Arrays Deep Dive / Iteration Methods (58–72)
58. Iterate an array with a classic `for` loop and build a new array of values ×10.
59. Iterate an array with `for...of` and collect all string elements into a new array.
60. Implement `forEachManual(arr, fn)` using a `for` loop (recreate `forEach`).
61. Using `forEach`, sum numbers in an array.
62. Using `map`, transform an array of strings into lengths (string → length).
63. Using `filter`, remove all empty strings from an array.
64. Using `reduce`, convert `["a","b","c"]` to `"abc"`.
65. Using `reduce`, convert an array of `{id, score}` to object mapping id→score.
66. Using `reduce`, partition an array into two arrays: evens and odds.
67. Using `for` loops only, reverse an array into a new array.
68. Implement `arrayUnique(arr)` using iteration (no Set).
69. Write a function that rotates array right by `k` positions (using loops).
70. Implement `chunk(arr, size)` that splits array into chunks of given size.

## Day 13 — Higher-Order Functions & Functional Patterns (73–86)
71. Implement `applyToAll(arr, fn)` that returns array of `fn(item)` results.
72. Implement `filterBy(arr, predicate)` manually using basic loops (no built-in filter).
73. Compose two functions `f` and `g` (implement compose manually).
74. Implement `pipe(...fns)` that returns function applying each fn left→right.
75. Write `tap(value, fn)` that calls `fn(value)` and returns `value` (useful in chains).
76. Implement `curry2(fn)` that curries a 2-argument function into `fn(a)(b)`.
77. Write `once` (if not already) as a higher-order function wrapper.
78. Implement `retry(fn, times)` that attempts `fn` up to `times` if it throws.
79. Implement `memoize` for functions of one argument (improve earlier).
80. Create `negate(predicate)` that returns a predicate returning opposite boolean.
81. Implement `groupBy(arr, keyFn)` returning an object grouped by keyFn result.
82. Implement `pluck(arr, propName)` that extracts property values from object array, similar to `map(o => o[propName])`.
83. Create `limitRate(fn, ms)` that ensures `fn` runs at most once per `ms` ms (simple throttle).

## Day 14 — JavaScript Objects (Advanced) (87–100)
84. Using basic loops, clone an object shallowly (no Object.assign).
85. Implement `mergeObjectsDeep(target, source)` that shallowly copies only top-level keys (note difference from deep merge).
86. Using `Object.keys`, write a function that returns object size (number of own keys).
87. Implement `invertObject(obj)` that swaps keys and values (assume primitive values).
88. Write a function that removes properties from an object by given array of keys.
89. Using only loops, write `select(obj, keysArray)` returning new object with only those keys.
90. Write `omit(obj, keysArray)` returning object without those keys.
91. Implement `safeGet(obj, pathArray)` to retrieve nested property safely (return `undefined` if not present).
92. Implement `setNested(obj, pathArray, value)` to set nested value, creating intermediate objects as needed.
93. Implement `deepClone(obj)` using recursion (handle arrays and plain objects; avoid circular refs).
94. Write a function `isPlainObject(value)` that returns true if `value` is a plain object (not array, not null, not function).
95. Implement `mergeArrayObjects(arr, idKey)` that merges array of `{id, ...}` into object keyed by id (id → object).
96. Build `pickRandomKey(obj)` that returns a random property name from object.
97. Write `objectToQueryString(obj)` that converts `{a:1,b:2}` to `"a=1&b=2"` (URL-encoding optional).
98. Implement `mapObject(obj, fn)` that returns a new object where each value is `fn(value, key)`.
99. Create `deepFreeze(obj)` recursively freezing nested objects.
100. Implement `diffObjects(a,b)` returning keys that differ (list keys only present or with different primitive values).
