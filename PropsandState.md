# Props and State

* Does a deployed React application require a server?
We don’t necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.

* Why do we prefer to test a React application at the behavior rather than the unit level?
 It's in front-end side.
 Because React is not like a function that gives a simple output, there is a visual aspect involved

* What does npm run build do?
When you're ready to deploy to production, running npm run build will create an optimized build of your app in the build folder

* Describe the actual composition / architecture of a React application
The key feature of React is composition of components. Components written by different people should work well together. It is important to us that you can add functionality to a component without causing rippling changes throughout the codebase.

## Term
* BDD:Behavior Driven Development.
* Acceptance Tests:testing technique performed to determine whether or not the software system has met the requirement specifications.
* mounting:In react, it is the process of outputting the virtual representation of a component into the final UI representation
* build:create a production build of your app in the build/ folder of your project.


### Preparation Materials
***setState***
Update to a component state should be done using `setState()`
You can pass an object or a function to setState().
Pass a function when you can to update state multiple times.


***Handling events*** with React elements is very similar to handling events on DOM elements
There are some syntax differences;React events are named using camelCase rather than just lowercase, and with JSX you pass a function as the event handler rather than a string.
you must call preventDefault explicitly

***forms***
HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state
In HTML, form elements such as input, textarea, and select typically maintain their own state and update it based on user input
In React, mutable state is typically kept in the state property of components, and only updated with setState()
***

[setState explained](https://css-tricks.com/understanding-react-setstate/)

[handling events](https://facebook.github.io/react/docs/handling-events.html)

[forms](https://facebook.github.io/react/docs/forms.html)

[state and lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)

[components and props](https://facebook.github.io/react/docs/components-and-props.html)

[React Testing Library](https://testing-library.com/docs/react-testing-library)

[RTL Testing Example](https://thomlom.dev/beginner-guide-testing-react-apps/)

### Bookmark

[Roles Reference](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques#Roles)