# ES6 FEATURES 


1. `Let` to declare variable that only can locally used in a block- { "this is a block"}

```
if(true) {
var a =2; }
console.log(a) // 2

if(true) {
let a=2; }
console.log(a) // error a not defined yet
```

2. `const` have same feature like `let` but a constant variable can not be updated

```
const TAX =0.1;
TAX = 0.2; // error
```

**Note**: we can not change the constant variable value. But if variable is an object ( array, object, function), it can be updated. 
```
const Arr =[1,2,3];
Arr =[2,3]; //error
Arr.push(4);  //ok
Arr; // [1,2,3,4]

const foo =(a) => a*2;
foo = () =>4; //error;
foo(2); //4
foo(3); //6 -> value can be updated.
```

3. **Arrow function** `()=> some results` or `(arg1, arg2) => some results;`

```
var square = function (a) {
return a*a; }

var square = (a) => a*a;
```

4. **Default parameter**: when no argument is passed to function parameter, argument will take the default value

```
var hello = function(name="buddy") { return "Hello" + name; }

or 
var hello =(name="buddy") => "Hello" + name;

hello("Linh); // Hello Linh
hello(); // Hello buddy   <= return default name
```
5. **Rest Operator** `...args`. No need to know how many and which parameters of a function, use '...args' then the arguments of the function are **stored in an array**.

```
var numberOfArgument= (...args) => args.length;
numberOfArgument("string",2,null, undefined); // 4   
(arguments stored in an array args=["string",2,null, undefined] )
```

6. **Spread array**: by **Spead operator** unpack an array into a chain of string. 
```
var arr1 =["name",25,"pink"];
var arr2 =["rock",...arr1] 
arr2; //["rock","name",25,"pink"]

var arr = [6, 89, 3, 45];
var maximus = Math.max.apply(null, arr); // returns 89
const arr = [6, 89, 3, 45];
const maximus = Math.max(...arr); // returns 89
```
**NOTE**: the spread operator only works in-place, meaning that `...arr` only put in `(...arr)` of a function/method or `[...arr]` of other arrays.


7. **Destructuring Assignment** for an Object and nested Object


8. **Destructuring Assignment** for an Array

9. Combine **Destructuring Assignment** & **Rest Operator** `const [a,b,...arr] =[1,2,3,4,5,6,7,8,9]`
```
const [a,b,...arr] =[1,2,3,4,5,6,7,8,9]
console.log(a,b)// 1,2
console.log(arr); //[3,4,5,6,7,8,9]
```

10. **Destructuring Assignment** as function's parameter `const foo =({a,b}) => some results; `

11. **Template Literal** ` `it is a template ${variable}` `
- `+ variable` replaced by ${variable}
- template literal can be multiline
```
const person = {
  name: "Zodiac Hasbro",
  age: 56
};

// string interpolation
const greeting = `Hello, my name is ${person.name}!
I am ${person.age} years old.`;

console.log(greeting); // prints
// Hello, my name is Zodiac Hasbro!
// I am 56 years old.
```
12. Write Concise Object Literal Declarations Using Simple Fields
```
const createPerson = (name, age, gender) => ({name,age,gender});
console.log(createPerson("Zodiac Hasbro", 56, "male")); // returns a proper object
```
