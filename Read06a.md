# what is a function ?

function let you group a series of statements together to performed a specific task.

if different parts of a script repeat the same tasks, you can reuse the function rather than repeating the same set of statements.

The statements in a function are not always executed when a page loads, so functions also offer away to store the steps needed to achieve a task.

* when you ask the function to performed its task, it is known as calling the function.
     
     `firstName();`

some function need to be provided with information in order to achieve a given task. the information which passed to a function are known as parameters. such as width and height in calculate the area function
  
  ` calculateArea(width,height);`

* when you write a function and you expect it to provide you with an answer the response is known as return value
Declaring a function

to create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces.

```
function sayHello(){
    document.Write('hello');
}
```

# calling a function

after declared the function, you can then execute all of the statements between its curly braces with just one line of code

`sayHello();`

# declaring function that need information

parameters act like variables.

```
function getArea(width,height){
    return width * height;
}
```

# calling functions that need information

`getArea(3 ,5);`

# getting a single value out of a function

```
function calculateArea(width,height){
    var area = width * height ;
    return area;
}```
