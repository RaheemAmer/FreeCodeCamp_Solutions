You can add new properties to existing JavaScript objects the same way you would modify them.

Here's how we would add a `bark` property to `ourDog`:

```jsx
ourDog.bark = "bow-wow";
```

or

```jsx
ourDog["bark"] = "bow-wow";
```

Now when we evaluate `ourDog.bark`, we'll get his bark, `bow-wow`.

Example:

```jsx
const ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

ourDog.bark = "bow-wow";
```

---

Add a `bark` property to `myDog` and set it to a dog sound, such as "woof". You may use either dot or bracket notation.

```jsx
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.bark = "woof";
```
