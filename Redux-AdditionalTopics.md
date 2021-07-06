#  Redux - Additional Topics

- What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
`useEffect()` to dispatch the async action which load data on application start.

- When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
 The actual action from the reducer.

***

## Term
- middleware: Code between the framework receiving a request and the framework generating the response.

- thunk:
With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.

Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.

***
### Preparation Materials

Getting Started with Redux Toolkit
Purpose#
The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

"Configuring a Redux store is too complicated"
"I have to add a lot of packages to get Redux to do anything useful"
"Redux requires too much boilerplate code"
We can't solve every use case, but in the spirit of create-react-app and apollo-boost, we can try to provide some tools that abstract over the setup process and handle the most common use cases, as well as include some useful utilities that will let the user simplify their application code.

Redux Toolkit also includes a powerful data fetching and caching capability that we've dubbed "RTK Query". It's included in the package as a separate set of entry points. It's optional, but can eliminate the need to hand-write data fetching logic yourself.

These tools should be beneficial to all Redux users. Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.


**Installation**
Using Create React App:
The recommended way to start new apps with React and Redux is by using the official Redux+JS template or Redux+TS template for Create React App, which takes advantage of Redux Toolkit and React Redux's integration with React components.

```
# Redux + Plain JS template
npx create-react-app my-app --template redux

# Redux + TypeScript template
npx create-react-app my-app --template redux-typescript

```


***

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

[Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

**Alternative State Managers**

[MobX](https://mobx.js.org/getting-started.html)

[HookState](https://hookstate.js.org/)