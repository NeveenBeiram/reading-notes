# ch2

when we creating a web page we add tags(which known as markup)to the content of the page.

* **Structural markup** which is the elements we used to describe the paragraphs and headings
* **Semantic markup** which provides extra information ,ex:where emphasis is placed in a sentence.

## headings :
there is 6 level of headings started from `<h1>` for the main heading to `<h6>`for the sixth subheading.

## paragraph :

`<p>here put the paragraph</p>`

 and the browser will show each paragraph on a new line with some space between it by default.

 ## Bold & iTalic :
 bold:

 `<p>This is how we make a word appear<b>bold.</b></p>`

italic:

 `<p>This is how we make a word appear <i>italic</i>.</p>`

## suPerscriPT & suBscriPT:

The `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power. 

The `<sub>` element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

## white space :
it used to make the code easier to read.
when two or more spaces next to each other the browser display it as one space.This is known as white space collapsing.

## line Breaks & HorizonTal rules :

`<br />`

The browser will show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag `<br />`.

`<hr />`

To create a break between themes,you can add a horizontal rule between sections using the `<hr />` tag.

## semantic markup:
elements that are not intended to affect the structure of your web pages.

`<strong>`

The use of this element indicates that its content has strong importance.

`<em>`

This element indicates emphasis that subtly changes the meaning of a sentence.

### Quotation

The `<blockquote>` element is used for longer quotes that take up an entire paragraph.

The `<q>` element is used for shorter quotes that sit within a paragraph.

### abbre Viations & acronyms :

`<abbr>` If you use an abbreviation or an acronym, then the`<abbr>`element can be used. A titleattribute on the opening tag is used to specify the full term.
```
<p><abbr title="Professor">Prof</abbr> Stephen Hawking is a theoretical physicist and    cosmologist.</p>
```
### citations &definitions:
`<cite>`can be used to indicate where the citation is from.

`<dfn>`explain some new terminology n a document,t is known as the defining instance of it.
### author details
The `<address>` element has quite a specific use: to contain contact details for the author of the page.
### changes To content
The `<ins>` element can be used to show content that has been inserted into a document, while the `<del>` element can show text that has been deleted from it.

The`<s>` element indicates something that is no longer accurate or relevant (but that should not be deleted).

# ch10

The key to understanding how CSS works is to imagine that there is an invisible box around
every HTML element.

A CSS rule contains two parts: 
* a selector (p in the example)
* a declaration(font-family:arial in the exapmle)

```
p {
 font-family: Arial;}
```

## Using External CSS
The `<link>` element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page.

`href`
This specifies the path to the
CSS file (which is often placed in a folder called css or styles).

`type`This attribute specifies the type of document being linked to.The value should be text/css.

`rel`This specifies the relationship between the HTML page and the file it is linked to.The value should be stylesheet when linking to a CSS file.

```
<link href="css/styles.css" type="text/css"
 rel="stylesheet" />
```

## using internal css 

`<style>`
You can also include CSS rules
within an HTML page by placing
them inside a `<style>` element,
which usually sits inside the
`<head>` element of the page.

```
<head>
 <title>Using Internal CSS</title>
 <style type="text/css">
 body {
 font-family: arial;
 background-color: rgb(185,179,175);}
 h1 {
 color: rgb(255,255,255);}
 </style>
</head>
```

# js book 
## ch2 

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
1. ASSIGN A
VALUE TO A VARIABLE
`var color='red;` 
10. USE TWO OR
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

# ch4 
## evaluating condition and conditional statements

there are two components to a decision :

1. expression is evaluated which return a value 

53. conditional statement says what to do in a given situation 

## comparsion operators:evaluating condition 
`==` is equal to 

`!=`is not equal to

`===`strict equal to

`!==`strict not equal to

`>`grater than

`<`less than
`>=`greater than or equal to

`<=`less than or equal to

## structuring comparison operators :
`(score>= pass)`
## using expression with comparison operators:
`((score1 + score2)>(highsc1+highsc2)) `
## logical operator 
`((5>2)&&(3<8))`
## if statement
```
if(score>=50){
result= 'pass';
}
```
## if else statement 
```
if (score>=50){result='pass';}else{result=fail;}
```
*********

# How to Write a Git Commit Message 

If you browse the log of any random Git repository, you will probably find its commit messages are more or less a mess.
a well-crafted Git commit message is the best way to communicate context about a change to fellow developers (and indeed to their future selves).
A diff will tell you what changed, but only the commit message can properly tell you why.

## The seven rules of a great Git commit message :
1. Separate subject from body with a blank line
3. Limit the subject line to 50 characters
6. Capitalize the subject line
9. Do not end the subject line with a period
8. Use the imperative mood in the subject line
47. Wrap the body at 72 characters
87. Use the body to explain what and why vs. how.


