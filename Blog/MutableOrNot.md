1. Mutable: Object,
2. Unmutable: String,

ví dụ cho mutable và unmutable.

```
var str1="2e";
str1;
"2e"
var str2=str1;
undefined
str2;
"2e"
str2=2;
2
str1;
"2e"
var ob = { a: 1, b: 3};
var ob1= ob;
undefined
ob1;
Object {a: 1, b: 3}
ob1.a=0;
0
ob1;
Object {a: 0, b: 3}
ob;
Object {a: 0, b: 3}
```
