## 2.8 New Keyword:

- The new keyword is used to create instances of objects or to invoke constructor functions.
- When you use new with a constructor function, it performs the following steps:

1. A "new" empty object is created.
2. The 'this' keyword inside the constructor function is set to refer to the newly created object.
3. The constructor function is executed, and it can modify the properties and methods of the newly created object.

If the constructor function does not explicitly return an object, the newly created object is returned automatically.
Example:

```javascript
function salam() {
  this.message = "Assalam-o-Alaikum!";
}

var mySalam = new salam();
```

