**1.Hoisting**

Hoisting is JS's default behavior of defining all the declarations at the top of the scope before code execution.\
One of the benefits of hoisting is that it enables us to call functions before they appear in the code.\ 
JavaScript only hoists declarations, not initializations.\

**2.Closures**

A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In other words, a closure gives you access to an outer function’s scope from an inner function. In JavaScript, closures are created every time a function is created, at function creation time.
To use a closure, define a function inside another function and expose it. To expose a function, return it or pass it to another function.
The inner function will have access to the variables in the outer function scope, even after the outer function has returned.

**3.let var const**

`const` is a signal that the identifier won't be reassigned.\ 
`let` is a signal that the variable may be reassigned, such as a counter in a loop, or a value swap in an algorithm.\
It also signals that the variable will be used only in the block it's defined in, which is not always the entire containing function.\

**4.Event bubbling and how to prevent it?**\

With bubbling, the event is first captured and handled by the innermost element and then propagated to outer elements.\
With capturing, the event is first captured by the outermost element and propagated to the inner elements.\

- prevent event bubling
-Bubbling/capturing can be stopped by `event.cancelBubble=true` (IE) or `event.stopPropagation()` for other browsers. 

**5.What is the difference between event preventDefault and event stopPropagation?**\

preventDefault() – It stops the browsers default behaviour.\
event.stopPropagation() – It prevents the event from propagating (or “bubbling up”) the DOM.\

**6. Prototype Inheritance**

The Prototypal Inheritance is a feature in javascript used to add methods and properties in objects. It is a method by which an object can inherit the properties and methods of another object. Traditionally, in order to get and set the [[Prototype]] of an object, we use Object. getPrototypeOf and Object.
```
function Person(first, last, age, eyecolor) {
  this.firstName = first;
  this.lastName = last;
  this.age = age;
  this.eyeColor = eyecolor;
}

Person.prototype.nationality = "English";

Person.prototype.name = function() {
  return this.firstName + " " + this.lastName;
};
```
**6. Advantages of using arrow functions**

Arrow functions intend to fix the problem where we need to access a property of this inside a callback.\
There are already several ways to do that: One could assign this to a variable, use bind , or use the third argument available on the Array aggregate methods.

This arrow function reduces lots of code and makes the mode more readable.\ 
Arrow function syntax automatically binds “this” to the surrounding code's context.\ 
Writing the arrow => is more flexible as compared with the writing function keyword.\

**7. Function and function expression ?**

9. Bind call and apply
Ans: https://medium.com/@rlynjb/js-interview-question-explain-function-prototype-bind-bbdaed41bd89
9. Mutability and immutability
10. What is IIFE ?
An IIFE (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined. 
An IIFE is a good way to secure the scope. You can use IIFEs to prevent global variables' definition issues, alias variables, protect private data, and avoid conflicts of using many libraries that export the same object name.

11. this keyword
12. what are the diff ways of defining an object
13. How to clone an object
14. deep copy and shallow copy
15. difference between instanceof and typeof
16. difference between undefined and not defined
17. closure and its advantages
18. How do you check if an object is an array or not?
19. difference between function and methods
20. How can we prevent modification of object in JavaScript ?
21. Write code for merge two JavaScript Object dynamically
22. What is the drawback of having private methods in a JavaScript object?
23. How to empty an array in JavaScript?
24. object.hasOwnProperty
25. Promises
26. Es6 new features
27. Destructuring
28. Singleton
29. Best way to detect undefined object property in JavaScript.
30. How to check whether a key exist in a JavaScript object or not
31. What is NaN, why do we need it, and when can it break the page?
32. Describe Object-Based inheritance in JavaScript.
33. Event binding and function binding
34. Explain why the following doesn’t work as an IIFE: function foo(){ }();.What needs to be changed to properly make it an IIFE?
Ans: https://medium.com/@rlynjb/js-interview-question-explain-why-the-following-doesn-t-work-as-an-iife-1faaf74a7d
7d
35.Can you describe the main difference between a forEach loop and a .map() loop and why you would pick one versus the other?
Ans: https://hashnode.com/post/what-is-the-difference-between-map-and-foreach-in-javascript-ciibz8ek700nuj3xtywxndnj8
36. What’s a typical use case for anonymous functions?
Ans: https://medium.com/@rlynjb/js-interview-question-what-s-a-typical-use-case-for-anonymous-functions-54cf547b2a0e
37.What’s the difference between host objects and native objects?
Ans: https://medium.com/@rlynjb/js-interview-question-what-s-the-difference-between-host-objects-and-native-objects-b395f7c5fbf1
38. Difference between: function Person(){}, var person = Person(), and var person = new Person()?
Ans: https://medium.com/@rlynjb/js-interview-question-difference-between-function-person-var-person-person-and-var-ab6eb8c9ae88
39.Difference between window load event and document DOMContentLoaded event?
Ans: https://javascript.info/onload-ondomcontentloaded
40.Create a for loop that iterates up to 100 while outputting “fizz” at multiples of 3, “buzz” at multiples of 5 and “fizzbuzz” at multiples of 3 and 5
Ans: 
for (var i = 1; i <= 100; i++) {
 var output = ‘’;
 if (i % 3 === 0) output += ‘fizz’;
 if (i % 5 === 0) output += ‘buzz’;
 output !== ‘’ ? console.log(output, i) : ‘’;
}
41. Make this work:
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]?
Ans: ???
42.What are the pros and cons of using Promises instead of callbacks?
Ans: https://digitalfortress.tech/js/promises-vs-callbacks/
43. What are the differences between ES6 class and ES5 function constructors?
Ans: https://medium.com/@muthuks/difference-between-es-5-and-es-6-e993c7ab0a70
44. What is local storage method ?
45.cache method
46.what is callback hell ?

