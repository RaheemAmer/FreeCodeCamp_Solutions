`catch` is the method used when your promise has been rejected. It is executed immediately after a promise's `reject` method is called. Here’s the syntax:

```jsx
myPromise.catch(error => {

});

```

`error` is the argument passed in to the `reject` method.

---

Add the `catch` method to your promise. Use `error` as the parameter of its callback function and log `error` to the console.

```jsx
const makeServerRequest = new Promise((resolve, reject) => {
  // responseFromServer is set to false to represent an unsuccessful response from a server
  let responseFromServer = false;
    
  if(responseFromServer) {
    resolve("We got the data");
  } else {  
    reject("Data not received");
  }
});

makeServerRequest.then(result => {
  console.log(result);
});
makeServerRequest.catch(error => {
	console.log(error);
});
```