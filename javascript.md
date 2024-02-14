
## Beginner to Intermidiate:

* Primitive datatypes in javascript? 
string, number, bigint, boolean, undefined, symbol, and null. All primitives are immutable, i.e., they cannot be altered.

* How do you find the datatype of one variable during runtime?

typeof <VARIABLE_NAME>

var names = ['Arun', 'James', 'David'];

* what is the datatype of variable 'names'? 
		
	console.log(typeof names); // 'Object' is an answer
	
* What is undefined and not defined?

Whenever we declare a variable without assigning any value to it, javascript implicitly assigns its value as undefined. 

let name;
console.log(name); //undefined

A not defined is a variable which is not declared at a given point of time with declaration keyword like var, let or const.

* What is event bubling and even capturing?

* How do you bind an event during the capturing time?

* Difference b/w == and ===

Abstract Equality Comparison (==) => Converts both left/right hand values into string and compare. 3 == '3' will be true.
Strict Equality Comparison (===) It chaecks the data type too.  3 == '3' will be false. '3' === '3' will be true.

* What is callbacks?
A callback is a function passed as an argument to another function and passed function will be executed later sometime.



Intermidiate to Advanced:

* Variable hoisting and function hoisting?

function foo1() {
	console.log(a);
	var a = 10;
	console.log(a);
}

function foo2() {
	console.log(a);
	a = 10;
	console.log(a);
}

foo1();
foo2();


* How do you handle errors in javascript?

* Different variable scopes in javascript? 
	funtion scope, global scope and block scope.
	
* Difference b/w var, let and const?

* What are the ways to create objects in Javascript?

* How do you find, whether a particular property is present in the object or not? Name the inbuild function name.

* What is javascript closure? Write example code. 

* What is use of call, apply, and bind methods? What is the relation with "this" keyword?

* How do you achive the inheritance in javascript? (using prototype is an answer. For more experienced person we can ask to write an example)

* How do you add one or more elements in an array? (Ex. names array declared top) Add new name "Kim" b/w "James" and "David"? 
	// Push will not work. names[2] = 'Kim' will not work.
	// names.splice(2, 0, 'Kim'); // Correct answer.
	// Expected output => ['Arun', 'James', 'Kim', 'David']
	
* Sort the below array in descending order?
	var numbers = [4, 6, 5, 8, 3];
	
* For more experienced person, we can ask them sort the array of strings in a descending order.
	var names = ["b", "g", "d", "a", "c", "f", "e"];
	
* Can you name few higher-order functions in javascript?

* What are all new additions to the ES6?
	* spread operator
	* object de-structuring
	* Nullish coalescing operator '??'
	* Arrow functions - this keyword difference
	* Optional chaining '?'
	
* Template literals in javascript?

* What is Function Expression vs Function Declaration?



var students = [
	{
		"name": "alex",
		"age": 15,
		"city": "Chennai",
		"subjects": ["English", "Maths"]
	},
	{
		"name": "david",
		"age": 14,
		"city": "Mumbai",
		"subjects": ["Maths", "Physics"]
	},
	{
		"name": "ben",
		"age": 16,
		"city": "Mumbai",
		"subjects": ["English", "Maths", "Chemistry"]
	},
	{
		"name": "Chris",
		"age": 15,
		"city": "Kolkatta",
		"subjects": ["English"]
	},
	{
		"name": "Frank",
		"age": 14,
		"city": "Kochi",
		"subjects": ["Physics", "Chemistry"]
	},
	{
		"name": "Tom",
		"age": 12,
		"city": "Delhi",
		"subjects": ["English", "Chemistry"]
	}
]


Angular:

How does angular app bootstrap?
Lifecycle hooks?
NgModule meta data?
What is component?
structural directives?
Data binding? Tell me different type of data binding? (Property binding, Attribute, class, and style binding, and Event binding etc.)
What is string interpolation?
What is Lazy loading and how Angular is doing lazy loading technique? 
Different routing startegies in angular?
Wild card routing?
Router outlet?
What is pipe? difference b/w pure pipe and impure pipe?
What are the different kind of forms in Angular? (tempalte driven and reactive forms)
Difference b/w Promise vs Observable?
Subject vs BehaviourSubject?
What is decorators? And different type of decorators?
	Class Decorators
	Property Decorators
	Method Decorators
	Parameter Decorators
What is dependency injection?



HTML:

What is semantic tags?
What is block element and an inline element?
What is standalone tags? Example please?
What is the purpose of using alternative texts in images?
Explain The Key Differences Between LocalStorage And SessionStorage Objects.



CSS

What is box modal
CSS specificity
scss processor 
mixin
BEM
Flex box and how it works?

grid

z-index technics.
Web Accessbility. Other than aria attributes? Any other techniques? 
	tab-index
	Alt attributes for image

!important keyword in CSS

what is diff b/w not adding alt attribute at all and setting empty string?

.el.el.el {}

.my-class.my-class {}


Angular

Pure/impure pipes
Angular optimization techniques


add() {


}

var sum1 = add(1, 3);
var sum2 = add(1)(3);

console.log(sum1 === sum2 && sum2 === 4);?




function foo() {
    console.log('Above>>>', x, y, z);
	if(true) {
	  let x = 100;
	  var y = 200;
	  z = 300
	  console.log('Inside>>>', x, y, z);
	}
	console.log('after if block>>>', x, y, z);
}
console.log('after function>>>', x, y, z);
foo();
