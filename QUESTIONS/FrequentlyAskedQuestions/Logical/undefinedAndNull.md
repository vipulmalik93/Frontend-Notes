| Feature                   | `undefined`                               | `null`                                    |
| ------------------------- | ----------------------------------------- | ----------------------------------------- |
| **Type**                  | `undefined`                               | `object` ← (quirk in JavaScript)          |
| **Meaning**               | Variable declared but **not assigned**    | **Intentional absence** of any value      |
| **Who sets it?**          | JavaScript engine                         | Developer (you)                           |
| **Use Case**              | Default value for uninitialized variables | Explicitly set when a variable is "empty" |
| **Example**               | `let a; console.log(a); // undefined`     | `let a = null; console.log(a); // null`   |
| **Falsy?**                | ✅ Yes                                     | ✅ Yes                                     |
| **Equality (==)**         | `undefined == null` → `true`              |                                           |
| **Strict Equality (===)** | `undefined === null` → `false`            |                                           |


---

### typeof undefined; // "undefined"
### typeof null;      // "object" ❗ (this is a well-known JavaScript bug)

---

'5' == 5       // true  → because '5' is coerced to 5
'5' === 5      // false → different types (string vs number)

null == undefined  // true  → special rule in JS
null === undefined // false → different types

0 == false    // true  → because false is coerced to 0
0 === false   // false → different types (number vs boolean)


---

| Question                   | Answer                                          |
| -------------------------- | ----------------------------------------------- |
| Why `==` and `===` differ? | Because `==` does type coercion, `===` does not |
| Which one should I prefer? | Use `===` for safer comparisons                 |
| Is `'0' == 0` true?        | ✅ Yes (`'0'` is coerced to `0`)                 |
| Is `'0' === 0` true?       | ❌ No (string ≠ number)                          |


---
### In JavaScript, false is coerced to 0 when using loose equality (==) or in arithmetic contexts.
🔁 Type Coercion: false → 0
Here are a few examples where this happens:

```
false == 0        // ✅ true
false + 1         // ✅ 1 (false → 0 → 0 + 1)
Number(false)     // ✅ 0
```

🧠 Why?
Because JavaScript has type coercion rules that convert non-numbers to numbers when needed:
| Value       | To Number |
| ----------- | --------- |
| `false`     | `0`       |
| `true`      | `1`       |
| `''`        | `0`       |
| `'5'`       | `5`       |
| `null`      | `0`       |
| `undefined` | `NaN`     |


❗ But careful with ===
```
false === 0    // ❌ false (different types: boolean vs number)
```

✅ Summary

✔️ false == 0 → true because of type coercion

❌ false === 0 → false because types are different

Number(false) → 0


---

| Expression     | Coerced To | Result |
| -------------- | ---------- | ------ |
| `true + 1`     | `1 + 1`    | `2`    |
| `false + 1`    | `0 + 1`    | `1`    |
| `true + true`  | `1 + 1`    | `2`    |
| `true + false` | `1 + 0`    | `1`    |

---

| Value   | Number Equivalent |
| ------- | ----------------- |
| `true`  | `1`               |
| `false` | `0`               |

---

```
true + 1 === 2  ✅
```







