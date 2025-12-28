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