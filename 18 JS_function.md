## function

- ( ) means execute function.
- arguments are what given to functions.
```
alert("hey there!");   // "hey there!": arguments
```
- anonymous function.
```
var sayBye = function (){
  console.log("bye!");
};

sayBye();
```
## idea of dry
- do not repeat yourself.
- by adding arguments can make things easy.

## input, output, return
- return things: output, we get a value.
- w/o return things: undefined.
```
function multiply (a, b){
  return a*b;
}
```
- return is the final way to end a function, the program exits.

## functions are variables
- in JS, functions are variables
```
function multiply (a, b){
  return a*b;
}

var total = mutiply(4, 3);
alert(total);
```
- a, b: parameters.
- 4, 3: arguments.



## callback function
```
button.addEventListener("click", buttonAdd); 
input.addEventListener("keydown", enterAdd);
```
- This code in TODO LIST (add an new item to the list) uses "callback function".
- It means when the "JS engine" engine read this line, we have not need to execute it yet.   
the function will be execute until the "events" (click, keydown) happen.






