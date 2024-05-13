## 2.6 Constructor Function

A constructor function is a special type of function that is used to create and initialize objects.

Constructor functions are typically used in conjunction with the new keyword to create instances (objects) of a particular type or class.

Example:

```javascript
class person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }
}

var person1 = new person("huzi", 23);
var person2 = new person("babar", 21);
```

