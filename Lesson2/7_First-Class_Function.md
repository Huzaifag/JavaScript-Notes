## 2.7 First-Class Function:

A programming language is said to have First-class functions if functions in that language are treated like other variables.

So the functions can be assigned to any other variable or passed as an argument or can be returned by another function.

1. Functions can be assigned to variables:

Example:

```javascript
const greet = function (name) {
  console.log(`Hello, ${name}!`);
};

greet("John"); // Call the function using the variable
```

1. Functions can be passed as arguments to other functions:

Example:

```javascript
function performOperation(operation, x, y) {
  return operation(x, y);
}

function add(a, b) {
  return a + b;
}

function subtract(a, b) {
  return a - b;
}

const result1 = performOperation(add, 5, 3); // Pass the 'add' function as an argument
const result2 = performOperation(subtract, 8, 2); // Pass the 'subtract' function as an argument
```

