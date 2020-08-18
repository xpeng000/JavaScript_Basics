## JavaScript_Basics

This document highlights the differences between Java and JavaScript. This would hopefully make anyone who already knows Java but wants to learn JS easier! 

#### What’s the key difference between JS and Java?

*	Java is very powerful in that it is used in many areas, such as app development, big data applications, and etc. JS is mainly used to make website more interactive.

*	Java is more on the server side, whereas JS is more on developing the client side scripting. 

#### Why is JS useful? What role does it play in web applications?

*	It’s one of the core technologies of web development and can be used on both the front-end and the back-end. More on [CodeCademy](https://www.codecademy.com/catalog/language/javascript).

*	JS provides an interface for the end users to interact by generating dynamic content to the users, whereas HTML is static. 

#### What are JS primitives?

    string 
    number 
    boolean
    null
    undefined (It just refers to declaring a variable without giving it a value. Example: var str; )

#### Three ways to declare a variable and their differences? 
	
    var myName = “Rachel”; 
  	
    let myName = “Rachel”;
  
    const myName = “Rachel”;
  
  *Just like Java syntax, JS ends with a semi-colon and assigns with =*
  
*	var: you can use this variable through out the entire program 
	
*	let: only be used in the scope you declare it. 
  
  *You will get an error if you have to let variables with the same name in the same scope.*
 
*	const: a variable you can’t change or reassign (will get error if you change it)
  
  *most stuff we’ll do use const and let*

#### How to print out stuff on the console?
      
      console.log(“Goodbye World”);

#### Strings and index in JS?

*	get the length of a string
        
      	str.length
    
*	JS, like Java, uses *0-based index rule*. Use brakes notation to access letter in the string: 
  
     	str[0]

#### How to declare a function in JS?

*	In JS, you don’t need to specify the return type or parameter data types

*	function is the keyword to declare a function 

*	A function can also be stored in a variable, which can be used as a function later

<img width="643" alt="Screen Shot 2020-08-17 at 5 43 27 PM" src="https://user-images.githubusercontent.com/54920080/90382408-4a622280-e0b1-11ea-8333-e3acb7b7fc5c.png">

#### How to store multiple values with Arrays?

*	Unlike Java, you can store different data types in one array
  		    
        var arr = [“Rachel”, 13, true]; 

#### How to modify Arrays? 

*note that Arrays in JS = ArrayLists in Java, meaning it’s more flexible because it doesn’t have a fixed length.*

Besides from its flexibility, Arrays in JS also have more functions that are not available in Java, such as .shift() and .unshift(). 

*	.push() works like .add() in Java: it will add more elements to the Array you’re calling from

*	.pop() works like .remove() in Java: it will return the LAST element from the Array and remove it 

*	.shift() returns the FIRST element from the Array and removes it 

*	.unshift(a) will add an element at index 0 of the array

*	JSON.stringify(arr) will return the string format of the Arrays 

<img width="454" alt="Screen Shot 2020-08-17 at 5 46 27 PM" src="https://user-images.githubusercontent.com/54920080/90382628-9745f900-e0b1-11ea-96fb-88fb7a9c56f0.png">

#### How to evaluate equality in JS?

*	JS has 2 ways to compare values: == and ===

*	== is used for comparing two variables, but it ignores the datatype of variable

*	=== is used for comparing two variables, but this operator also checks datatype and compares two values

*	3 === 3 returns true while 3 === ‘3’ returns false 

*	3 == ‘3’ returns true while 3 == ‘4’ returns false

*	Similarly with equality checkmarks, inequality can be checked with != (capable of type conversion) and !== (strict comparison)

#### Switch statement?
*note that the case in the switch statement is using STRICT comparison implicitly*

*	the code will exit at “break”. So if you don’t have break, just a bunch of cases, then your code will exit when at the first break. Note that each case doesn’t need to have a break statement.  

<img width="287" alt="Screen Shot 2020-08-17 at 5 47 27 PM" src="https://user-images.githubusercontent.com/54920080/90382725-ba70a880-e0b1-11ea-8df9-e3d85c0c60cb.png">

#### What is JS Object?

*	Objects have properties and they are variables too (variables are just objects with single values)

*	JS object is a collection of named values (properties). The following is a simple example of a JS object: 

**note that this object variable is created using object literal, where we both define and create an object in ONE statement. This format is similar to JSON.** 

<img width="715" alt="Screen Shot 2020-08-17 at 5 48 15 PM" src="https://user-images.githubusercontent.com/54920080/90382811-d5dbb380-e0b1-11ea-9a44-8c95cf2bf5dc.png">

*	Another way to create a JS object is using the keyword new: 
	       
         	var newObj = new Object();
	
	then constructs the properties and values.

#### What are ways we can play with JS objects?
*	Objects are mutable! You can change values by accessing properties and adding properties with . or []. 

*	delete objectExample.firstname will delete the first name property from the object

*	.hasOwnProperty(pro) will check if an object has certain property or not

*	JS objects can also be nested:

<img width="275" alt="Screen Shot 2020-08-17 at 5 49 20 PM" src="https://user-images.githubusercontent.com/54920080/90382916-fdcb1700-e0b1-11ea-9112-b8db167d06fb.png">

*	JSON.parse(JSON.stringify(obj)) is often used to make a copy of the object before we want to modify it

#### Why do we need JS objects? What's its role in web development?

*	In JS, most things are objects, such as Arrays and browser APIs built on top of JS. JS objects are created similarily to JSON format, which makes it easy to parse and send data bewteen users and servers. 

*	In order for websites to be interactive, we need to have data, which is often stored in JSON format (key:value pair). Different websites have different data properties that we need to store by creating different JS objects. For example, as a web developer for an insurance company, you want to create a JS object to store user's income, occupation, and age, whereas for a music company, you need to create a different JS object with different properties, such as music genres.
 
#### How to simplify if-else statement using ternary operator (?) ?

*	Ternary operators can make your code more compact, but it doesn’t change the functionality or runtime.

*	These 2 functions are the same, and obviously the one with ternary operator is more compact. 

<img width="543" alt="Screen Shot 2020-08-17 at 5 51 22 PM" src="https://user-images.githubusercontent.com/54920080/90383110-45ea3980-e0b2-11ea-996a-7440faab843e.png">

#### What is and how to create anonymous function?
*	Anonymous function is a function declared without name identifier to refer to it

*	This type of functions is usually inaccessible once it is created, but it’s useful as an argument to other functions or as an immediately invoked function execution (works well with higher order functions).

*	create anonymous function with arrow heads:
        
        const magic = () => new Date() 
        
  now variable magic is assigned to a new Date object
 
*	 create anonymous function with parameters: 

<img width="549" alt="Screen Shot 2020-08-17 at 5 52 20 PM" src="https://user-images.githubusercontent.com/54920080/90383215-687c5280-e0b2-11ea-9062-59edbba8b296.png">







