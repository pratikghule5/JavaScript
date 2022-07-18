##JavaScript Snippets

#Revere String program in Java Script

``` js
function reverseString(str){
  var reverseStr = '';
for(var i = str.length - 1; i >= 0; i--){
 reverseStr += str.charAt(i);
}
console.log(reverseStr);
return reverseStr;
}
console.log(reverseString("pratik"));
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
var name="pratik";
var rev='';

for(var i=name.length-1;i>=length;i--){
   rev+= name[i]
}
console.log(rev);
```

```js
for(var i = 0; i< 6; i++) 
{
  setTimeout(function() { 
  console.log(i); 
  });
}
           
```js
console.log(a); 
a = 10; 
var a = 5;
```

let a = [1,3,5,7,8,9,11];
let b = [0, 1, 3];

// a = [1,5,8,11]
// a.pop(0);
var j=0;
for(var i=0;i<b.length;i++){
  // console.log(b[i]);
  
  a.splice(b[i] - j,1);
  // a.indexOf(11);
  // a.remove(b[i])
  // console.log(a);
// a.shift(b[i]);
  j =j+1;
}

 console.log(a);


```js
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

```
