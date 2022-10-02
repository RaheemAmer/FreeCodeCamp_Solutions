`if/else` statements can be chained together for complex logic. Here is pseudocode of multiple chained `if` / `else if` statements:

```jsx
if (condition1) {
  statement1
} else if (condition2) {
  statement2
} else if (condition3) {
  statement3
. . .
} else {
  statementN
}
```

---

Write chained `if`/`else if` statements to fulfill the following conditions:

`num < 5` - return `Tinynum < 10` - return `Smallnum < 15` - return `Mediumnum < 20` - return `Largenum >= 20` - return `Huge`

```jsx
function testSize(num) {
  // Only change code below this line
  if (num < 5){
    return "Tiny";
  }
  else if (num < 10){
    return "Small";
  }
  else if (num < 15 ){
    return "Medium";
  }
    else if (num < 20 ){
    return "Large";
  }
    else if (num >= 20){
    return "Huge";
  }
  return "Change Me";
  // Only change code above this line
}

testSize(7);
```
