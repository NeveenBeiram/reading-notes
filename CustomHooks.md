#  Custom Hooks

- What does a component’s lifecycle refer to?

everything in React is consist of either components or a part of the components.
These components are subjected to follow a certain lifecycle, almost like that of any living creature on earth. They take birth, grow, and then die at last. The phase when they are born is called mounting, when they grow is called updating, and the last phase of death is known as unmounting.
This whole process is called ‘Component Lifecycle’.[source](https://medium.com/habilelabs/what-are-component-lifecycle-methods-in-react-js-5269aaa37046)

- Why do you sometimes need to “wrap” functions in `useCallback` when called from within `useEffect`
useCallback will return a memoized version of the callback that only changes if one of the dependencies has changed. This is useful when passing callbacks to optimized child components that rely on reference equality to prevent unnecessary renders [source](https://reactjs.org/docs/hooks-reference.html#usecallback)

- Why are functional components preferred over class components?
functional components easer to read and presentational.

- What is wrong with the following code?
useEffect is used inside a for loop, and it's not used at the top level of the function

```
 function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

*** 
## Term

- state hook:useState is a Hook. We call it inside a function component to add some local state to it. React will preserve this state between re-renders. useState returns a pair: the current state value and a function that lets you update it.[resource](https://reactjs.org/docs/hooks-overview.html)

- effect hook:useEffect, adds the ability to perform side effects from a function component. It serves the same purpose as `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` in React classes, but unified into a single API. 

- reducer hook:useReducer is a React hook that helps us manage a state object via reducers.
```
const [state, dispatch] = useReducer(reducerFunction, initialState);
```
It returns:
a state object that you can bind your components to.
a dispatch function that you can send actions to.[source](https://rajeshnaroth.medium.com/why-use-reducer-hooks-for-state-management-in-react-c9528f615ddf)

***

### Preparation Materials


useReducer

```
const [state, dispatch] = useReducer(reducer, initialArg, init);
```
An alternative to useState. Accepts a reducer of type `(state, action) => newState`, and returns the current state paired with a dispatch method. 

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.


Building Your Own Hooks:
Building your own Hooks lets you extract component logic into reusable functions.

When we were learning about using the Effect Hook, we saw this component from a chat application that displays a message indicating whether a friend is online or offline:

```
import React, { useState, useEffect } from 'react';

function FriendStatus(props) {
  const [isOnline, setIsOnline] = useState(null);
  useEffect(() => {
    function handleStatusChange(status) {
      setIsOnline(status.isOnline);
    }
    ChatAPI.subscribeToFriendStatus(props.friend.id, handleStatusChange);
    return () => {
      ChatAPI.unsubscribeFromFriendStatus(props.friend.id, handleStatusChange);
    };
  });

  if (isOnline === null) {
    return 'Loading...';
  }
  return isOnline ? 'Online' : 'Offline';
}
```
1. useArray hook
Array manipulation is what a dev goes through every weekday. Adding elements to an array or removing an element at a given index is a daily routine for us. useArray reduces this burden by providing us with various array manipulation methods. This hook is a part of the react-hanger package.

2. react-use-form-state hook
Forms are everywhere, even in the smallest of applications we have to encounter forms and manage their state. Managing form state in React can be a bit unwieldy sometimes.
react-use-form-state is a small React Hook that attempts to simplify managing form state, using the native form input elements you are familiar with.

3. react-fetch-hook
Making ajax calls is like the most basic and most performed task for a frontend developer. And the React community is quick enough to create a hook for this purpose too.

4. useMedia hook
useMedia is a React sensor hook that tracks the state of a CSS media query. We all know the importance of the media queries and how much important is responsiveness for any site.

5. react-useportal hook
React Portals provide a first-class way to render children into a DOM node that exists outside the DOM hierarchy of the parent component. And this hook helps us do that.

6. react-firebase-hooks
We all appreciate the greatness of firebase and use it a lot in our projects, whether its for authentication or storage. And this hook is the one we really need.

7. use-onClickOutside hook
An outside click is a way to know if the user clicks everything but a specific component. You may have seen this behavior when opening a dropdown menu or a modal or a dropdown list.

8. useIntersectionObserver hook
A React hook for using intersection observers.
The Intersection Observer API provides a way to asynchronously observe changes in the intersection of a target element with an ancestor element or with a top-level document’s viewport.

9. use-location hook
The name says it all, this hook is used for getting the location of the browser.

10. use-redux hook
This one is for my redux readers. This hook returns the store and dispatch property.














***
- Authoring

[custom hooks - all you need to know](https://www.telerik.com/blogs/everything-you-need-to-create-a-custom-react-hook)

[async hooks](https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g)

[useReducer Hook](https://reactjs.org/docs/hooks-reference.html#usereducer)

[react custom hooks](https://reactjs.org/docs/hooks-custom.html)

- Hooks Lists/Collections

[use hooks](https://usehooks.com/)

[hooks list](https://github.com/rehooks/awesome-react-hooks)

[10 essential react hooks](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)