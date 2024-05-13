## 2.5 Higher Order functions

A “higher-order function” is a function that accepts functions as parameters and/or returns a function.

Example:

```javascript
function abcd(val) {
  val(); // This will execute the function passed as 'val'
}

function myfunc() {
  console.log("hey");
}

abcd(myfunc); // Pass the function reference without parentheses
```

