## 2.9 What is an IIFE?

An IIFE (Immediately Invoked Function Expression) is a function that runs the moment it is invoked or called in the JavaScript event loop.

Example:

```javascript
var ans = (function () {
  var privatevar;

  return {
    getter: function () {
      console.log(privatevar);
    },
    setter: function (val) {
      privatevar = val; // Corrected to access the private variable directly
    },
  };
})();

ans.setter(23);
ans.getter(); // Now it will correctly log the value 23
```

