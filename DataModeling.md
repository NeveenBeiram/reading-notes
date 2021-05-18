# Data Modeling

## Name 3 advantages to Test Driven Development

1. Better program design and higher code quality
2. Detailed project documentation
3. TDD reduces the time required for project development

- You spend less time in the debugger.You are able to identify the errors and problems quickly.

## In what case would you need to use beforeEach() or afterEach() in a test suite?

They help to avoid repetition in tested code... especially if there is similar code across multiple tests

We use it when we want to apply something to the data before each testing and after each one.

## What is one downside of Test Driven Development

Tests show the presence of bugs in the code... but they cannot help find or solve them
Might be a slow process, because the test codes are written before the actual code
Tests change when the requirements of the features change... this means more maintenance time

## What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?

In classes each method will be defined as a prototype, meaning when you make instance of that class the prototype will not take from memory and will not be there unless you call it in the instance, whereas in constructors each method you define in it, and make new instance all the methods will be there and will take from the memory even if you do not call them.

“A prototype is a working object instance. Objects inherit directly from other objects.” “Classes inherit from classes and create subclass relationships: hierarchical class taxonomies.”

## Why REST?
Because of its flexibility.. it can handle multiple types of calls and data formats... and is able to communicate between different services written in different languages



## Term

* functional programming 
    It is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects... it is declarative rather than imperative, meaning that the application flows through pure functions... it is easier to test and predict than imperative or object oriented programming. 

* object-oriented programming (OOP)
     It is the most popular programming paradigm and is taught as the standard way to code... it relies on the concept of classes and objects... classes can contain functions (methods)... and classes can be inherited in subclasses, saving time and space in writing repeated code unnecessarily.

* class
    another way to write an objects (object template) that give us more flexibility and shortcuts to deal with objects (in fact it is a special functions and it has two syntax just like a normal function; expressions or declaration).

* super
    This keyword is used to access and call functions on an object's parent (from subclass to class). 

* this
    In the global context, it refers to the global object (window)... inside classes, it refers to the object it belongs to... inside events, it refers to the element that received the event

* Test Driven Development (TDD)
    It is a programming principle where the requirements of a feature are set, and then written as a test unit before the actual code is even written... each feature is executed this way.

* Jest
    It is a testing framework(dependance) for JavaScript that help us to test our code and build testing units in JS.

* Continuous Integration (CI)
     Is a coding philosophy and set of practices that drive development teams to implement small changes and check in code to version control repositories frequently.

* REST
    Representational state transfer is a software architectural style which uses a subset of HTTP. It is commonly used to create interactive applications that use Web services. A Web service that follows these guidelines is called RESTful.

* Data Model
     A data model is an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities.

### important links
[sql vs nosql video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
[nosql modeling techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)

[mongoose api](https://mongoosejs.com/docs/api.html#Model)
