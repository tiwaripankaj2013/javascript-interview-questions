# 📘 JavaScript Basic Interview Questions

---


<details>
<summary><strong>Q1. What is <code>undefined</code> in JavaScript?</strong></summary>

`undefined` means a variable has been declared but not assigned any value.

```js
let a;
console.log(a); // undefined

<details> <summary><strong>Q2. What will be the output of <code>undefined == null</code> and <code>undefined === null</code>? Why?</strong></summary>
console.log(undefined == null);  // true
console.log(undefined === null); // false


Explanation:

== performs type coercion and treats both as empty values

=== checks both value and type, which are different

</details>

### Table of Contents

<!-- TOC_START -->
| No. | Questions |
| --- | --------- |
| 1 | [Q1. What is undefined in JavaScript? ](#What-is-undefined-in-JavaScript) |

1. **Undefined:**

      `undefined` means a variable has been declared but not assigned any value.
    ```let a;
        console.log(a); // undefined
       ```
