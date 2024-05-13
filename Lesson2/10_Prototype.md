## 2.10 Prototype

All JavaScript objects inherit properties and methods from a prototype.

Example:

```javascript
function Person(first, last, age, eyecolor) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eyecolor;
}

const myFather = new Person("John", "Doe", 50, "blue");
const myMother = new Person("Sally", "Rally", 48, "green");

// Object inheritence prototyping

var human = {
  canFly: true,
  canTalk: true,
  canEat: true,
  canPlay: true,
};

var csStudent = {
  canCode: true,
  canMakeSW: true,
};

csStudent.__proto__ = human;
```