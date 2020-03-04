## Creating a global variable within a function

Somehow, I thought defining variable within a function like this 

```javascript

let globalVariable = "global";

function jsScope = (){
  let superGlobalVariable = "super global"; 
}
```

However, it's about not creating variable with let or const which makes that variable a global variable.

```javascript

let globalVariable = "global";

function jsScope = (){
  superGlobalVariable = "super global"; 
}
```


Hee ha!
