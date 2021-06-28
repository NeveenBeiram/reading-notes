# Context API

- Describe use cases for `useMemo()` and `useReducer()`
useMemo is a React hook: memorizes the output of a function
useReducer: is usually preferable to useState when you have complex state logic that involves multiple sub-values or when there is a state depends on another one.

- Why do custom hooks need the use prefix?
to know that its a hook not a normal function.

- What do custom hooks usually do?
extract component logic into reusable functions.

- Using any list of custom hooks, research and name one that you think will be useful in your applications.

 use-location hook
The name says it all, this hook is used for getting the location of the browser. 

- Describe how a hook that fetches API data might work.
We could abstract the logic for fetching the data into a custom hook then call that in useEffect for example on multiple pages if they all need access to data from that api call

## Term
- reducer:A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change.


## Preparation Materials

***Context:***
Context provides a way to pass data through the component tree without having to pass props down manually at every level.

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component:

```
class App extends React.Component {
  render() {
    return <Toolbar theme="dark" />;
  }
}

function Toolbar(props) {
  // The Toolbar component must take an extra "theme" prop
  // and pass it to the ThemedButton. This can become painful
  // if every single button in the app needs to know the theme
  // because it would have to be passed through all components.
  return (
    <div>
      <ThemedButton theme={props.theme} />
    </div>
  );
}

class ThemedButton extends React.Component {
  render() {
    return <Button theme={this.props.theme} />;
  }
}
```




- [context api](https://reactjs.org/docs/context.html)

- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

- [react context links](https://github.com/diegohaz/awesome-react-context)