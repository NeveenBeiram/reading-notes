## Comparison operators :

***Evaluating conditions***

You can evaluate a situation by comparing one value in the script to what you expect it might be.

**The result** will be Boolean :
* True 
* False 

1.	`== `  is equal to 

To compares two values (numbers,string ,or booleans)to see if they are the same

 2. `!=` is not equal to 

           To compare two values to see if they are the same 

5. `===` strict equal to 

Compare two values to check that both the data type and value are the same 

9. `!==` strict not equal to

Compare two values to check that both data type and value are not the same 

***
-	`>` greater than 

Check the number on the left is grater than the number on the right 

-	`<` less than 

Check if the number on the left is less than the number on the right 

-	`>=` greater than or equal to 

Check if the number on the left is greater than or equal to the number on the right 

-	`<=`less than or equal to 

Check if the number on the left is less than or equal to the number on the right 

## Logical operators 

comparing operators usually return single values of true or false.

Logical operator allow you to compare the result of more than one comparison operator 

```
((5 <3)&& (2<=3))
``` 

`&&` **logical and** 

Tests more than one condition 

`||` **logical or**
 
Test at least one condition 

```
((2<5)||(2<1))
```

`!` **logical not**


```
!(2<1)
```


# loops

Loops check a condition .

If it return true , a code block will run  Then the condition will be checked again and if it still returns true,the code block will run again It repeats until the condition returns false.

•	For 

If we want to run code specific number of times use for loop 

```
For (var i=0;i<10;i++){
Document.write(i);
}
```

•	While

If we do not know how many times the code should run
The condition can be something other than a counter 

•	Do while

The do while is similar to the while loop but the different is the do while will run the statement inside the curly braces at least once even if the condition evaluate to false 

***
## Loop counters

A for loop uses a counter as a condition it is instructs the code to run a specified number of  times. 

Condition is made up of three statements :

*  **Initialization**

    `var I =0;`

*  **condition**

   `i<10;`

*  **update** 

    `i++`


```
For(var I =0; i<10;I ++){
Document.write(i);
}
```

## Using while loop :

```
Var i=1;
Var msg=’’;
While(i<10){
Msg + = I + ‘* 5 =’ +(i*5)’+ ‘<br />’;
I++;
}
Document.getElementById(`answer`).innerHTML = msg;
```
Here is a while loop. It write out the **5 times table**.each time the loop is run, another calculation is written into the variable called msg.


***This loop will continue to run*** for as **long** as the condition in the parentheses is true. That condition is a counter indicating that, as long as the variable `i` remains less than 10, the statements in the subsequent code block should run.Inside the code block 

## there are two statements:
The first statement uses the `+=` operator, which is used to add new content to the msg variable.Each time the loop runs, a new
calculation and line break is added to the end of the message
being stored in it. So+" works as a shorthand for writing:

`msg = msg + 'new msg'`


The second statement increments the counter variable by one. (This is done inside the loop rather than with the condition.)
When the loop has finished, the interpreter goes to the next line
of code, which writes the msg variable to the page.

```
1 * 5= 5
2 x 5 = 10
3 x 5 = 15
4 x 5 = 20
5 x 5 = 25
6 x 5 = 30
7 x 5 = 35
8 x 5 = 40
9 x 5 = 45
```

In this example, the condition specifies that the code should run nine times. A more typical use of awhile loop would be when you do not know how many times you want the code to run. It should continue to run as long as a condition is met.


