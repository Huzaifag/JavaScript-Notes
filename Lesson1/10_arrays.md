## Lesson 1.10:Arrays

A data structure that allows us to store multiple values

Example:

```javascript
var fruites = ["Apple", "Banana", "Cherry"];

//display array elements:
 for (let i = 0; i < fruites.length ; i++) {

 console.log(fruites[i]);
 }
```
- array index starts from 0.
### array methods:
1) push():Add element at the end of the array:
```javascript
fruites.push("date");
```
2) pop():Remove elements at the end of the array
```javascript
fruites.pop();
```
3) shift():removes 1st element
```javascript
fruites.shift();
```
4) unshift():adds 1st element
```javascript
fruites.unshift("Apple");
```
5) splice():Adds / removes at specific position.
```javascript
fruites.splice(2, "banana");
```
**Copy reffernce of an array to other variable.**
```javascript
var copyfruites = [...fruites];

console.log(copyfruites);
```