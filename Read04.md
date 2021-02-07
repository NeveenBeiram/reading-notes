# JavaScript 
### *JavaScript* used in browser to make the website more :

*	interesting 
* 	user friendly 
* interactive by accessing and modifying the content and markup used in a web page while it is being viewed in the browser 

### How  javascript makes web pages more interactive?

1.	access content
by select any element  from HTML page
example :
•	select the text inside all of the `<h1>` element 
•	select any elements have a class attribute with a value of note 
•	find out what was entered into a text input 


2.	modify content 
by adding elements 
example :
•	add paragraph of text after the first `<h1>` element 
•	change the value of class attribute to trigger new css rules for those elments
•	change the size or position of an `<img>` element 

3.  program rules 
You can specify a set of steps for the browser to follow which allows it to access or change the content of page 
Example:
•	gallery script could check which image a user clicked 
•	mortgage calculator collect values from a form do calculation 
•	an animation check the dimension of the browser window and move an image to the bottom of the viewable area

4- peact to events
Script should run when a specific event has occurred 
Example it could be run when :
•	Abutton is pressed 
•	A link is clicked 
•	A cursor hovers over an element 
•	Information is added to a form 
***
#### EXAMPLES OF JAVASCRIPT IN THE BROWSER

Being able to change the content of an HTML page while it is loaded in
the browser is very powerful

•	SLIDESHOWS

•	FORMS

•	RELOAD PART OF PAG

•	FILTERING DATA

***

***What Is a script and how to create it ?***


A script is a series of instructions that computer follow to achieve a goal 
Computer follow the script step by step 


Browser may use different parts of the script depending on how the user interacts with the web page 

Scripts run can run different sections of the code in response of the situation around them 
***
### Writing a script 

  to write a script , you need to state your goal at the beginning then listing the tasks that need to be completed in order to achieve it.

You have to start with the big picture of what you want to achieve,and break that down into smaller steps:
1.	Define the goal
2.	Design the script
3.	Code each step
Designing a script tasks:
Once you know the goal of your script, you can work out the individual tasks needed to achieve it. This high-level view of the tasks can be represented using a flowchart 


![image](https://jquery-plugins.net/image/plugin/flowchartjs-svg-flow-chart-diagrams-with-javascript.png)

***
### From steps to code 
Every step for every task shown in flowchart needs to be written in a language the computer can understand and follow 


Sketching out the  tasks in a flowchart 
Often script will need to perform different tasks in different situation .
You can use flowcharts to work out how the tasks fit together.the flowcharts show the paths between each step 
***
### Experssions 
An expression evaluates into (results in) a single value. there are two types of expressions :

1 expression that just assign a value to a variable `var color = ‘beige’ ;`
2 expression that use two or more value to return a single value `var area =3 * 2 ;`
***

### Operators :
 Expression rely on things called operators; they allow programmers to create a single value from one or more values 

* Assignment operators 

`color = beige ;`

* Arithmetic operators 

`area = 3 * 2 ;`

* String operators 

`greeting = ‘hi ’ + ‘molly ’ ;`

* Comparison operators 

`buy = 3> 5 ;`

* Logical operators 

`buy = (5 > 3) && (2 < 4)`


### ARITHMETIC OPERATORS
ORDER OF EXECUTION Several arithmetic operations can be performed in one expression, but it is important to understand how the result will be calculated. 

Multiplication and division are performed before addition or subtraction.
This can affect the number that you expect to see. To illustrate this effect

### STRING OPERATOR
There is just one string operator: the + symbol.
It is used to join the strings on either side of it.

There are many occasions where you may need to join two or more strings to create a single value. Programmers call the process of joining together two or more strings to create one new string concatenation.

### MIXING NUMBERS AND STRINGS TOGETHER

**If you try to add a numeric data type to a string, then the number becomes part of the string WHAT IS A FUNCTION?**

functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).

### Declaring a function 

To creat a function, you give it a name and then write the statement needed to achieve its task inside the curly braces 

```
function sayHello() {
document.write(‘hello!’);
}
```

**Calling a function**

`sayHello();`


**Declearing functions that need information**


```
Function getArea(width,height){
Return width * height ;
}
```
**Calling function that need information**

`getArea (3 , 5);`

**Getting a single value out of a function**
 
```
Function calculateArea (width,height){
Var area = width * height ;
Return area ;
}
```
