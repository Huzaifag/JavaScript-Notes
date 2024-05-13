## 2.1 Window object

**Defination:**

- The window object is supported by all browsers. It represents the browser's window.

- All global JavaScript objects, functions, and variables automatically become members of the window object.

- Global variables are properties of the window object.

- Global functions are methods of the window object.

- Even the document object (of the HTML DOM) is a property of the window object:
```javascript
window.document.getElementById("header");
```
is the same as:
```javascript
document.getElementById("header");
```
### Window Size
```javascript
let w = window.innerWidth; // the inner width of the browser window (in pixels)
let h = window.innerHeight;// the inner height of the browser window (in pixels)
```
### Other Window Methods
```javascript
window.open() // open a new window
window.close() // close the current window
window.moveTo() // move the current window
window.resizeTo() // resize the current window
```
**Explain:**

JS main khuch cheezain nhi hain jo hum use kar sakte hain aur wo cheezain hamain js se nhi balke browser se milti hain , wo saari cheezain jo js ka part nhi hai but phir bhi use kar sakty hai , dhoond sakte hain ek particular object main jiska naam window hai.

