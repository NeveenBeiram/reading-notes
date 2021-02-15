# ch3 Lists :

## HTML provides to us 3 types: 

1. ordered list `<ol>`
5. unordered list `<ul>`
7. definition list `<dl>`
  inside the `<dl>` element we put`<dt>` contain the term **and** `<dd>` contain the definistion.



****
# ch 13 Boxes :

## we saw that css treats HTML elements as if it lives in its own box .

we can set/change many properties that affect the appearance of that boxes so we will do :
 
* changing the dimenstion of boxes .
 
* creating borders around boxes.

* set margins and padding for the boxes .

* show and hide the boxes .

## box dimensions 
`width and height `

if we have div in our code 

```
div.box{
    height : 200px;
width : 150px;
}
```

### limiting width

`min-width and max-width`
page designs expand and
shrink to fit the size of the user's screen 

to do that : example from the book 

```
td.description{
    min-width:450px;
    max-width:650px;
}
```
### limiting height :
`min-height , maz-height`
the same way for it as the limiting width.

## overflowing content :
it is tells the browser what to do for the content which be in box smaller than it self 
*so* we have  : 

* `hidden` 

* `scroll`

## border,margin and padding

every box have 3 properties :
1. border
5. margin
8. padding

## white space and vertical margin 

the padding and margin very helpful in adding space between various itwms on the page .


## border width 
to control the width of a border we can enter the value in pixels or of one of this :

* thin  
* medium
* thick 

## border style 

* solid 
* dotted 
* dashed
* double
* groove 
* ridge
* inset
* outset
* hidden/none

we can change individually like : 
`border-top-style`

`border-left-style`

## border color :
can specify the color  using RGB,hex codes,css color names.
and we can also do it individually like : 

`border-bottom-color`


## shorthand border 
to change all of what we said in one property 

**this example from the book**

```
p{
    width:250px;
    border:3px dotted #0088dd;
}
```

## padding 
specify how much space we want between the content of an element and its border 

```
p{
   padding:15px; 
}
```
## margin 
to control the gap between boxes 

```
p{
    margin:13px;
}
```
## centering content 

`p{margin : auto;}`

## changing inline/block 

**display**

`inline`

`block`

`none`

## hiding boxes 
**visibility**
    
   `hidden`
     
 `visible`

## border images 

**border-image**

**stretch** stretches the image

**repeat** repeats the image 

**round** like repeat 

and it is important that the box must have boder width for the image to be shown .

## box shadow

`Horizontal offset`

`Vertical offset`

`Blur distance`

`Spread of shadow`


## rounded corner 
`border-radius`


# Duckett JS book: ch2 
A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

## comments :

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code.

This is an example from the book : 

```
/*This script displays a greeting to the user based upon the current time.
It is an example from JavaScript & jQuery book */
var today= new Date();
var hour Now = today.getHours();
var greeting;
// Create a ne1~ dat e object
II Fi nd the current hour
JI Display the appropriate greeti ng based on the current time
if (hourNow > 18) {
greet ing = 'Good evening ' ;
else if (hourNow > 12) {
greeting = 'Good afternoon';
else if (hourNow > 0) {
greeting= ' Good morning';
else {
gr eeting = 'Welcome';
}
document.write(greeting) ;
```

* multi-line comments 

```
/*  
 a
 b
 c
 */
 ```

 * single-line comment

 `//this is a comment`

 ## what is a variable?

 to store data in variable

 ```
 var width= 5;
 var height= 5;
 var Area = width * height;
 ```

 ## data types:

 * numeric 

 * string

 * boolean

## array 

An array is a special type of variable. It doesn't
just store one value; it stores a list of values.

this exapmle from the book : 

```
var colors;
colors ['white', 'black', ' custom'];
var el document.getElementByld('col ors');
el.textContent = col ors[O]; 
```

## VALUES IN ARRAYS
Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one). 

## accessing and changing values

`colors[2] ='red';`

## Expressions

* ASSIGN A
VALUE TO A VARIABLE

`var color='red;` 

* USE TWO OR
MORE VALUES TO RETURN A
SINGLE VALUE  

`var area=5*6;`

## operators 

1. ASSIGNMENT OPERATORS    

    `var color='red';`

5. ARITHMETIC OPERATORS  

   `var area=3*5;`

63. STRING OPERATORS  

    `fullName='Neveen'+'Beiram';`

8. COMPARISON OPERATORS  

    `b= 6<2;`

5. LOGICAL OPERATORS  

   `b=(5>3)&&(2<5);`

# ch 4 
## the if ..else statements 
if the condition resolves to true the first code block is executed ,if it revolves to false the second code block is run .

## using if statement 

```
var area ;
var width =5;
var height=2;
if (width>0 && height>0)
(area=width* height)
else {area=0;}
document.write(area);
```
## switch statement 

switch value : it is the variable which switch statement stats with .

## loops 
* for 
* while 
* do while 
