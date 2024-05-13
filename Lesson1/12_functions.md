## Lesson 1.12: Functions
A block of code to perform perticular task.
- invokes only when we call
**Function K mainly 3 kaam hain:**
1)Jab app apna code fooran nhi chalana chahty, Future main chalana chahte ho
2)Jab app apna code reuse karna chahty ho.
3)Jab app apna code chalana chahty ho with different data.

Example:
```javascript
function sumoftwo(num1, num2) {
  num1 = 9;
  num2 = 10;
  return num1 + num2;
}
console.log(sumoftwo());
```
### Types of Functions
**callback function:** Aisa func jo baad main chalta hai ussy hum ek function dy dyty hain ke bhaiya jab complete hojaana to ye func chala dena , aur us func ko hum callback function kehty hain.

Example:
```javascript
setTimeout(function(){
    console.log("2 sec baad chlna");
},2000);
```
**First class function:** js main ek concept hota hai jis main aap function ko as a value use kaar sakty ho.

```javascript
var myfunc = function(){}; //function ko variables main store kar sakty ho.

function sadafun(a){
a();
}

sadafun(function(){console.log("hello g");});
```
### Scope of a Function:
The scope of a function in JavaScript refers to the region or context in which variables and identifiers declared within that function are accessible. It defines where a particular variable can be used or accessed in your code.

#### 1. Local Scope (Function Scope):

>Variables declared inside a function using the var, let, or const keywords have local scope. They are only accessible within the function in which they are defined.

> Variables with local scope are often referred to as "local variables" or "function-scoped variables."

> They are not accessible from outside the function.

Example:
```javascript
function myFunction() {
var localVar = "I'm local!";
console.log(localVar); // Accessible here
}

console.log(localVar); // Error - localVar is not defined outside the function
```
#### 1. Global Scope :

> Variables declared outside of any function or at the top level of your code have global scope.

> Global variables are accessible from anywhere in your code, including within functions.

> However, it's considered good practice to limit the use of global variables because they can lead to naming conflicts and make your code less maintainable.


Example:
```javascript
var globalVar = "I'm global!";

function myFunction() {
console.log(globalVar); // Accessible inside function
}

console.log(globalVar); // Accessible here outside function as well.
```
