# Component Based UI

- Name 5 Javascript UI Frameworks (other than React)
Angular,Vue.js,Ember.js,Meteor,Mithril,Webix

- What’s the difference between a framework and a library?
The key difference between a library and a framework is "Inversion of Control".
 
When you call a method from a library, you are in control. But with a framework, the control is inverted: the framework calls you.
***Framework***
In a framework, all the control flow is already there and there are many predefined white spots that we should fill out with our code. A framework is normally more complex. It defines a skeleton where the application defines its own features to fill out the skeleton. In this way, your code will be called by the framework appropriately. The benefit is that developers do not need to worry about if a design is good or not, but just about implementing domain-specific functions. The framework will provide you with hooks and call-backs so that you build on it; it will then call your plugged-in code whenever it wishes, a phenomenon called Inversion of Control.
 
A framework can contain libraries. A framework will usually include many libraries to make your work easier.
***Library***
A library performs specific, well-defined operations. A library is just a collection of class definitions. The reason is it simply code reuse, in other words, gets the code that has already been written by other developers. The classes and methods normally define specific operations in a domain-specific area. For example, there are some libraries of mathematics that can let developers just call the function without redoing the implementation of how an algorithm works. A library will usually focus on a single piece of functionality that you access using an API. You call a library function, it executes some code and then the control is returned to your code.
[source](https://www.c-sharpcorner.com/UploadFile/a85b23/framework-vs-library/)

***

## Term

- Rendering: processing the code that we have written and showing the result of it.

- Templates: is a piece/block of code that is created with an overall layout to be used with other program.

- State: Describing the status of the entire of the code/program or an individual object.

***

## Preparation Materials
Hello World:
 The smallest React example looks like this:

```
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```

It displays a heading saying “Hello, world!” on the page.

```
const element = <h1>Hello, world!</h1>;
```

This funny tag syntax is neither a string nor HTML.

It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

JSX produces React “elements”.

Why JSX?
React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display.

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.


Let’s say there is a <div> somewhere in your HTML file:

<div id="root"></div>
We call this a “root” DOM node because everything inside it will be managed by React DOM.

Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

To render a React element into a root DOM node, pass both to ReactDOM.render():

```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```
***
[react hello world](https://facebook.github.io/react/docs/hello-world.html)

[introducing JSX](https://facebook.github.io/react/docs/introducing-jsx.html)

[rendering elements](https://facebook.github.io/react/docs/rendering-elements.html)

[sass cheatsheet](https://devhints.io/sass)

[react cheatsheet](https://devhints.io/react)

[another react cheatsheet](https://reactcheatsheet.com/)