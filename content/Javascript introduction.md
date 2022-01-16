# Javascript introduction
<!-- #anki/deck/Programming #anki/tag/Javascript -->

Q. `Math.random();`. What relation does random have to math?
A. It is a method of Math.

Q. How do you define a variable in javascript?
A. `let MyVar = MyValue;`

Q. The logical OR operator in Javascript
A. `||`

Q. Type an if/else statement in Javascript.
A. 
``` js
if (2 > 3) {
	console.log("true");
} else {
	console.log("false");
}
```

Q. The logical AND operator in Javascript
A. `&&`

Q. Define a function in Javascript
A. 
``` js
function sum(num1, num2) {
  return num1 + num2;
}
```

Q. What is name to sayHello?
``` js
function sayHello(name) {
  return name;
}
```
A. Its parameter 

Q. How do you add an element to an array in Javascript?
A. `array.push(element);`

Q. How do you get the last element from an array in Javascript?
A. `array.pop();`

Q. How do you write a classical, 3-part for loop in Javascript? 
A.
``` js
for (let i = 0; i < 4; i += 1) {
	console.log(i);
};
```

Q. How do you most easily loop over an iterable in JS?
A.
``` js
for (item of iterable) {
	// run
} 
```

Q. How do you most easily loop through an objects properties in JS?
A.
``` js
for (property in object) {
	// run
}
```

Q. How do you access the color property of an apple object in JS?
A. 
``` js
apple["color"] or apple.color
```

Q. How do you define an object method in JS?
A. 
``` js
const object = {
	method_name(parameter_name) {
		// function code;
	},
	property: 'description'
};
```

<!-- {BearID:1CD3CE3B-5E66-4AE2-A578-377B4334247A-726-000003E22F7E913E} -->
