---

## Day 8 – Advanced Arrays

1. `.map()` returns:
   - a) Modified array
   - b) New array
   - c) Same array
   - d) Undefined

2. `.filter()` returns:
   - a) Single value
   - b) New array
   - c) Boolean
   - d) Null

3. Which method stops after finding the first match?
   - a) find()
   - b) filter()
   - c) map()
   - d) reduce()

4. `.some()` returns:
   - a) Boolean
   - b) Array
   - c) Index
   - d) Value

5. True/False: `.every()` checks if all elements meet a condition.

6. `Array.flat(2)` will:
   - a) Flatten one level
   - b) Flatten two levels
   - c) Flatten all levels
   - d) Throw error

7. `.reduce()` requires:
   - a) Initial value
   - b) Callback function
   - c) Both
   - d) None

8. `arr.includes(2)` checks:
   - a) Index
   - b) Presence of value
   - c) Type
   - d) Length

9. `.findIndex()` returns:
   - a) Boolean
   - b) Index
   - c) Value
   - d) Object

10. True/False: `.concat()` modifies the original array.

---

## Day 9 – Objects (Deep Dive)

11. Which creates a shallow copy?
    - a) Object.assign({}, obj)
    - b) Spread syntax `{...obj}`
    - c) Both
    - d) None

12. Object.keys({a:1,b:2}).length returns:
    - a) 1
    - b) 2
    - c) ['a','b']
    - d) Error

13. `Object.values()` returns:
    - a) Keys
    - b) Values
    - c) Entries
    - d) Error

14. True/False: `delete obj.key` removes a property.

15. Which checks property existence?
    - a) in
    - b) hasOwnProperty
    - c) Both
    - d) None

16. `Object.freeze()`:
    - a) Prevents adding/removing
    - b) Allows modification
    - c) Allows adding
    - d) None

17. True/False: `Object.seal()` prevents adding but allows value changes.

18. Which returns [key, value] pairs?
    - a) Object.entries()
    - b) Object.keys()
    - c) Object.values()
    - d) Object.pairs()

19. `{...obj1, ...obj2}`:
    - a) Merges objects
    - b) Copies object
    - c) Both
    - d) None

20. True/False: Object methods can be stored in variables.

---

## Day 10 – Functions (In-depth)

21. Arrow functions have:
    - a) Own this
    - b) Lexical this
    - c) Both
    - d) None

22. True/False: Function declarations are hoisted.

23. Which is valid?
    - a) function* gen() {}
    - b) func* gen() {}
    - c) generator gen() {}
    - d) None

24. IIFE syntax:
    - a) (function(){})();
    - b) function()(){};
    - c) (()function(){});
    - d) None

25. True/False: Default parameters must be at the start.

26. Higher-order function:
    - a) Accepts function
    - b) Returns function
    - c) Both
    - d) None

27. Rest parameter syntax:
    - a) ...
    - b) ***
    - c) &&
    - d) $$

28. True/False: Named functions can be recursive.

29. `arguments` is available in:
    - a) Regular functions
    - b) Arrow functions
    - c) Both
    - d) None

30. True/False: Anonymous functions must be stored in variables.

---

## Day 11 – Scope & Closures

31. Lexical scope means:
    - a) Runtime scope
    - b) Scope defined at creation
    - c) Dynamic scope
    - d) None

32. True/False: Closures can access global variables.

33. Which will cause ReferenceError?
    - a) Accessing let before declaration
    - b) Accessing var before declaration
    - c) Both
    - d) None

34. `var` scope is:
    - a) Block
    - b) Function
    - c) Global
    - d) Both function & global

35. True/False: const values cannot be reassigned.

36. Closures can:
    - a) Store state
    - b) Hide variables
    - c) Both
    - d) None

37. Temporal Dead Zone applies to:
    - a) let
    - b) const
    - c) Both
    - d) None

38. True/False: A closure is created every time a function is invoked.

39. Inner functions can access:
    - a) Outer variables
    - b) Inner variables
    - c) Global variables
    - d) All of the above

40. True/False: Variables in closures are garbage collected immediately after function returns.

---

## Day 12 – Array Iteration

41. `.forEach()` returns:
    - a) Array
    - b) Undefined
    - c) Boolean
    - d) Object

42. True/False: `for...of` iterates over array values.

43. Which iterates over keys?
    - a) for...in
    - b) for...of
    - c) Both
    - d) None

44. `.every()` stops when:
    - a) First false
    - b) First true
    - c) End of array
    - d) Never

45. True/False: `.map()` skips empty slots.

46. `.filter()` skips:
    - a) Undefined
    - b) Empty slots
    - c) Null
    - d) None

47. True/False: `.reduce()` executes callback for each element.

48. Which breaks early?
    - a) some()
    - b) every()
    - c) find()
    - d) All of the above

