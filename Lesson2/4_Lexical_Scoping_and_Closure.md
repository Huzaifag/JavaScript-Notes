## 2.4 Lexical Scoping and Closure:

Lexical scoping is the process used to define the scope of a variable by its position in the source code.

ye hota hai ek chart jisme likha hota hai appka func kin cheezon ko access kar sakta hai kin ko nhi.

```javascript
function outer() {
  let name = "Huzaifa"; // 'name' is declared and accessible within the 'outer' function

  function inner() {
    let secret = "my123";
    console.log("inner", name); // 'name' is accessible in the 'inner' function
  }

  function innerTwo() {
    console.log("innerTwo", name); // 'name' is accessible in the 'innerTwo' function
    console.log(secret); // 'secret' is not accessible here because it's declared in the 'inner' function
  }

  inner(); // Call the 'inner' function
}

outer(); // Call the 'outer' function

console.log("outer", name); // 'name' is not accessible here because it's declared in the 'outer' function
```

### Closure:

- A closure is a function that "closes over" its surrounding lexical scope, capturing variables from that scope even after the outer function has finished executing.

  - Closures allow you to maintain access to the variables of an outer function, even if that function has already returned or completed.

  Example:

  ```javascript
  function outer() {
    let y = 20; // Variable 'y' is defined here

    function inner() {
      console.log(y); // 'y' is accessible here even after 'outer' function has returned
    }

    return inner; // 'inner' function is returned, creating a closure
  }
  const closureFunc = outer(); // 'closureFunc' is a closure
  closureFunc(); // Accesses 'y' even though 'outer' has completed
  ```

