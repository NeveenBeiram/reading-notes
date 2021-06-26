# Hooks API

- Why do we not need more .html pages in a multi-page React app?
JavaScript libraries (most notably react-router-dom) allow the developer to register URLs—and their corresponding components—in one of the parent nodes of the DOM tree. Then, depending on the URL entered, certain nodes are rendered to the DOM, and others are not.[source](https://rapidapi.com/blog/react-multi-page-app/)

- If we wanted a component to show up on every page, where would we put it and why?
Outside the `<BrowserRouter/>`
Inside the `<BrowserRouter />`, outside a `<Route />`
Inside a `<Route />`?

Inside the `<BrowserRouter />`, outside a `<Route />`
 because it needs to be included in the `<BrowserRouter />`, because its holds everything, but outside the `<Route/>` so that component will show up on every page.


- What does props.children contain?
you can use `props.children` on components that represent ‘generic boxes’ and that don’t know their children ahead of time.
 `this.props.children` it is used to display whatever you include between the opening and closing tags when invoking a component.

```
 const Picture = (props) => {
  return (
    <div>
      <img src={props.src}/>
      {props.children}
    </div>
  )
}
```
This component contains an `<img>` that is receiving some props and then it is displaying `{props.children}`.

Whenever this component is invoked `{props.children}` will also be displayed and this is just a reference to what is between the opening and closing tags of the component.
[source](https://stackoverflow.com/questions/49706823/what-is-this-props-children-and-when-you-should-use-it)


*** 

## Term
- Composition:React Composition is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop.[source](https://formidable.com/blog/2021/react-composition/)

- Children / Child Components:components that are nested within a parent React component.

- Hash Routing:Using the anchor part of the URL to simulate different content.

- Link Routing:Provides declarative, accessible navigation around your application.

***

### Preparation Materials
If the React community embraces the Hooks proposal, it will reduce the number of concepts you need to juggle when writing React applications. Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.

Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

Hooks API Reference:
- Basic Hooks

    - useState
    - useEffect
    - useContext

- Additional Hooks

    - useReducer
    - useCallback
    - useMemo
    - useRef
    - useImperativeHandle
    - useLayoutEffect
    - useDebugValue

What does useEffect do? By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

Why is useEffect called inside a component? Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

Does useEffect run after every render? Yes! By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.


***

[making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

[the state hook](https://reactjs.org/docs/hooks-state.html)

[hooks api](https://reactjs.org/docs/hooks-overview.html)

[hooks api reference](https://reactjs.org/docs/hooks-reference.html)

[effects hook](https://reactjs.org/docs/hooks-effect.html)