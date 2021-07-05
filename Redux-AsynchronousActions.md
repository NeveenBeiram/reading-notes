# Redux - Asynchronous Actions

- How granular should your reducers be?
many reducers is better than only a few or just one. 
and in Redux there is combineReducers method to combine these reducers .

- Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
con

- Name a strategy for preventing the above
thunk middleware or maybe you have to be more specific when you named the reducers!.

***

## Term
- store:A store is an immutable object tree in Redux.
 the store is a state container that holds the state of the application.
  Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.

- combined reducers:helper function from redux,that takes all the reducer functions and combines them in one reducer then pass it to the store in (createStore).

***

### Preparation Materials
**Async Logic and Data Fetching**
 React-Redux library  let our React components interact with a Redux store, including calling useSelector to read Redux state, calling useDispatch to give us access to the dispatch function, and wrapping our app in a `<Provider>` component to give those hooks access to the store.

So far, all the data we've worked with has been directly inside of our React+Redux client application. However, most real applications need to work with data from a server, by making HTTP API calls to fetch and save items.

**Redux Middleware and Side Effects**
By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

Earlier, we said that Redux reducers must never contain "side effects". A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. Some common kinds of side effects are things like:

Logging a value to the console
Saving a file
Setting an async timer
Making an AJAX HTTP request
Modifying some state that exists outside of a function, or mutating arguments to a function
Generating random numbers or unique random IDs (such as` Math.random()` or `Date.now()`)

However, any real app will need to do these kinds of things somewhere. So, if we can't put side effects in reducers, where can we put them?

Redux middleware were designed to enable writing logic that has side effects.

 Redux middleware can do anything when it sees a dispatched action: log something, modify the action, delay the action, make an async call, and more. Also, since middleware form a pipeline around the real store.dispatch function, this also means that we could actually pass something that isn't a plain action object to dispatch, as long as a middleware intercepts that value and doesn't let it reach the reducers.

Middleware also have access to dispatch and getState. That means you could write some async logic in a middleware, and still have the ability to interact with the Redux store by dispatching actions.

![](https://redux.js.org/assets/images/ReduxAsyncDataFlowDiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

**Using the Redux Thunk Middleware**
As it turns out, Redux already has an official version of that "async function middleware", called the Redux "Thunk" middleware. The thunk middleware allows us to write functions that get dispatch and getState as arguments. The thunk functions can have any async logic we want inside, and that logic can dispatch actions and read the store state as needed.

Writing async logic as thunk functions allows us to reuse that logic without knowing what Redux store we're using ahead of time.



***
[async actions](https://redux.js.org/advanced/asyncactions)

[thunk middleware](https://github.com/reduxjs/redux-thunk)

[redux thunk](https://alligator.io/redux/redux-thunk/)
