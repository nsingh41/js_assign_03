Closures

A closure is a function which is defined within the body of another function as a return expression. this function(closure) actually refers to varibles which are defined by its parent function or used by its own i.e. it basically remebers the environment of the variables in which they were created.

basic structure 

function f1(val1){

	var a=1
	
	return f2(){
	
	return (a+2)
	
	}
} 

f1 here is our parent function.

f2 is our another function which is defined within f1's body.

For f2 the value of a is 1 when it is  called for the first time because it does not have the value of a intially in its local scope. i.e. it remebers the value of a which is created in parent function. 

Whether the parent function is closed , it does not affect the functioning of closure function.

To initiate the parent function , its call is stored in a variable , but to activate the closure function the name of the variable in which parent function was stored is followed by the paranthesis '()' to act as a function and a value may also be passed to closure function through this calling

Example:-

division = first_value(15)

first_value(n){

var b=n

return divide(m){

return (b/m)
	
}
	
}

divison(5);



 Explanation :-
 
 here first function(first_value) is initiated which reads its functioning from its body

  second function takes the value of variable b from parent function and stores it 

  then divide function is called through division variable followed by a parameter which is passed within the paranthesis 


  ** Any function can have access to any global variables it does not matter whether this function is enclosed or not within the body of another function**


  References


https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures

http://www.w3schools.com/js/js_function_closures.asp

http://eloquentjavascript.net/Eloquent_JavaScript.pdf (page no. 50)

https://www.youtube.com/watch?v=71AtaJpJHw0