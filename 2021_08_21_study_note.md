## 1. template literal 
### definition: like a non-code text
``` 
const k = { firstName :"Wang" };
const b =  `Could you please get ${k.firstName} over here ?`
console.log(b);
```
## 2 destructuring objects   

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