**Variables** which are **declared** within a **function**, as well as the **function parameters**, have **local scope**. That means they are only **visible** within that **function**.

```jsx
function myTest() {
  const loc = "foo";
  console.log(loc);
}
myTest(); // foo
console.log(loc); //Uncaught ReferenceError
```

<aside>
💡 The `myTest()` function call will display the string `foo` in the console. The `console.log(loc)` line (outside of the `myTest` function) will throw an error, as `loc` is not defined outside of the function.

---

The editor has two `console.log`s to help you see what is happening. Check the console as you code to see how it changes. Declare a local variable `myVar` inside `myLocalScope` and run the tests.

---

**Note:** The console will still display `ReferenceError: myVar is not defined`, but this will not cause the tests to fail.

</aside>

```jsx
function myLocalScope() {
  // Only change code below this line

  console.log('inside myLocalScope', myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope
console.log('outside myLocalScope', myVar);
```
