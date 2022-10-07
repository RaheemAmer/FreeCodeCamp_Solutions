In JavaScript, we often don't need to name our functions, especially 
when passing a function as an argument to another function. Instead, we 
create inline functions. We don't need to name these functions because 
we do not reuse them anywhere else.

To achieve this, we often use the following syntax:

```jsx
const myFunc = function() {
  const myVar = "value";
  return myVar;
}
```

ES6 provides us with the syntactic sugar to not have to write anonymous functions this way. Instead, you can use **arrow function syntax**:

```jsx
const myFunc = () => {
  const myVar = "value";
  return myVar;
}
```

When there is no function body, and only a return value, arrow function syntax allows you to omit the keyword `return` as well as the brackets surrounding the code. This helps simplify smaller functions into one-line statements:

```jsx
const myFunc = () => "value";
```

This code will still return the string `value` by default.

---

Rewrite the function assigned to the variable `magic` which returns a `new Date()` to use arrow function syntax. Also, make sure nothing is defined using the keyword `var`.

```jsx
const eatMe = function (){
	let number = 10;
	let total = 0;
	return (number + total);
}
const eatMe = () => {
	let number = 10;
	let total = 0;
	return (number + total);
}
const eatMe = () => number + total;
--------
const magic = () => new Date();
```