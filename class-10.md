# JavaScript book, Ch. 10, “Error Handling & Debugging”

## ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.

## THE STACK 
The JavaScript interpreter processes one line of code at a time.

* When a statement has to call some other code in order to do its job, the new task goed to the top of the pile of things to do .

* once the new task has been performed , the interpreter can go back to the task in hand .

* Each time a new item is added to the stack ,it creates a new execution context.

## EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases
of activity: 

1. PREPARE 
    * The new scope is created
    *  Variables, functions, and arguments are created
    *  The value of the this keyword is determined
3. EXECUTE
    * Now it can assign values to variables
    * Reference functions and run their code
    * Execute statements

## UNDERSTANDING SCOPE

In the interpreter, each execution context has its own variables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object. 

## UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.

## Handiling Exceptions

```
try{
    // try to execute this code 
}catch(exception){
    // if there is an exception ,run this code
}finally{
    //this always gets executed 
}

```
