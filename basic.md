📘 JavaScript Basic Interview Questions
<!-- TOPIC_START -->
| No. | Questions |
| --- | --------- |
| 1 | [What is undefined in JavaScript?](#What-is-undefined-in-JavaScript) |
| 2 | [What will be the output of undefined == null and undefined === null?](#What-will-be-the-output-of-undefined-==-null-and undefined-===-null)|
| 3 | [Can you explicitly assign undefined to a variable?](#can-you-explicitly-assign-undefined-to-a-variable) |
| 4 | [Can you explicitly assign undefined to a variable?](#can-you-explicitly-assign-undefined-to-a-variable) |
| 5 | [What is hoisting in JavaScript?](#what-is-hoisting-in-javascript) |
| 6 | [How does block scope work?](#how-does-block-scope-work) |
| 7 | [What is the scope of a variable?](#what-is-the-scope-of-a-variable) |
| 8 | [Should you terminate all lines with semicolons?](#should-you-terminate-all-lines-with-semicolons) |
| 9 | [Why does this function return undefined despite returning an object?](#why-does-this-function-return-undefined-despite-returning-an-object) |
| 10 | [Can we use the arguments object in an arrow function?](#can-we-use-the-arguments-object-in-an-arrow-function) |
| 11 | [Which is the best way to create a new array with assignment?](#which-is-the-best-way-to-create-a-new-array-with-assignment) |
| 12 | [How can a function accept any number of parameters?](#how-can-a-function-accept-any-number-of-parameters) |
| 13 | [Can the rest operator be placed anywhere in parameters?](#can-the-rest-operator-be-placed-anywhere-in-parameters) |
| 14 | [How will you validate positive or negative Infinity?](#how-will-you-validate-positive-or-negative-infinity) |
| 15 | [What will be the output of NaN == NaN?](#what-will-be-the-output-of-nan--nan) |
| 16 | [What will be the output of the statement Output of console.log(NaN == NaN)](what-will-be-the-output-of-the) |
| 17 | [What is the difference between isNaN() and isFinite() method?](what-is-the-difference-between-isnan-and-isfinite-method) |
| 18 | [Explain the syntactical features of arrow function?.](explain-the-syntactical-features-of-arrow-function) |
| 19 | [Why this does not work in arrow function?](why-this-does-not-work-in-arrow-function) |
| 20 | [Explain output of following code with reason const obj={
     method:()=>{  console.log(this)}}](explain-output-of-following-code-with-reason) |

| 21 | [How can you handle arguments object like functionality in arrow function?](how-can-you-handle-arguments-object-like-functionality-in-arrow-function) | |
| 22 | [Can you write IIFE with arrow function syntax?](can-you-write-iife-with-arrow-function-syntax) | |
| 23 | [How can you access private variable or function outside the scope?](how-can-you-access-private-variable-or-function-outside-the-scope) | |
| 24 | [Explain the advantage of closure?](explain-the-advantage-of-closure) | |
| 25 | [What is function currying?](what-is-function-currying) | |
| 26 | [What will this statement do?](what-will-this-statement-do) | |
| 27 | [Explain practical usage of function currying.](explain-practical-usage-of-function-currying) | |
| 28 | [What is the purpose of the iterator?](what-is-the-purpose-of-the-iterator) | |
| 29 | [How do you create an iterator?](how-do-you-create-an-iterator) | |
| 30 | [Explain a practical use of an iterator?](explain-a-practical-use-of-an-iterator) | |
| 31 | [What are generator functions? Explain the syntax.](what-are-generator-functions-explain-the-syntax) | |
| 32 | [Which is the right syntax for generator function?](which-is-the-right-syntax-for-generator-function) | |
| 33 | [Explain all methods of generator objects.](explain-all-methods-of-generator-objects) | |
| 34 | [Explain the use of yield*.](explain-the-use-of-yield) | |
| 35 | [Can you prevent return() from terminating the generator?](can-you-prevent-return-from-terminating-the-generator) | |




---
1. ### What is `undefined` in JavaScript?
      `undefined` means a variable has been declared but not assigned any value.
    ```let a;
        console.log(a); // undefined
---       ```
2. ### What will be the output of `undefined` `==` `null` and `undefined` `===` `null`?
    ```console.log(undefined == null);  // true
    console.log(undefined === null); // false
       ```
       Explanation:
    == performs type coercion and treats both as empty values
    === checks both value and type, which are different
---
3. ### Can you explicitly assign `undefined` to a `variable`
    `let i = undefined
    Yes, but not recommended.
    let i = undefined;
    console.log(i); // undefined
---

4. ### Can you explicitly assign `undefined` to a variable?
    Yes, but it is **not recommended**.
    ```javascript
    let i = undefined;
    console.log(i); // undefined
---
5. ### What is hoisting in JavaScript?
    Hoisting moves variable and function declarations to the top of their scope.
    ```javascript
    console.log(a); // undefined (due to hoisting)
    var a = 10;
    ---
6. ### How does block scope work?
    Variables declared with let or const are only accessible inside `{}`.
    `if (true) {
        let x = 5;
        }
    console.log(x); // ReferenceError`
    ---
7. ### What is the scope of a variable?
    Scope defines where a variable is accessible: Global, Function, and Block.
---
8.  ### Should you terminate all lines with semicolons?
    Not mandatory because JavaScript uses ASI (Automatic Semicolon Insertion), but recommended to avoid errors.
    ---
9. ### Why does this function return undefined despite returning an object?
    Because ASI inserts a semicolon after `return`.
    `function test(){
    return 
    {
        a: 5
    }
    }
    const obj = test();
    console.log(obj); // undefined `
    Correct way:
    `
        function test(){
        return {
            a: 5
        };
        }
    `
    ---
10. ### Can we use the `arguments` object in an arrow function?
    No. Arrow functions do not have their own arguments object.
    `const f = () => console.log(arguments); // ReferenceError`
    ---
11. ### Which is the best way to create a new array with assignment?
    Use the spread operator.
    `const arr1 = [1, 2];
    const arr2 = [...arr1];
    console.log(arr2); // [1, 2]
    `
    ---
12. ### How can a function accept any number of parameters?
    By using rest parameters.
    `
        function sum(...nums){
        return nums.reduce((a, b) => a + b);
        }
        console.log(sum(1, 2, 3, 4)); // 10
    `
    ---
13. ### Can the rest operator be placed anywhere in parameters?
    No. Rest parameter must be the last parameter.
    `function test(...a, b) {} // Invalid `
---
14. ### How will you validate positive or negative Infinity?
   ` Number.isFinite(Infinity);   // false
     Number.isFinite(-Infinity);  // false`
---
15. ### What will be the output of `NaN == NaN`?
    `console.log(NaN == NaN); // false`
    ---

16. ###  What will be the output of the below statement?
`console.log(NaN == NaN);`
**Output:** `false`
**Explanation:** According to the IEEE 754 floating-point standard, `NaN` is not equal to any value, including itself.

---

17. ###  What is the difference between isNaN() and isFinite() method?
* **`isNaN()`**: Returns `true` if the value is `NaN` or cannot be converted into a number.
* **`isFinite()`**: Returns `true` if the value is a finite number (not `NaN`, `Infinity`, or `-Infinity`).

---

18. ###  Explain the syntactical features of arrow function.
1.  **Shorter syntax:** Uses `=>` instead of the `function` keyword.
2.  **No `this` binding:** Does not have its own `this` context.
3.  **Implicit return:** For single-line expressions, `return` is implied.
    ```javascript
    const add = (a, b) => a + b;
    ```

---

19. ###  Why this does not work in arrow function?
Arrow functions do not have their own `this` context. Instead, they capture the `this` value of the parent lexical scope (the context in which they were created).

---

20. ###  Explain output of following code with reason?.
    ```javascript
    const obj = {
        method: () => {
            console.log(this);
        }
    }
    `Output : // window / global object
    Reason: arrow function ignores object as this.`
---
21. ### How can you handle arguments in arrow functions?
    `Use rest parameters.
    `const f = (...args) => console.log(args);
    f(1, 2, 3); // [1, 2, 3]
    `
---
22. ### Can you write an IIFE using arrow function syntax?
    Yes.
    `   (() => {
    console.log("IIFE");
    })(); `

---
23. ### How can you access private variables outside a scope?
    Using a closure.
    `
    function outer() {
  let x = 10;
  return () => x;
}
const fn = outer();
console.log(fn()); // 10
    `
---

24. ### What are the advantages of closures?
   * Data privacy
   * Encapsulation
   * State management
---
25. ### What is function currying?
Transforming a function with multiple arguments into nested single-argument functions.
---
26. ### Explain the currying multiplication function
`
const multiplication = a => b => c => a * b * c;
console.log(multiplication(2)(3)(4)); // 24

`
Each function captures its argument using closures.
---
27. ### Explain practical usage of function currying
    * Reusable functions
    * Logging
    * Validation
    `const add = a => b => a + b;
const add10 = add(10);
console.log(add10(5)); // 15
`
---
28. ### What is the purpose of an iterator?
Iterators provide sequential access to elements.

---
29. ### How do you create an iterator?
`function createIterator(arr) {
  let i = 0;
  return {
    next() {
      return i < arr.length
        ? { value: arr[i++], done: false }
        : { done: true };
    }
  };
}
`
---
30. ### Explain a practical use of an iterator
* `for...of` loops
* Custom data structures
---
31. ### What are generator functions?
Functions that can pause and resume execution using `yield`.
`
    function* gen() {
  yield 1;
  yield 2;
}

`
---
32. ### Which generator syntax is correct?
Both are valid:
`
function* test() {}
function *test() {}

`
33. ### Explain methods of generator objects
    * ` next()`
    * `return()`
    * `throw()`
---
34. ### Explain the use of `yield*`
Delegates iteration to another iterable or generator.
`
function* g1() {
  yield* [1, 2, 3];
}
console.log([...g1()]); // [1, 2, 3]

`
35. ### Can you prevent return() from terminating a generator?
No.
Calling `generator.return()` immediately ends the generator and sets `done: true.`