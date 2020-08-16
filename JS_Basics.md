## JavaScript_Basics

This document highlights the differences between Java and JavaScript. This would hopefully make anyone who already knows Java but wants to learn JS easier! 

#### What’s the key difference between JS and Java?


#### Why is JS useful? What role does it play in web applications?

#### What are JS primitives?
	⁃	String 
	⁃	Number 
	⁃	Boolean
	⁃	Null
	⁃	Undefined 

#### Three ways to declare a variable and their differences? 
	
    var myName = “Rachel”; 
  	
    let myName = “Rachel”;
  
    const myName = “Rachel”;
  
  **Just like Java syntax, JS ends with a semi-colon and assigns with =**
	⁃	var: you can use this variable through out the entire program 
	⁃	let: only be used in the scope you declare it. 
  **You will get an error if you have to let variables with the same name in the same scope.**
	⁃	const: a variable you can’t change or reassign (will get error if you change it)
  *most stuff we’ll do use const and let*

#### How to print out stuff on the console?
      
      console.log(“Goodbye World”);

#### Strings and index in JS?
	⁃	get the length of a string
        
      str.length
     
  ⁃	JS, like Java, uses *0-based index rule*. Use brakes notation to access letter in the string: 
  
      str[0]

#### How to declare a function in JS?

⁃	In JS, you don’t need to specify the return type or parameter data types
⁃	function is the keyword to declare a function 
⁃	A function can also be stored in a variable, which can be used as a function later


#### How to store multiple values with Arrays?

⁃	Unlike Java, you can store different data types in one array
  		    
      var arr = [“Rachel”, 13, true]; 

#### How to modify Arrays? 

**note that Arrays in JS = ArrayLists in Java, meaning it’s more flexible because it doesn’t have a fixed length.** 

Besides from its flexibility, Arrays in JS also have more functions that are not available in Java, such as .shift() and .unshift(). 

⁃	.push() works like .add() in Java: it will add more elements to the Array you’re calling from
⁃	.pop() works like .remove() in Java: it will return the LAST element from the Array and remove it 
⁃	.shift() returns the FIRST element from the Array and removes it 
⁃	.unshift(a) will add an element at index 0 of the array
⁃	JSON.stringify(arr) will return the string format of the Arrays 


#### How to evaluate equality in JS?

⁃	JS has 2 ways to compare values: == and ===
⁃	== is used for comparing two variables, but it ignores the datatype of variable
⁃	=== is used for comparing two variables, but this operator also checks datatype and compares two values
⁃	3 === 3 returns true while 3 === ‘3’ returns false 
⁃	3 == ‘3’ returns true while 3 == ‘4’ returns false
⁃	Similarly with equality checkmarks, inequality can be checked with != (capable of type conversion) and !== (strict comparison)

#### Switch statement?
**note that the case in the switch statement is using STRICT comparison implicitly**

⁃	the code will exit at “break”. So if you don’t have break, just a bunch of cases, then your code will exit when at the first break. Note that each case doesn’t need to have a break statement.  

#### What is JS Object?
⁃	Objects have properties and they are variables too (variables are just objects with single values)
⁃	JS object is a collection of named values (properties). The following is a simple example of a JS object: 
**note that this object variable is created using object literal, where we both define and create an object in ONE statement. This format is similar to JSON.** 
⁃	Another way to create a JS object is using the keyword new: 
	       
         var newObj = new Object();
	
then constructs the properties and values.

#### What are ways we can play with JS objects?
	⁃	Objects are mutable! You can change values by accessing properties and adding properties with . or []. 
	⁃	delete objectExample.firstname will delete the first name property from the object
	⁃	.hasOwnProperty(pro) will check if an object has certain property or not
	⁃	JS objects can also be nested:
	⁃	JSON.parse(JSON.stringify(obj)) is often used to make a copy of the object before we want to modify it

#### How to simplify if-else statement using ternary operator (?) ?
	⁃	Ternary operators can make your code more compact, but it doesn’t change the functionality or runtime.
	⁃	These 2 functions are the same, and obviously the one with ternary operator is more compact. 


#### What is and how to create anonymous function?
	⁃	Anonymous function is a function declared without name identifier to refer to it
	⁃	This type of functions is usually inaccessible once it is created, but it’s useful as an argument to other functions or as an immediately invoked function execution (works well with higher order functions).
	⁃	create anonymous function with arrow heads:
        
        const magic = () => new Date() 
        
  now variable magic is assigned to a new Date object
 
  ⁃	 create anonymous function with parameters: 


Work on tomorrow: 
JS functions
JS Array methods, sorting, iterations (higher order function (filter, map))






