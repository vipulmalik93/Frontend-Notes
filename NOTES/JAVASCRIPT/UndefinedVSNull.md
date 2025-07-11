 ### undefined
➤ What is it?
undefined means a variable has been declared but has not yet been assigned a value.

➤ Examples:

```
let a;
console.log(a); // undefined
```

```
function test() {}
console.log(test()); // undefined (no return value)
```

➤ Who sets it?
JavaScript itself assigns undefined by default.

➤ Common Use:
Default value for uninitialized variables

Return value of a function with no return

When object property doesn’t exist

---

### null
➤ What is it?
null is an intentional absence of any object value. It means "nothing", but set deliberately.

➤ Examples:

``` 
let a = null;
console.log(a); // null
```

```
let person = {
  name: null  // Intentionally saying: "no name"
};
```


➤ Who sets it?
Developer sets it explicitly.

➤ Common Use:
To reset or clear a value

As a placeholder to represent no object

---

| Feature                 | `undefined`                   | `null`                                 |
| ----------------------- | ----------------------------- | -------------------------------------- |
| Type                    | `undefined`                   | `object` (this is a long-standing bug) |
| Assigned by             | JavaScript                    | Developer                              |
| Meaning                 | Not assigned                  | Intentionally empty                    |
| Use Case                | Missing value                 | Explicitly no value                    |
| Equality (`==`)         | `undefined == null` → `true`  | `null == undefined` → `true`           |
| Strict Equality (`===`) | `undefined !== null` → `true` | Different types                        |


---

✅ Best Practice
Use undefined to check if something has not been assigned.

Use null when you want to intentionally empty a value.

