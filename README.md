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
