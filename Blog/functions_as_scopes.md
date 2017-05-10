# Functions as Scopes.

1 function sẽ được thành lập như sau


```
//khai báo function
function myFuctionName() { 
//do something; 
}
// execute function 
myFunction(); 
```
function thực ra có thể được coi là 1 biến. Hãy so sánh với 
``` var a = 4;```

trong đó `function` dùng để khai báo-declare 1 function tương tự như `var` dùng để declare biến-variable. 
myFunctionName và a là tên- gọi chung là indentifier. 

- function-based scope: biến được declared trong 1 function sẽ được dùng locally ( private cho scope của function đó). Nên trong trường hợp
mún tạo 1 scope riêng bao quanh các biến để chương trình được gọn và biến ko bị vô tình gọi chồng lên nhau thì ta mới gom những biến này đặt
vào 1 function based scope. 
```
function valarea() {
var a = 2;
var b= 3; 
console.log( a+b);
}
valarea();
// bên ngoài ko thể gọi các giá trị a, b trong valarae() được
```
nhưng làm vậy sẽ tạo ra thêm 1 function với tên và làm polute môi trường code. để giải quyết, ta đem function biết thành 1 expression

``` 
(function valarea() {
do something; }) ();

```
### anonymous function và Named ( function ko tên và function có tên)
```function () {console.log("I am a no name function");} ```

anonymous function thường được thấy trong call back function. Bởi vì những trường hợp này ta thuwòng ko cần thiết sử dụng function này ở
chỗ khác, function đc dùng 1 lần hết nhiệm vụ thfi thôi, nên thường tên function sẽ đc bỏ qua. eg

``` setTimeout( callbackfunction, time)
setTimeout( function() {console.log("I wated 1 s");}, 1000)
vs
setTimeout( function timeoutHandler() {console.log("I wated 1 s");}, 1000)
```
Tuy nhiên, đây ko pải là 1 good practice. cách tốt nhât là luôn luôn kèm tên cho function, kể cả khi nó là callbackfunction. 

