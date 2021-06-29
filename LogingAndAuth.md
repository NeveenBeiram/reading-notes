# Login and Auth
 `<Login />` & `<Auth />`

- Why is the Context API useful?
Context API is useful because it can help to make information globally available in the app rather than having to pass it in props to each individual child element.

- Can a component outside of a provider get its context?
No.

- What are some common use cases for using the Context API?
 Theming, Authentication

- Describe “Context Hell”
many nested contexts.

## Term
- global state: State that all component can use it.

- global context: context that is passed from the app.js component and is available to all child components.

- provider:The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree.

- consumer:A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

Requires a function as a child. The function receives the current context value and returns a React node. The value argument passed to the function will be equal to the value prop of the closest Provider for this context above in the tree. If there is no Provider for this context above, the value argument will be equal to the defaultValue that was passed to createContext().

### Preparation Materials
Learn about role-based access control (RBAC): restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

**react-cookies**

- `$ npm install react-cookies --save`

- Usage
```
import { Component } from 'react'
import cookie from 'react-cookies'
 
import LoginPanel from './LoginPanel'
import Dashboard from './Dashboard'
 
class MyApp extends Component {
  constructor () {
    super()
 
    this.onLogin = this.onLogin.bind(this)
    this.onLogout = this.onLogout.bind(this)
  }
 
  componentWillMount() {
    this.state =  { userId: cookie.load('userId') }
  }
 
  onLogin(userId) {
    this.setState({ userId })
    cookie.save('userId', userId, { path: '/' })
  }
 
  onLogout() {
    cookie.remove('userId', { path: '/' })
  }
 
  render() {
    const { userId } = this.state
 
    if (!userId) {
      return <LoginPanel onSuccess={this.onLogin} />
    }
 
    return <Dashboard userId={userId} />
  }
}
```

- `universal-cookie `- Universal cookies for JavaScript

- `universal-cookie-express` - Hook cookies get/set on Express for server-rendering

```
<script
  crossorigin
  src="https://unpkg.com/react@16/umd/react.production.js"
></script> 
<script
  crossorigin
  src="https://unpkg.com/universal-cookie@3/umd/universalCookie.min.js"
></script> 
<script
  crossorigin
  src="https://unpkg.com/react-cookie@3/umd/reactCookie.min.js"
></script> 
```

`<CookiesProvider />`
Set the user cookies

On the server, the cookies props must be set using `req.universalCookies` or `new Cookie(cookieHeader)`


- `useCookies([dependencies])`
Access and modify cookies using React hooks.
`const [cookies, setCookie, removeCookie] = useCookies(['cookie-name']);`

***

[what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

[react-cookie library](https://www.npmjs.com/package/react-cookie)