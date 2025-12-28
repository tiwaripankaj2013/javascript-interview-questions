# JavaScript Interview Questions (Q1 - Q36)

| # | Question |
| :--- | :--- |
| 1 | [What is JavaScript?](#what-is-javascript) |
| 2 | [What are the different data types in JavaScript?](#what-are-the-different-data-types-in-javascript) |
| 3 | [What is the difference between `var`, `let`, and `const`?](#what-is-the-difference-between-var-let-and-const) |
| 4 | [Can you explicitly assign `undefined` to a variable?](#can-you-explicitly-assign-undefined-to-a-variable) |
| 5 | [What is hoisting in JavaScript?](#what-is-hoisting-in-javascript) |
| 6 | [What is the difference between `null` and `undefined`?](#what-is-the-difference-between-null-and-undefined) |
| 7 | [What is the use of `typeof` operator?](#what-is-the-use-of-typeof-operator) |
| 8 | [What is the difference between `==` and `===`?](#what-is-the-difference-between-and) |
| 9 | [What is a template literal?](#what-is-a-template-literal) |
| 10 | [What is NaN? What is its type?](#what-is-nan-what-is-its-type) |
| 11 | [What is an Immediately Invoked Function Expression (IIFE)?](#what-is-an-immediately-invoked-function-expression-iife) |
| 12 | [What is a closure in JavaScript?](#what-is-a-closure-in-javascript) |
| 13 | [What are the falsy values in JavaScript?](#what-are-the-falsy-values-in-javascript) |
| 14 | [What is the difference between Function Declaration and Function Expression?](#what-is-the-difference-between-function-declaration-and-function-expression) |
| 15 | [What are Arrow Functions?](#what-are-arrow-functions) |
| 16 | [What is the 'this' keyword?](#what-is-the-this-keyword) |
| 17 | [What is the difference between global scope and local scope?](#what-is-the-difference-between-global-scope-and-local-scope) |
| 18 | [What is a Higher-Order Function?](#what-is-a-higher-order-function) |
| 19 | [What is a Callback function?](#what-is-a-callback-function) |
| 20 | [How do you create an object in JavaScript?](#how-do-you-create-an-object-in-javascript) |
| 21 | [How do you access object properties?](#how-do-you-access-object-properties) |
| 22 | [What is the output of `2 + "2"`?](#what-is-the-output-of-2--2) |
| 23 | [What is the output of `2 - "2"`?](#what-is-the-output-of-2---2) |
| 24 | [What is strict mode in JavaScript?](#what-is-strict-mode-in-javascript) |
| 25 | [What is the Ternary Operator?](#what-is-the-ternary-operator) |
| 26 | [What is Destructuring assignment?](#what-is-destructuring-assignment) |
| 27 | [What is the Spread Operator?](#what-is-the-spread-operator) |
| 28 | [What is the Rest Parameter?](#what-is-the-rest-parameter) |
| 29 | [What is the DOM?](#what-is-the-dom) |
| 30 | [How do you select an element by ID?](#how-do-you-select-an-element-by-id) |
| 31 | [What is Event Bubbling?](#what-is-event-bubbling) |
| 32 | [What is the difference between `alert`, `prompt`, and `confirm`?](#what-is-the-difference-between-alert-prompt-and-confirm) |
| 33 | [What is JSON?](#what-is-json) |
| 34 | [How do you convert a JSON string to an Object?](#how-do-you-convert-a-json-string-to-an-object) |
| 35 | [How do you convert an Object to a JSON string?](#how-do-you-convert-an-object-to-a-json-string) |
| 36 | [What is a Promise?](#what-is-a-promise) |

---

1. ### What is JavaScript?
    JavaScript is a high-level, interpreted programming language primarily used to create interactive effects within web browsers. It is loosely typed and supports event-driven, functional, and imperative programming styles.

---

2. ### What are the different data types in JavaScript?
    JavaScript has Primitive types and Reference types.
    * **Primitive:** String, Number, Boolean, Null, Undefined, Symbol, BigInt.
    * **Reference:** Object (Arrays, Functions, Dates, etc.).

---

3. ### What is the difference between `var`, `let`, and `const`?
    * `var`: Function scoped, can be redeclared, hoisted with `undefined`.
    * `let`: Block scoped, cannot be redeclared in the same scope, hoisted but in a "temporal dead zone".
    * `const`: Block scoped, cannot be reassigned, must be initialized at declaration.

---

4. ### Can you explicitly assign `undefined` to a variable?
    Yes, but it is **not recommended**. It is better to use `null` to indicate an empty or unknown value.
    ```javascript
    let i = undefined;
    console.log(i); // undefined
    ```

---

5. ### What is hoisting in JavaScript?
    Hoisting is the behavior where variable and function declarations are moved to the top of their scope during the compilation phase.
    ```javascript
    console.log(a); // undefined (var is hoisted)
    var a = 10;
    ```

---

6. ### What is the difference between `null` and `undefined`?
    * `undefined`: A variable has been declared but not assigned a value.
    * `null`: An assignment value that represents "no value" or "nothing".

---

7. ### What is the use of `typeof` operator?
    It returns a string indicating the type of the unevaluated operand.
    ```javascript
    typeof "John" // "string"
    typeof 3.14   // "number"
    typeof null   // "object" (known bug in JS)
    ```

---

8. ### What is the difference between `==` and `===`?
    * `==` (Loose Equality): Converts types before comparing (coercion).
    * `===` (Strict Equality): Compares both value and type without coercion.

---

9. ### What is a template literal?
    Template literals use backticks (`` ` ``) and allow for embedded expressions and multi-line strings.
    ```javascript
    let name = "John";
    console.log(`Hello ${name}`);
    ```

---

10. ### What is NaN? What is its type?
    `NaN` stands for "Not-a-Number". It is a result of an invalid mathematical operation (e.g., `5 * "A"`). Surprisingly, `typeof NaN` is `"number"`.

---

11. ### What is an Immediately Invoked Function Expression (IIFE)?
    A function that is executed immediately after it is created.
    ```javascript
    (function() {
        console.log("I run immediately!");
    })();
    ```

---

12. ### What is a closure in JavaScript?
    A closure is a function that remembers its outer variables and can access them even when the function is executed outside its original scope.

---

13. ### What are the falsy values in JavaScript?
    Values that evaluate to `false` in a boolean context: `0`, `""` (empty string), `null`, `undefined`, `NaN`, and `false` itself.

---

14. ### What is the difference between Function Declaration and Function Expression?
    * **Declaration:** Hoisted, can be called before definition.
        `function foo() {}`
    * **Expression:** Not hoisted, created when execution reaches the line.
        `const foo = function() {}`

---

15. ### What are Arrow Functions?
    A concise syntax for writing function expressions. They do not have their own `this` or `arguments` binding.
    ```javascript
    const add = (a, b) => a + b;
    ```

---

16. ### What is the 'this' keyword?
    `this` refers to the object that is executing the current function. Its value depends on how the function is called (method call, standalone, constructor, etc.).

---

17. ### What is the difference between global scope and local scope?
    * **Global Scope:** Variables declared outside any function; accessible anywhere.
    * **Local Scope:** Variables declared inside a function or block; accessible only there.

---

18. ### What is a Higher-Order Function?
    A function that takes another function as an argument OR returns a function. (e.g., `map`, `filter`, `reduce`).

---

19. ### What is a Callback function?
    A function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.

---

20. ### How do you create an object in JavaScript?
    1.  Object Literal: `let obj = {};`
    2.  `new` keyword: `let obj = new Object();`
    3.  Constructor Function.
    4.  `Object.create()`.

---

21. ### How do you access object properties?
    * Dot notation: `obj.name`
    * Bracket notation: `obj["name"]` (useful for dynamic keys).

---

22. ### What is the output of `2 + "2"`?
    `"22"` (String concatenation).

---

23. ### What is the output of `2 - "2"`?
    `0` (String "2" is coerced to number).

---

24. ### What is strict mode in JavaScript?
    Enabled via `"use strict";`. It enforces stricter parsing and error handling (e.g., you cannot use undeclared variables).

---

25. ### What is the Ternary Operator?
    A shorthand for `if-else`. Syntax: `condition ? exprIfTrue : exprIfFalse`.

---

26. ### What is Destructuring assignment?
    A syntax that allows unpacking values from arrays or properties from objects into distinct variables.
    ```javascript
    let [x, y] = [1, 2];
    let {name} = {name: "John", age: 30};
    ```

---

27. ### What is the Spread Operator?
    Represented by `...`. It expands an iterable (like an array) into individual elements.
    ```javascript
    let arr = [1, 2, 3];
    let newArr = [...arr, 4, 5];
    ```

---

28. ### What is the Rest Parameter?
    Also represented by `...`. It collects multiple elements into a single array (used in function arguments).
    ```javascript
    function sum(...args) { /* args is an array */ }
    ```

---

29. ### What is the DOM?
    The Document Object Model (DOM) is an interface that treats an HTML document as a tree structure, where each node is an object representing a part of the document.

---

30. ### How do you select an element by ID?
    `document.getElementById("myId");`

---

31. ### What is Event Bubbling?
    A concept where an event triggers on the deepest target element first and then bubbles up through its ancestors in the DOM tree.

---

32. ### What is the difference between `alert`, `prompt`, and `confirm`?
    * `alert()`: Shows a message with an OK button.
    * `confirm()`: Shows a message with OK and Cancel (returns true/false).
    * `prompt()`: Shows a message with a text input (returns string or null).

---

33. ### What is JSON?
    JavaScript Object Notation. It is a lightweight data-interchange format, easy for humans to read/write and machines to parse/generate.

---

34. ### How do you convert a JSON string to an Object?
    `JSON.parse(jsonString);`

---

35. ### How do you convert an Object to a JSON string?
    `JSON.stringify(object);`

---

36. ### What is a Promise?
    An object representing the eventual completion (or failure) of an asynchronous operation and its resulting value. It has three states: Pending, Fulfilled, Rejected.