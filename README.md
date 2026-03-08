# Programming-Hero-Assignment-5

<p>To show the live demo <a href="https://nayon-kumar.github.io/Programming-Hero-Assignment-5/">Click Here</a></p>

## Some question and answer

#### 1. What is the difference between var, let, and const?

**Var**: It can be redeclare and reassing. It suppot hoisted. It is old way, generally we don't use it.

```javascript
var name = "Nayon";
var name = "Rohim"; // allowed
name = "Korim"; // allowed
```

**Let**: It can be reassign but can not be redeclare. This is modern way. It can be hoisted but temporal dead zone (TDZ).

```javascript
let x = 20;
x = 30;
//let x = 50 (Not allowed)
```

**Const**: It value can not be change. We can not redeclare and reassing it's value.

```javascript
const PI = 3.1416;
// PI = 100; (Not allowed)
// const PI = 200; (Not allowed)
```

#### 2. What is the spread operator (...)?

Spread operator used to spread something. Using this we can spread array and object. It is one kind of copy or clone. If we use it the reference array or object value will not change. Without spread operator if we change one array/object value then other array/object value will be changed.

```javascript
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];

const arr3 = [...arr1];
const arr4 = [...arr1, ...arr2, 7, 8];

const user = { name: "Nayon Kumar", age: 24 };
const newUser = { ...user };
```

#### 3. What is the difference between map(), filter(), and forEach()?

**map()**: It create new array transfering each element. It return a new array as same length of original array.

```javascript
const numbers = [1, 2, 3, 4];
const doubled = numbers.map((num) => num * 2);
```

**filter()**: It create new array based on the condition. If the condition is satisfied then it go to the new array element. It return a new array according to the condition.

```javascript
const numbers = [1, 2, 3, 4, 5];
const even = numbers.filter((num) => num % 2 === 0);
```

**forEach()**: It run for each element but don't return new array.

```javascript
const numbers = [1, 2, 3];
numbers.forEach((num) => {
  console.log(num);
});
```

#### 4. What is an arrow function?

Arrow function is short and modern way of declare a function. We use => (arrow) sign for write arrow function. This function can be with parameters also without parameter.

```javascript
const add = (a, b) => a + b;

const square = (x) => x * x;

const greet = () => "Hello";

const myFun = (a, b) => {
  const result1 = a + b;
  const result2 = result1 * a * b;
  return result2;
};
```

#### 5. What are template literals?

Template literals allow create string using variable. We use `` (backtick) and ${} for it.

```javascript
const name = "Nayon Kumar";
const message = `Hello ${name}`;
```
