## Lesson 1.9: Control Structures
### 1) if-else and if-esle if

Jab baat agar mager par a jaye, ya phir bat a jaye aysa hua to ye waisa hua to ye.

Use for desion making.

Example : 
```javascript
let myage = 18;

 if (myage < 18) {
 //if this condition is true than this statement will print
 console.log("You are chlid my dear:");
 } 

 else {
//this will print if 1st one is false
console.log("You are an adult:");
}
```
![image](https://github.com/Huzaifag/JavaScript-Notes/assets/92973781/d4af42ce-d5bd-486e-83f8-2450687389e6)

 js main jo bhi likho wo mainly ya true hoga ya false
> **Falsy values** = 0 false undefine NULL NaN document.all

> **truthy values** = all others

### 2) Loops
if we to run same code over and over again with different value than we us loops.

![image](https://github.com/Huzaifag/JavaScript-Notes/assets/92973781/e54d5a98-a51b-4f4f-b471-33db0d9d2b25)


**1.For loop:-** loops through a block of code a number of times.

Syntax: 
```javascript
for (Initialization ; condition; increament) {
// code block to be executed
 }
```
Example:
```javascript
for (let i = 0; i < 5; i++) {
console.log("itration:" + i);
 }
```
**2.While loop:-** loops through a block of code while a specified condition is true.

Example:
```javascript
let j = 0;

while (j <= 5) {
j++;
console.log("2n itration:" + j);
}
```
**3.foreach loop:-** Sirf array py chalta hai,jab har element py kuch na kuch perform karna ho. 

Example:
```javascript
var a1 = [1,2,3,4,5,6,7];
a1.forEach(function(val){
console.log(val + 2);
})
```

- foreach kabhi bhi by default aapke array ko change nhi karta wo appko changes kar k deta
hai array ki temporary copy pr jis wajah se array same rehta hai.

**4.Forin loop:-** object par loop chalany k liye.

Example:
```javascript
var obj1 = {
name1 : "Huzi",
class : " IT",
rollNo : "bsf2009558"
}

for(var key in obj1 ){
console.log(key, obj1[key]);
}
```
**5. dowhile loop:-**
```javascript
var ar1= 12;

do{

console.log("hey");
ar1++;

}while(ar1 < 15);
```
