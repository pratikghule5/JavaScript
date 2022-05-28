##JavaScript Snippets

#Revere String program in Java Script

``` javascript
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

```javascript
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

```javascript
var numbers = [1, 2, 3, 4];
var colors = ["red", "green", "blue", "purple"];


for(let i=0;i<numbers.length;i++){
  var style= "style='color:"+colors[i]+"'";
  document.write("<h1 "+style+">"+numbers[i]+"</h1>");
}

```

```javascript
var name="pratik";
var rev='';

for(var i=name.length-1;i>=length;i--){
   rev+= name[i]
}
console.log(rev);
```

```javascript
for(var i = 0; i< 6; i++) 
{
  setTimeout(function() { 
  console.log(i); 
  });
}
           
```javascript
console.log(a); 
a = 10; 
var a = 5;
```


```
