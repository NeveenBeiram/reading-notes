# Routing

- Do child components have direct access to props/state from the parent?
No.
have access to state from the parent (this.state) when in a class, and have access to props as a functional component.

- When a component “wraps” another component, how does the child component’s output get rendered?
props.children 

```
<Main>
  <Content />
</Main>
```

- Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application? 
No,standalone components have no parents to get props from or children to pass props to.

- What trick can a parent use to share all props with it’s children
pass all the props with the spread operator:
 `<ChildComponent {...props}>`
***
## Term
- props.children:
its used to display whatever you include between the opening and closing tags 

- composition:
Creating a unique component from a generic/reusable component

***

### Preparation Materials
***A Simple React Router v4 Tutorial***
React Router v4 is a pure React rewrite of the popular React package. Previous versions of React Router used configuration disguised as pseudo-components and could be difficult to understand

Installation:
React Router has been broken into three packages: react-router, react-router-dom, and react-router-native.

We are building a website, so we will install react-router-dom.

`npm install --save react-router-dom`

The Router
When starting a new project, you need to determine which type of router to use. For browser based projects, there are `<BrowserRouter>` and `<HashRouter>` components.
The `<BrowserRouter>` should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI), while the `<HashRouter>` should be used for static websites (where the server can only respond to requests for files that it knows about).

Usually it is preferable to use a `<BrowserRouter>`, but if your website will be hosted on a server that only serves static files, then the `<HashRouter>` is a good solution.

***

[browser router tutorial](https://blog.pshrmn.com/entry/simple-react-router-v4-tutorial/)

[browser router api docs](https://reacttraining.com/react-router/web/api)
### Bookmark
[react-if component](https://www.npmjs.com/package/react-if)

[react testing library queries](https://testing-library.com/docs/dom-testing-library/api-queries)

[aria roles](https://www.w3.org/TR/html-aria/)