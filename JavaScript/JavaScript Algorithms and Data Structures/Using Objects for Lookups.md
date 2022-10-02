Objects can be thought of as a key/value storage, like a dictionary. 
If you have tabular data, you can use an object to lookup values rather 
than a `switch` statement or an `if/else` chain. This is most useful when you know that your input data is limited to a certain range.

Here is an example of a simple reverse alphabet lookup:

```jsx
const alpha = {
  1:"Z",
  2:"Y",
  3:"X",
  4:"W",
  ...
  24:"C",
  25:"B",
  26:"A"
};

const thirdLetter = alpha[2];
const lastLetter = alpha[24];

const value = 2;
const valueLookup = alpha[value];
```

`thirdLetter` is the string `Y`, `lastLetter` is the string `C`, and `valueLookup` is the string `Y`.

---

Convert the switch statement into an object called `lookup`. Use it to look up `val` and assign the associated string to the `result` variable.

```jsx
// Setup
function phoneticLookup(val) {
  let result = "";

  // Only change code below this line
  const lookup = {
    "alpha":"Adams",
    "bravo":"Boston",
    "charlie":"Chicago",
    "delta": "Denver",
    "echo": "Easy",
    "foxtrot": "Frank"
  }
 result = lookup[val];
  // Only change code above this line
  return result;
}

phoneticLookup("charlie");
```
