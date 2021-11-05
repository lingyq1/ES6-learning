## 1. template literal 
### definition: like a non-code text 通过模板方便地插入想要的数据信息
``` 
const k = { firstName :"Wang" };
const b =  `Could you please get ${k.firstName} over here ?`
console.log(b);
```
## 2. destructuring objects   

### definition:can use the same variate 
``` 
const member= {name:"Anzo",
                age:"25",
                gender:"male"
        }
const { name ,gender} = member;
console.log(name);
console.log(gender);
```
## 3. spread operator
### definition: can represent the rest object
```
const a = [1,2,3];
const b = [...a,4,5];
console.log(a);
console.log(b);
```
## 4.object literal  
### definition: How to express a variable
```
function member (information){
  const {name,age} = information;
  console.log(`I'm ${name}.I'm ${ age} years old now`);
}
member({name:'Anno',age:'25'});
```
## 5. for of loop
### definition: You can iterate over each object 
```
let arrs = [1,2,3];
const num =0;
for(const a of arrs ){
 console.log(`the number is ${num + a}`);
}
```
## 6.rest operator   
### definition: allow us to represent an indefinite number of argument as an array
```
 function sum(a, b, c) {
    return a + b + c;
  }
  var args = [1, 2, 3];
  console.log(sum(...args)); 
```
## 7. allow fucntion 
### definition: which can omit function name  even the round brackets
```
const total= (a,b) =>{
   console.log( a + b); 
  }
total(1,2);
```
## 8.default parameters 
### definition: which is set to undefined
```
const player = (sport)=>{
    console.log(`Kobe is a great ${sport} player.`);
}
player("basketball");
player(); //default

```
## 9.includes() 
### definition:which can know whether contain boolean value
```
let arr1 = [1,2,3,5];
console.log(arr1.includes(2));
```
## 10.let & const
### definition: let can assign a value ,like var but couldn't hoist the variable;const used in the constant variable,and can't assign value again.
```
const num1 =2;
console.log(num1);
// num1 = 3;
// console.log(num1);
let num2 = 3;
console.log(num2);
num2 =4;
console.log(num2);
```
## 11.import & export
###  definition: Import a binding exported by another module
```
export.js:
export const data1 = [1,2,3];
import.js:
import {data1} from "./export.js";
console.log(data1);

```
## 12.padStart() &padEnd();
### definition: fills the current string with another string from left/right side;
```
const string1 ="g";
console.log(string1.padStart(2,"e"));
console.log(string1.padEnd(2,"e"));

```
## 13. class
### definition:creates a new class with the given name based on stereotype inheritance
```
class add{
 constructor(a,b){
     this.total= a+b;
 }
}
console.log(new add(2,3).total);

```