49. `.entries()` returns:
    - a) Index-value pairs
    - b) Values
    - c) Keys
    - d) None

50. True/False: `for...in` order is guaranteed.

---

## Day 13 – Higher-Order Functions

51. True/False: Higher-order functions can be anonymous.

52. `.map()` is:
    - a) Higher-order
    - b) Pure function
    - c) Both
    - d) None

53. `setTimeout` is:
    - a) Higher-order
    - b) Callback function
    - c) Both
    - d) None

54. True/False: A higher-order function must return a function.

55. `.filter()` is:
    - a) Pure
    - b) Higher-order
    - c) Both
    - d) None

56. True/False: Passing a function to another function makes it higher-order.

57. Array methods that are higher-order:
    - a) map
    - b) filter
    - c) reduce
    - d) All

58. `.sort()` is:
    - a) Pure
    - b) Impure
    - c) Both
    - d) None

59. True/False: Higher-order functions can modify global variables.

60. Which is a higher-order function?
    - a) forEach
    - b) every
    - c) some
    - d) All

---

## Day 14 – Objects (Advanced)

61. Object.create(null) creates:
    - a) Normal object
    - b) Object without prototype
    - c) Object with null values
    - d) None

62. True/False: Object.fromEntries() creates object from key-value pairs.

63. `Object.getOwnPropertyNames()` returns:
    - a) Enumerable only
    - b) All own properties
    - c) Prototype properties
    - d) None

64. Which prevents changes to property descriptors?
    - a) Object.freeze
    - b) Object.seal
    - c) Object.preventExtensions
    - d) None

65. True/False: Object.preventExtensions() stops adding new properties.

66. Object.is(NaN, NaN) returns:
    - a) true
    - b) false
    - c) Error
    - d) Undefined

67. True/False: Object.assign() performs deep copy.

68. Object.hasOwn(obj, 'prop') is:
    - a) ES2022 method
    - b) ES6 method
    - c) ES5 method
    - d) None

69. Which copies enumerable string-keyed properties?
    - a) Object.assign
    - b) Spread syntax
    - c) Both
    - d) None

70. True/False: Object.defineProperty() can make a property read-only.

---

## Mixed Review (Day 8–14)

71. True/False: Array.isArray([]) returns true.

72. Which checks array type without Array.isArray?
    - a) instanceof Array
    - b) typeof
    - c) isArrayType
    - d) None

73. True/False: `typeof null` is 'object'.

74. Which returns a shallow copy?
    - a) slice()
    - b) splice()
    - c) push()
    - d) pop()

75. True/False: Spread syntax works for both arrays and objects.

76. Which removes first element?
    - a) shift()
    - b) pop()
    - c) unshift()
    - d) splice()

77. True/False: `delete` can remove array elements.

78. Which is mutable?
    - a) Arrays
    - b) Objects
    - c) Both
    - d) None

79. True/False: `const` array elements can be changed.

80. Which merges arrays?
    - a) concat
    - b) spread
    - c) Both
    - d) None

---

## Extra Drill

81. True/False: Functions are objects in JavaScript.

82. Which returns function name?
    - a) func.name
    - b) name(func)
    - c) getName(func)
    - d) None

83. True/False: Closures can lead to memory leaks if not handled properly.

84. Which stops setInterval?
    - a) clearInterval
    - b) stopInterval
    - c) cancelInterval
    - d) None

85. True/False: typeof [] === 'object'.

86. Which method mutates array?
    - a) reverse
    - b) slice
    - c) map
    - d) filter

87. True/False: forEach can break early.

88. Which checks if all properties are enumerable?
    - a) propertyIsEnumerable
    - b) Object.enumerable
    - c) checkEnumerable
    - d) None

89. True/False: Spread syntax deep copies arrays.

90. Which is asynchronous?
    - a) setTimeout
    - b) forEach
    - c) map
    - d) filter

---

## Final Rapid Fire

91. True/False: NaN === NaN is false.

92. Which finds largest number?
    - a) Math.max
    - b) max()
    - c) Number.max
    - d) None

93. True/False: .includes() is case-sensitive.

94. Which creates new array length 10?
    - a) new Array(10)
    - b) Array(10).fill()
    - c) Both
    - d) None

95. True/False: Array indexes start at 1.

96. Which joins array into string?
    - a) join
    - b) concat
    - c) merge
    - d) toString

97. True/False: Object properties can have symbols as keys.

98. Which checks if object is frozen?
    - a) Object.isFrozen
    - b) isFrozen
    - c) checkFrozen
    - d) None

99. True/False: Array.flat(Infinity) fully flattens array.

100. Which converts object to JSON?
    - a) JSON.stringify
    - b) JSON.parse
    - c) toJSON
    - d) None
```
