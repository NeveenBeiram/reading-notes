# Understanding The Problem Domain Is The Hardest Part Of Programming

## What is the hardest thing about writing code?

There are many common answers to this question:

* Learning a new technology

* Naming things
* Testing your code

* Debugging

* Fixing bugs

* Making software maintainable
The list goes on and on.

***The real world*** is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.

**As programmers**, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it.

## **What can you do about it?**
If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

* Make the problem domain easier

   You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.
* Get better at understanding the problem domain


# Chapter 3: Object Literals 

## What is an object ?

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,variables and functions take on new names. 

* IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES 
* IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS

**example:**

```
var human ={
firstName: 'neveen',
lastName:'beiram',
age:24,
eyecolor:'brown'

}
```


# Chapter 5: Document Object Model

**The Document Object Model (DOM)** specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window. 

## ***THE DOM TREE IS A MODEL OF A WEB PAGE*** 
As a browser loads a web page, it creates a model of that page.The model is called a DOM tree, and it is stored in the browser's memory .It consists of four main types of nodes.

## **WORKING WITH THE DOM TREE**
Accessing and updating the DOM tree involves two steps:

1. Locate the node that represents the element you want to work with.
3.  Use its text content, child elements, and attributes.

## ACCESSING ELEMENTS
***DOM queries*** may return one element, or they may return a Nodelist,which is a collection of nodes.

## Methods that select individual elements 

`getElementById()` and `querySelector()` can both search an entire document and return individual elements. both use a similar syntax .

## **SELECTING AN ELEMENT FROM A NODELIST**
 
 There are two ways to select an element from a Nodelist:`The item()` method and array syntax.Both require the index number of the element you want


 Array syntax is preferred over the `item()` method because it is faster.
 example form the book: 

 ```
var elements=document.getElementsByClassName('hot');
if(element.length>=1){
    var firtItem=elements[0];
}
 ```

## *LOOPING THROUGH A NODELIST*

```
var hotl t ems = document .querySelectorAl l ('li.hot') ;
if (hot ltems.length > O) {for (var i=O; i<hotl tems.length; i++) { II Loop through each i t em
hotltems[i ] .className = 'cool';
}
}
```



