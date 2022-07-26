JavaScript Snippets

Revere String program in Java Script

``` js
`Solution - 1`
function reverseString(str){
  var reverseStr = '';
  for(var i = str.length - 1; i >= 0; i--){
   reverseStr += str.charAt(i);
  }
  return reverseStr;
}
console.log(reverseString("pratik"));

`Solution - 2`
var name="pratik";
var rev='';
for(var i=name.length-1;i>=length;i--){
   rev+= name[i]
}
console.log(rev);
```


#Sort a array using custom function

```js
function sort(arr){
  for(var i=0;i<= arr.length;i++){
    for(var j=i;j<=arr.length;j++){
      if(arr[i] < arr[j]){
        var temp = arr[i];
        arr[i] = arr[j]
        arr[j] = temp;
      }
    }
  }
  return arr;
}
console.log(sort([2,6,3,1,99,33]));

```

```js
var numbers = [1, 2, 3, 4];
var colors = ["red", "green", "blue", "purple"];


for(let i=0;i<numbers.length;i++){
  var style= "style='color:"+colors[i]+"'";
  document.write("<h1 "+style+">"+numbers[i]+"</h1>");
}

```

```js
**Delete element by provided array index**
let a = [1,3,5,7,8,9,11];
let b = [0, 1, 3];

var j=0;
for(var i=0;i<b.length;i++){
  a.splice(b[i] - j,1);
  j =j+1;
}

console.log(a);
```

Output

```js
1. for(var i = 0; i< 6; i++) 
{
  setTimeout(function() { 
  console.log(i); 
  });
}

//Output
6
6
6
6
6
6

2.
console.log(a); 
a = 10; 
var a = 5;

//Output
undefined


3.
console.log(1);
setTimeout(() => {
  console.log(2);},0);
const promise1 = new Promise((resolve, reject) => {
console.log(3);
    resolve('success')
});
promise1.then(() => {
console.log(4);
});
console.log(5); 

//Output
1
3
5
4
2

4.const a = 5;
{
  const a = 4;
  console.log(a);
}
console.log(a);

//Output
4
5

```ts

**Type Script**
/ Suppose this is a requirement in a project, what will you do?
// CREATE AN INTERFACE NAMED ‘PERSON’ HAVING 3 PROPERTIES: fname, lname, title and 1 getter that will return the full name. CREATE 2 CLASSES NAMED ‘EMP’ & ‘CUST’ FROM THIS INTERFACE: class Emp; class Cust
// Create 1 Employee using the "Emp" class
// Create 1 Customer using the "Cust" class
  
  interface Person{
      fname:string;
      lname:string;
      title:string;
      getName():string;
  }

  class Emp{
    fname:string;
    lname:string;
    title:string;
    constructor(title:string,fname: string, lname:string,) {
        this.fname = fname;
        this.lname=lname;
        this.title =title;
    }  

    getName(): string {
        return `${this.title} ${this.fname} ${this.lname}`;
    }
  }
  

 class Customer extends Emp{
    constructor(title:string,fname: string, lname:string) {
         super(title,fname,lname);
    } 
}
    
const emp = new Emp("Mr",'Pratik','Ghule');
const cust = new Customer ("Mr",'Vaibhav','Iname');

console.warn("From Employee",emp.getName());
console.warn("From Customer",cust.getName());
