___

# JavaScript Interview Questions (Q37 - Q50)

| # | Question |
| :--- | :--- |
| 37 | [How can you generate an error?](#how-can-you-generate-an-error) |
| 38 | [Can you generate SyntaxError or ReferenceError kind of errors?](#can-you-generate-syntaxerror-or-referenceerror-kind-of-errors) |
| 39 | [What is the purpose of the finally block?](#what-is-the-purpose-of-the-finally-block) |
| 40 | [How can you refer to the name or description of error?](#how-can-you-refer-to-the-name-or-description-of-error) |
| 41 | [Can we have finally without a catch block as well?](#can-we-have-finally-without-a-catch-block-as-well) |
| 42 | [What is the difference between for...in and for...of?](#what-is-the-difference-between-forin-and-forof) |
| 43 | [What will be the output of the below code? (Coercion)](#what-will-be-the-output-of-the-below-code-coercion) |
| 44 | [What will be the output of below statements? (Comparison)](#what-will-be-the-output-of-below-statements-comparison) |
| 45 | [What is the difference between push() and unshift() method?](#what-is-the-difference-between-push-and-unshift-method) |
| 46 | [What is the difference between pop() and shift()?](#what-is-the-difference-between-pop-and-shift) |
| 47 | [How can you insert an element at a given position?](#how-can-you-insert-an-element-at-a-given-position) |
| 48 | [How can you remove a specific element?](#how-can-you-remove-a-specific-element) |
| 49 | [What does splice() return?](#what-does-splice-return) |
| 50 | [If there is not element removed then what will splice() method return?](#if-there-is-not-element-removed-then-what-will-splice-method-return) |
| 51 | [What is the difference between find() and filter() method?](#what-is-the-difference-between-find-and-filter-method) |
| 52 | [If there is no value to return, what will findIndex() return?](#if-there-is-no-value-to-return-what-will-findindex-return) |
| 53 | [What is the difference between indexOf() and includes() method?](#what-is-the-difference-between-indexof-and-includes-method) |
| 54 | [How will you search multiple values in an array?](#how-will-you-search-multiple-values-in-an-array) |
| 55 | [What will be the output of this code?](#what-will-be-the-output-of-this-code) |
| 56 | [Find length of each element in a new array.](#find-length-of-each-element-in-a-new-array) |
| 57 | [Find the square root of every element and store it in new array.](#find-the-square-root-of-every-element-and-store-it-in-new-array) |
| 58 | [Get all product names (pNames) in a new array.](#get-all-product-names-pnames-in-a-new-array) |
| 59 | [How will you flatten an array?](#how-will-you-flatten-an-array) |
| 60 | [Get sum of a key field of an object literal.](#get-sum-of-a-key-field-of-an-object-literal) |
| 61 | [Find avg value of all elements of an array?](#find-avg-value-of-all-elements-of-an-array) |
| 62 | [Find the sum or product of all elements?](#find-the-sum-or-product-of-all-elements) |
| 63 | [What is the difference between reduce() and reduceRight()?](#what-is-the-difference-between-reduce-and-reduceright) |
| 63 | [What is the difference between reduce() and reduceRight()?](#what-is-the-difference-between-reduce-and-reduceright) |
| 64 | [What happens if an array has undefined while sorting?](#what-happens-if-an-array-has-undefined-while-sorting) |
| 65 | [How will you sort an object literal?](#how-will-you-sort-an-object-literal) |
| 66 | [How will you sort a numeric array?](#how-will-you-sort-a-numeric-array) |
| 67 | [Sort all values of array in descending order.](#sort-all-values-of-array-in-descending-order) |
| 68 | [What is the destructuring assignment?](#what-is-the-destructuring-assignment) |
| 69 | [Swap values using destructuring.](#swap-values-using-destructuring) |
| 70 | [What is the output of let [a,b,c] = [5,,7]?](#what-is-the-output-of-let-abc--57) |
| 71 | [How will you set a default value while destructuring an array?](#how-will-you-set-a-default-value-while-destructuring-an-array) |
| 72 | [Explain different ways of creating date/time object.](#explain-different-ways-of-creating-datetime-object) |
| 73 | [What is the output of new Date(2020,08,23)?](#what-is-the-output-of-new-date20200823) |
| 74 | [Explain various formats of ISO standard in JavaScript.](#explain-various-formats-of-iso-standard-in-javascript) |
| 75 | [Get Character month?](#get-character-month) |
| 76 | [Find the date before 50 days of the given date.](#find-the-date-before-50-days-of-the-given-date) |
| 77 | [What will be the output if you add 35 as date in Date() constructor?](#output-of-adding-35-as-date-in-date-constructor) |
| 78 | [Calculate the date difference in days?](#calculate-the-date-difference-in-days) |
| 79 | [How can you change hours or minutes in time?](#how-can-you-change-hours-or-minutes-in-time) |
| 80 | [Can you have dynamic keys with object literal?](#can-you-have-dynamic-keys-with-object-literal) |
| 81 | [How can you add read-only properties to an object?](#how-can-you-add-read-only-properties-to-an-object) |
| 82 | [What is property value shorthand with object literal?](#what-is-property-value-shorthand-with-object-literal) |
| 83 | [Reference vs Value: Output of obj1.a = "Second"?](#reference-vs-value-output-of-obj1a--second) |
| 84 | [How can we create a clone or separate copy of an object literal?](#how-can-we-create-a-clone-or-separate-copy-of-an-object-literal) |
| 85 | [Output of 'this' in a global function in the browser?](#output-of-this-in-a-global-function-in-the-browser) |
| 86 | [Context of 'this' inside an arrow function?](#context-of-this-inside-an-arrow-function) |
| 87 | [What is the difference between call, apply and bind()?](#what-is-the-difference-between-call-apply-and-bind) |
| 88 | [Can you assign value to “this” object with assignment operator?](#can-you-assign-value-to-this-object-with-assignment-operator) |
| 89 | [How can you create a class?](#how-can-you-create-a-class) |
| 90 | [When does constructor() called?](#when-does-constructor-called) |
| 91 | [Can we have dynamic property or method names in a class?](#can-we-have-dynamic-property-or-method-names-in-a-class) |
| 92 | [What is a class expression?](#what-is-a-class-expression) |
| 93 | [What are static members in a class?](#what-are-static-members-in-a-class) |
| 94 | [How can you call another static method from a class?](#how-can-you-call-another-static-method-from-a-class) |
| 95 | [How can you inherit a class?](#how-can-you-inherit-a-class) |
| 96 | [What is subclassing?](#what-is-subclassing) |
| 97 | [What is the purpose of super keyword?](#what-is-the-purpose-of-super-keyword) |
| 98 | [How will you override a method?](#how-will-you-override-a-method) |
| 99 | [How can you extend a built-in class?](#how-can-you-extend-a-built-in-class) |
| 100 | [Practical scenario of object literal destructuring?](#practical-scenario-of-object-literal-destructuring) |
| 101 | [Explain the output of const { a=90, b } = { };](#explain-the-output-of-const-a90-b---) |
| 102 | [What are the advantages of using Map over objects?](#what-are-the-advantages-of-using-map-over-objects) |
| 103 | [How will you iterate through Map?](#how-will-you-iterate-through-map) |
| 104 | [Can you assign key/values with map['key']=value?](#can-you-assign-keyvalues-with-mapkeyvalue) |
| 105 | [How can you convert simple objects to Map?](#how-can-you-convert-simple-objects-to-map) |
| 106 | [How can you convert a Map into simple objects?](#how-can-you-convert-a-map-into-simple-objects) |
| 107 | [How will you remove an item or all items from Map?](#how-will-you-remove-an-item-or-all-items-from-map) |
| 108 | [What is the difference between Map and Set?](#what-is-the-difference-between-map-and-set) |
| 109 | [How will you remove specific values from Set?](#how-will-you-remove-specific-values-from-set) |
| 110 | [What will entries() method with Set return?](#what-will-entries-method-with-set-return) |
| 111 | [Difference between Map and WeakMap?](#difference-between-map-and-weakmap) |
| 112 | [Difference between Set and WeakSet?](#difference-between-set-and-weakset) |
| 113 | [Difference between window and document?](#difference-between-window-and-document) |
| 114 | [What is DOM or DOM API?](#what-is-dom-or-dom-api) |
| 115 | [What is BOM (Browser Object Model)?](#what-is-bom-browser-object-model) |
| 116 | [Difference between DOM and BOM?](#difference-between-dom-and-bom) |
| 117 | [Which is the global object in browser?](#which-is-the-global-object-in-browser) |
| 118 | [Check innerWidth and innerHeight of window?](#check-innerwidth-and-innerheight-of-window) |
| 119 | [How to get hostname from address bar?](#how-to-get-hostname-from-address-bar) |
| 120 | [Difference between setTimeout() and setInterval()?](#difference-between-settimeout-and-setinterval) |
| 121 | [Why can't we write document.setTimeout()?](#why-cant-we-write-documentsettimeout) |
| 122 | [How can you stop a timer?](#how-can-you-stop-a-timer) |
| 123 | [How will you create a digital clock?](#how-will-you-create-a-digital-clock) |
| 124 | [What is the default propagation path?](#what-is-the-default-propagation-path) |
| 125 | [How can you stop the event propagation?](#how-can-you-stop-the-event-propagation) |
| 126 | [How can you change the default propagation path?](#how-can-you-change-the-default-propagation-path) |
| 127 | [Get the reference of element on which event is fired?](#get-the-reference-of-element-on-which-event-is-fired) |
| 128 | [Check the element type on which the event is triggered?](#check-the-element-type-on-which-the-event-is-triggered) |
| 129 | [What is a node in DOM tree? Types?](#what-is-a-node-in-dom-tree-types) |
| 130 | [Difference between childeNodes and children?](#difference-between-childenodes-and-children) |
| 131 | [Output of element.lastChild.nextSibling?](#output-of-elementlastchildnextsibling) |
| 132 | [Can you use element.getElementById()?](#can-you-use-elementgetelementbyid) |
| 133 | [Difference between querySelector() & querySelectorAll().](#difference-between-queryselector-queryselectorall) |
| 134 | [Explain syntax of addEventListener() method.](#explain-syntax-of-addeventlistener-method) |
| 135 | [Difference between clientX/Y and pageX/Y?](#difference-between-clientxy-and-pagexy) |
| 136 | [Difference between event.code and event.key?](#difference-between-eventcode-and-eventkey) |
| 137 | [Difference between onblur and onchange?](#difference-between-onblur-and-onchange) |
| 138 | [How to handle events for checkbox/radio buttons?](#how-to-handle-events-for-checkboxradio-buttons) |
| 139 | [How to stop cut, copy or paste events?](#how-to-stop-cut-copy-or-paste-events) |
---

37. ### How can you generate an error?
    You can throw an error manually using the `throw` statement. While you can throw simple strings or numbers, it is best practice to throw an instance of the `Error` object to maintain the stack trace.

    ```javascript
    throw new Error("Something went wrong"); 
    ```

---

38. ### Can you generate SyntaxError or ReferenceError kind of errors?
    Yes, JavaScript allows you to manually throw specific built-in error types to mimic standard engine errors.

    ```javascript
    throw new SyntaxError("Invalid syntax found");
    throw new ReferenceError("Variable not defined");
    ```

---

39. ### What is the purpose of the finally block?
    The `finally` block is used to execute code that must run regardless of whether an error occurred or not. It is typically used for cleanup operations, such as closing files, hiding loading spinners, or resetting variables.

    ```javascript
    try {
        // Code that might throw an error
    } catch (error) {
        // Handle error
    } finally {
        console.log("This always runs (cleanup)");
    }
    ```

---

40. ### How can you refer to the name or description of error?
    When an error is caught in a `catch` block, the error object typically has `name` (the type of error) and `message` (the description) properties.

    ```javascript
    try {
        throw new Error("Something bad happened");
    } catch (e) {
        console.log(e.name);    // "Error"
        console.log(e.message); // "Something bad happened"
    }
    ```

---

41. ### Can we have finally without a catch block as well?
    Yes, a `try...finally` block is valid JavaScript. If an error occurs in the `try` block, the script will eventually crash (unless caught by an outer scope), but the code in `finally` will still execute immediately before the crash/exit.

    ```javascript
    try {
        console.log("Executing...");
    } finally {
        console.log("Cleanup happens even without catch");
    }
    ```

---

42. ### What is the difference between for...in and for...of?
    * **`for...in`**: Iterates over the **keys** (property names or array indices).
    * **`for...of`**: Iterates over the **values** of an iterable (Arrays, Strings, etc.).

    ```javascript
    let arr = [10, 20, 30];

    // Returns indices: "0", "1", "2"
    for (let k in arr) console.log(k); 

    // Returns values: 10, 20, 30
    for (let v of arr) console.log(v); 
    ```

---

43. ### What will be the output of the below code? (Coercion)
    *(Standard Interview Example)*
    ```javascript
    console.log(1 + "2");
    console.log(1 - "2");
    ```
    **Output:**
    ```text
    "12"
    -1
    ```
    **Reason:** The `+` operator prefers string concatenation when one operand is a string. The `-` operator only works with numbers, so it coerces the string "2" into the number 2.

---

44. ### What will be the output of below statements? (Comparison)
    *(Standard Interview Example)*
    ```javascript
    console.log(3 > 2 > 1);
    ```
    **Output:**
    ```text
    false
    ```
    **Reason:** Evaluated left to right: `(3 > 2)` is `true`. The expression becomes `true > 1`. `true` is coerced to `1`, so `1 > 1` is `false`.

---

45. ### What is the difference between push() and unshift() method?
    * **`push()`**: Adds an element to the **end** of an array.
    * **`unshift()`**: Adds an element to the **beginning** of an array.

    ```javascript
    let arr = [2, 3];
    arr.push(4);    // [2, 3, 4]
    arr.unshift(1); // [1, 2, 3, 4]
    ```

---

46. ### What is the difference between pop() and shift()?
    * **`pop()`**: Removes an element from the **end** of an array.
    * **`shift()`**: Removes an element from the **beginning** of an array.

    ```javascript
    let arr = [1, 2, 3];
    arr.pop();   // Removes 3
    arr.shift(); // Removes 1
    ```

---

47. ### How can you insert an element at a given position?
    You use the `splice()` method. The syntax is `splice(index, 0, element)`. The `0` ensures no elements are deleted.

    ```javascript
    let arr = ["A", "C"];
    arr.splice(1, 0, "B"); // Insert "B" at index 1
    console.log(arr); // ["A", "B", "C"]
    ```

---

48. ### How can you remove a specific element?
    You use `splice()` with the delete count parameter. Syntax: `splice(index, count)`.

    ```javascript
    let arr = ["A", "B", "C"];
    arr.splice(1, 1); // Remove 1 element at index 1
    console.log(arr); // ["A", "C"]
    ```

---

49. ### What does splice() return?
    The `splice()` method returns an **array** containing the **deleted** elements. The original array is modified in place.

---

50. ### If there is not element removed then what will splice() method return?
    It will return an **empty array** `[]`.

    **Code:**
    ```javascript
    let arr = ["One", "Two", "Three", "Four", "Five"];
    console.log(arr.splice(2, 0, "New")); 
    ```
    **Output:**
    ```text
    []
    ```
    **Reason:** The second argument `0` tells JavaScript to delete zero items. Since nothing was deleted, the return value is `[]`. The array `arr` now contains "New" at index 2.
51. ### What is the difference between `find()` and `filter()` method?
    * `find()`: Returns the **value of the first element** that passes the test.
    * `filter()`: Returns a **new array** containing all elements that pass the test.

---

52. ### If there is no value to return, what will `findIndex()` return?
    It returns **-1**.

---

53. ### What is the difference between `indexOf()` and `includes()` method?
    * `indexOf()`: Returns the **first index** at which a given element can be found, or -1 if it is not present.
    * `includes()`: Returns a **boolean** (true/false) depending on whether the array contains the element.

---

54. ### How will you search multiple values in an array?
    You can use the `filter()` method in combination with `includes()`.
    ```javascript
    let result = arr.filter(item => [val1, val2].includes(item));
    ```

---

55. ### What will be the output of this code?
    ```javascript
    let arr = ["One","Two","Three","Four","Five"];
    console.log(arr.lastIndexOf("Abcd")); 
    ```
    **Answer:** `-1` (because "Abcd" is not in the array).

---

56. ### Find length of each element in a new array.
    ```javascript
    let arr = ["One", "Two", "Three"];
    let lengths = arr.map(word => word.length); 
    // [3, 3, 5]
    ```

---

57. ### Find the square root of every element and store it in new array.
    ```javascript
    let nums = [4, 9, 16];
    let roots = nums.map(Math.sqrt);
    ```

---

58. ### Get all product names (`pNames`) in a new array.
    ```javascript
    let products = [
        {pCode:1, pName:"Apple"},
        {pCode:2, pName:"Banana"},
        {pCode:3, pName:"Grapes"},
        {pCode:4, pName:"Oranges"}
    ];
    let names = products.map(p => p.pName);
    ```

---

59. ### How will you flatten an array?
    Use the `flat()` method.
    ```javascript
    let arr = [1, [2, 3], [4, 5]];
    let flatArr = arr.flat();
    ```

---

60. ### Get sum of a key field of an object literal
    ```javascript
    const employees = [
        {eNo:1001, salary:3000},
        {eNo:1002, salary:2200},
        {eNo:1003, salary:3400},
        {eNo:1004, salary:6000}
    ];
    const totalSalary = employees.reduce((acc, emp) => acc + emp.salary, 0);
    ```

---

61. ### Find avg value of all elements of an array?
    ```javascript
    let nums = [10, 20, 30];
    let avg = nums.reduce((a, b) => a + b) / nums.length;
    ```

---

62. ### Find the sum or product of all elements?
    ```javascript
    let sum = nums.reduce((a, b) => a + b, 0);
    let product = nums.reduce((a, b) => a * b, 1);
    ```

---

63. ### What is the difference between `reduce()` and `reduceRight()`?
    * `reduce()`: Executes the reducer function from **left-to-right**.
    * `reduceRight()`: Executes the reducer function from **right-to-left**.
---

64. ### What happens if an array has `undefined` while sorting?
    The `sort()` method always places `undefined` elements at the **end** of the array.
    ```javascript
    let arr = [1, undefined, 3, 2];
    arr.sort(); // [1, 2, 3, undefined]
    ```

---

65. ### How will you sort an object literal?
    You sort based on a specific property using a custom compare function.
    ```javascript
    products.sort((a, b) => a.pName.localeCompare(b.pName));
    ```

---

66. ### How will you sort a numeric array?
    Use a compare function, otherwise, it sorts as strings.
    ```javascript
    arr.sort((a, b) => a - b);
    ```

---

67. ### Sort all values of array in descending order.
    ```javascript
    arr.sort((a, b) => b - a);
    ```

---

68. ### What is the destructuring assignment?
    A syntax to unpack values from arrays or properties from objects into distinct variables.
    ```javascript
    let [x, y] = [10, 20];
    ```

---

69. ### Swap values using destructuring.
    ```javascript
    [a, b] = [b, a];
    ```

---

70. ### What is the output of `let [a,b,c] = [5,,7]`?
    **Output:** `5 undefined 7`.
    **Reason:** The empty slot in the array literal results in `undefined` being assigned to `b`.

---

71. ### How will you set a default value while destructuring an array?
    ```javascript
    let [a = 10, b = 20] = [5];
    console.log(a, b); // 5 20
    ```

---

72. ### Explain different ways of creating date/time object.
    1. `new Date()` (Current)
    2. `new Date(milliseconds)`
    3. `new Date(dateString)`
    4. `new Date(year, month, day, hours, minutes, seconds, ms)`

---

73. ### What is the output of `new Date(2020,08,23)`?
    **Output:** `Wed Sep 23 2020 ...`
    **Reason:** In JS, months are **0-indexed**. `08` represents September.

---

74. ### Explain various formats of ISO standard in JavaScript.
    * **Complete Date:** `YYYY-MM-DD` (e.g., "2025-12-28")
    * **Combined Date & Time:** `YYYY-MM-DDTHH:mm:ssZ`
    * **Year & Month:** `YYYY-MM`

---

75. ### Get Character month?
    Months are 0-indexed numbers (0-11). To get the name, use an array.
    ```javascript
    const months = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"];
    console.log(months[new Date().getMonth()]);
    ```

---

76. ### Find the date before 50 days of the given date.
    ```javascript
    let d = new Date();
    d.setDate(d.getDate() - 50);
    ```

---

77. ### What will be the output if you add 35 as date in Date() constructor?
    The date "overflows" into the next month. For example, `new Date(2025, 0, 35)` becomes February 4th, 2025.

---

78. ### Calculate the date difference in days?
    ```javascript
    const diff = Math.abs(date2 - date1);
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
    ```

---

79. ### How can you change hours or minutes in time?
    Use `.setHours()` or `.setMinutes()`.

---

80. ### Can you have dynamic keys with object literal?
    Yes, using Computed Property Names: `let obj = { [variable]: value };`.

---

81. ### How can you add read-only properties to an object?
    Using `Object.defineProperty` with `writable: false`.

---

82. ### What is property value shorthand with object literal?
    If the variable name matches the key: `let obj = { name };` instead of `name: name`.

---

83. ### Reference vs Value: Output of obj1.a = "Second"?
    **Output:** `Second`.
    **Reason:** Objects are reference types. `obj1` and `obj` point to the same memory address.

---

84. ### How can we create a clone or separate copy of an object literal?
    1. Spread: `{ ...obj }`
    2. Object.assign: `Object.assign({}, obj)`
    3. Deep clone: `JSON.parse(JSON.stringify(obj))`

---

85. ### Output of 'this' in a global function in the browser?
    `window` (global object). In "strict mode", it is `undefined`.

---

86. ### Context of 'this' inside an arrow function?
    Arrow functions do not have their own `this`. They inherit it from the parent lexical scope.

---

87. ### What is the difference between call, apply and bind()?
    * **call**: Invokes immediately, args passed individually.
    * **apply**: Invokes immediately, args passed as an array.
    * **bind**: Returns a new function with `this` locked; doesn't run immediately.

---

88. ### Can you assign value to “this” object with assignment operator?
    **No.** `this` is a keyword. `this = obj` throws a Syntax Error.

---

89. ### How can you create a class?
    ```javascript
    class User {
      constructor(name) { this.name = name; }
    }
    ```

---

90. ### When does constructor() called?
    Immediately when an instance is created using the `new` keyword.

---

91. ### Can we have dynamic property or method names in a class?
    Yes, using `[dynamicKey]() { ... }`.

---

92. ### What is a class expression?
    `const MyClass = class { ... };`

---

93. ### What are static members in a class?
    Members defined with `static` belong to the class itself, not the instances. Used for utility methods.

---

94. ### How can you call another static method from a class?
    Use `this.otherStaticMethod()` inside another static method, or `ClassName.methodName()`.

---

95. ### How can you inherit a class?
    Using the `extends` keyword.

---

96. ### What is subclassing?
    Creating a new class (subclass) based on an existing one (superclass) to inherit its properties.

---

97. ### What is the purpose of super keyword?
    To call the parent class's constructor or methods.

---

98. ### How will you override a method?
    Define a method with the same name in the child class.

---

99. ### How can you extend a built-in class?
    `class MyArray extends Array { ... }`.

---

100. ### Practical scenario of object literal destructuring?
    Unpacking property values from a function argument (e.g., a config object).

---

101. ### Explain the output of `const { a=90, b } = { };`
    **Output:** `a=90, b=undefined`. `a` takes the default value, `b` has no source value.

---

102. ### What are the advantages of using Map over objects?
    Keys can be any type (not just strings/symbols), insertion order is kept, and it has a `size` property.

---

103. ### How will you iterate through Map?
    Using `for...of` or `map.forEach()`.

---

104. ### Can you assign key/values with map['key']=value?
    **No.** This treats Map as a regular object and bypasses the Map logic. Use `map.set(key, value)`.

---

105. ### How can you convert simple objects to Map?
    `new Map(Object.entries(obj))`.

---

106. ### How can you convert a Map into simple objects?
    `Object.fromEntries(map)`.

---

107. ### How will you remove an item or all items from Map?
    `map.delete(key)` or `map.clear()`.

---

108. ### What is the difference between Map and Set?
    Map stores Key-Value pairs; Set stores unique values only.

---

109. ### How will you remove specific values from Set?
    `set.delete(value)`.

---

110. ### What will entries() method with Set return?
    An iterator of `[value, value]` pairs (to match Map's signature).

---

111. ### Difference between Map and WeakMap?
    WeakMap keys must be objects and are weakly held (garbage-collectable).

---

112. ### Difference between Set and WeakSet?
    WeakSet only stores objects and doesn't prevent garbage collection.

---

113. ### Difference between window and document?
    `window` is the browser tab/global context; `document` is the DOM tree of the page.

---

114. ### What is DOM or DOM API?
    An object-oriented representation of the web page which allows programs to change structure/style.

---

115. ### What is BOM (Browser Object Model)?
    Objects for interacting with the browser (navigator, screen, location, history).

---

116. ### Difference between DOM and BOM?
    DOM is the page content; BOM is everything outside the content (the browser shell).

---

117. ### Which is the global object in browser?
    `window`.

---

118. ### Check innerWidth and innerHeight of window?
    `window.innerWidth`, `window.innerHeight`.

---

119. ### How to get hostname from address bar?
    `window.location.hostname`.

---

120. ### Difference between setTimeout() and setInterval()?
    `setTimeout` runs once after a delay; `setInterval` runs repeatedly at fixed intervals.

---

121. ### Why can't we write document.setTimeout()?
    It is a global utility belonging to the `window` environment, not the document structure.

---

122. ### How can you stop a timer?
    `clearTimeout(id)` or `clearInterval(id)`.

---

123. ### How will you create a digital clock?
    Update the `innerHTML` of a div using `setInterval` every 1000ms.

---

124. ### What is the default propagation path?
    **Bubbling** (Target -> Parents -> Window).

---

125. ### How can you stop the event propagation?
    `event.stopPropagation()`.

---

126. ### How can you change the default propagation path?
    Set the `useCapture` flag to `true` in `addEventListener`.

---

127. ### Get the reference of element on which event is fired?
    `event.target`.

---

128. ### Check the element type on which the event is triggered?
    `event.target.tagName`.

---

129. ### What is a node in DOM tree? Types?
    Everything is a node: Element nodes, Text nodes, Comment nodes.

---

130. ### Difference between childeNodes and children?
    `childNodes` includes text/comments; `children` only includes HTML element tags.

---

131. ### Output of element.lastChild.nextSibling?
    `null` (The last child has no following sibling).

---

132. ### Can you use element.getElementById()?
    **No.** `getElementById` only exists on the `document` object.

---

133. ### Difference between querySelector() & querySelectorAll().
    `querySelector` returns the first match; `querySelectorAll` returns a NodeList of all matches.

---

134. ### Explain syntax of addEventListener() method.
    `element.addEventListener(event, function, useCapture)`.

---

135. ### Difference between clientX/Y and pageX/Y?
    `clientX/Y` is relative to the viewport; `pageX/Y` is relative to the whole document (includes scrolling).

---

136. ### Difference between event.code and event.key?
    `code` represents the physical key pressed (e.g., KeyZ); `key` represents the character produced (e.g., z).

---

137. ### Difference between onblur and onchange?
    `onblur` fires when focus is lost; `onchange` fires when focus is lost **and** the value has been modified.

---

138. ### How to handle events for checkbox/radio buttons?
    Use the `change` event and check the `element.checked` property.

---

139. ### How to stop cut, copy or paste events?
    `element.addEventListener('copy', e => e.preventDefault());`