# Redux - Combined Reducers

- Why choose Redux instead of the Context API for global state?
In complex application, Redux is a easier to manage the state.

- What is the purpose of a reducer?
reducers tell the application how to change state in response to an action. 
The action does not do anything except describe what happened and it is up to the reducer to respond to this.

- What does an action contain?
type and the payload.

- Why do we need to copy the state in a reducer?
The reducer needs to be a pure function that means without any side-effects. It should only take in an action and return the new state.

***

## Term
- immutable state:State cannot be modified, reducers must make copies of existing state to make updates.

- time travel in redux:This is a feature of redux dev tools that allows you to see every state that a page has been in.

- action creator: Instead of creating action objects inline in the places where you dispatch actions, can create functions generating them. You might write an action creator into a separate file, and import it into your component.

- reducer: Functions that take current state and an action as an arguments,then return the new state as a result.

- dispatch:store holds the whole state of the application,and the only way to change the state inside it is to dispatch an action on it.

***

## Preparation Materials

The most common state shape for a Redux app is a plain Javascript object containing "slices" of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have "slice reducer" functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.

As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state.

The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by `combineReducers()` namespaces the states of each reducer under their keys as passed to `combineReducers()`

You can control state key names by using different keys for the reducers in the passed object. For example, you may call` combineReducers({ todos: myTodosReducer, counter: myCounterReducer })` for the state shape to be `{ todos, counter }.`

A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation: `combineReducers({ counter, todos })`. This is equivalent to writing `combineReducers({ counter: counter, todos: todos })`.




[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

[Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)