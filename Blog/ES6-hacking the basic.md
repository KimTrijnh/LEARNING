**All about ES6**

** EMAScript (aka ES) is a standadized spec of JS. it will be updated, rivised, added more features to ensure the unifying of JS's features. ES5 is published in 2009 and commonly supported by different browsers. ES6 (2015) are the current version. and ES7 (2017) are coming in the way. Therefore, this time we have to update our skillset to familiar with using ES6, and keep aware that the next-coming of ES7. **

### The Update btween ES5 and ES6.
1. Declaration of variables.

 
 | No.      |    feature name      |   ES5  | ES6  | ES7   | 
 |----------|:--------------------:|:------:|:-----:|-----:|
 | 1 |  variables | $1600 | $1600 | $1600 | $1600 |
 | col 2 is |    centered   |   $12 |  $12  |  $12  |  $12  |
 | col 3 is | right-aligned |    $1 |    $1 |    $1 |    $1 |
  


### Examples
1. variables by `var`  `let` and `const`
 - `var`
 - `let` will limit the use of variable inside a statement, a block, a expression. 
 - `const`: variables can not be reassigned. Objects such as array can not re-assigned but can be mutable by adjust/modify individual items.
 ``` 
  for ( i=0; i<10; i++) {
var a = i +2; 
}
console.log(a); // return 11

for ( i=0; i<10; i++) {
let a = i +2;  
}
console.log(a); // return error 
```
```for ( i=0; i<10; i++) {
var a = i +2; 
  
  function plus() {
    var b = a+2; // b is only locally used in block of plush
    console.log(b);
  }
  
 
}
console.log(a);
plus(); // return 13
```
```
for ( i=0; i<10; i++) {
var a = i +2; 
let b;
      b = a+2; // b only can used in the for loop
   }
console.log(a); 11
console.log(b); return error
```
