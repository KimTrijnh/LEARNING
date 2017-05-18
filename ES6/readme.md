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

3. Arrow function `()=> some results` or `(arg1, arg2) => some results;`

```
var square = function (a) {
return a*a; }

var square = (a) => a*a;
```

4. Default parameter: when no argument is passed to function parameter, argument will take the default value

```
var hello = function(name="buddy") { return "Hello" + name; }

or 
var hello =(name="buddy") => "Hello" + name;

hello("Linh); // Hello Linh
hello(); // Hello buddy   <= return default name
```
5. Rest Operator `...args`. No need to know how many and which parameters of a function, use '...args' then the arguments of the function are ** stored in an array **.

```
var numberOfArgument= (...args) => args.length;
numberOfArgument("string",2,null, undefined); // 4   (arguments stored in an array args=["string",2,null, undefined] )
```



