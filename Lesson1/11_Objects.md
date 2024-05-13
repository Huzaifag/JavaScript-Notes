## Lesson 1.11:Objects
Organize and store data about single entity in key pair formate.

Example:
```javascript
var watch = {
brand: "titan",
price: "16k",
color: "Silver", //properties
type: "auttomatic",
1digital: false,
//you can also add function into an object
setTime: function () {}, //Methods
};
```
- Deleting a value of object.
```javascript
delete watch.type;
```
- copy reffernce of an object to other variable.
```javascript
var copywatch = {...watch};
console.log(copywatch);
```