# Component Composition

* Can a parent component access the state of a child component?
Yes, we can access the child’s state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child’s state.
* What can be passed along in a prop variable?
 you can pass any data.
 (Any information, function, JavaScript that needs to be passed)
* How can a child component “know” the state of another component?
To obtain the state of another component, you can pass the component’s state to it’s child components as props.

*** 

## Term
- component props:Keyword in React for properties, can be any information, function, JavaScript that needs to be passed to another component. Can only be passed in one direction, from the root to its children, no way for data to be passed up.

- component state:React components have built in state object, which is where you story property values that belong to the component. When the state object changes, t he component re-renders

- application state:This can refer to the storage that keeps the state of all the components of the app inside it

*** 

### Preparation Materials

Both Inheritance and Composition, aim towards code reuse and cleaner code structure.
React recommends use of Composition over Inheritance, here is why. Everything in React is a component, and it follows a strong component based model. This is one of the primary reasons that composition is a better approach than inheritance for code reuse.

props.children
What types of content are allowed for props.children? The content passed to a component through props.children can include undefined, null, a Boolean, a number, a string, a React element, or an array of any of these types recursively. It can also be a function returning one of these types.

lifecycle of components in react
Lifecycle of Components Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.





***
[react basics recap](https://medium.freecodecamp.org/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030)

[props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

[composition vs inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)

[react testing library api example](https://testing-library.com/docs/react-testing-library/example-intro)
### Bookmark
[react-if component](https://www.npmjs.com/package/react-if)

[react-testing-library-async](https://testing-library.com/docs/dom-testing-library/api-async)