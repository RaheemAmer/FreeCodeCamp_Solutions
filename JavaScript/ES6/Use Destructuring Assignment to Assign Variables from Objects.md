Destructuring allows you to assign a new variable name when 
extracting values. You can do this by putting the new name after a colon
 when assigning the value.

Using the same object from the last example:

```jsx
const user = { name: 'John Doe', age: 34 };
```

Here's how you can give new variable names in the assignment:

```jsx
const { name: userName, age: userAge } = user;
```

You may read it as "get the value of `user.name` and assign it to a new variable named `userName`" and so on. The value of `userName` would be the string `John Doe`, and the value of `userAge` would be the number `34`.

---

Replace the two assignments with an equivalent destructuring assignment. It should still assign the variables `highToday` and `highTomorrow` the values of `today` and `tomorrow` from the `HIGH_TEMPERATURES` object.

```jsx
const HIGH_TEMPERATURES = {
  yesterday: 75,
  today: 77,
  tomorrow: 80
};

// Only change code below this line
const {today: highToday, tomorrow: highTomorrow} = HIGH_TEMPERATURES;
// Only change code above this line
```