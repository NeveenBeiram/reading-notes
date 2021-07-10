# React Native

- Compare and Contrast Redux Toolkit with Redux “Ducks”
Ducks is essentially a proposal for bundling reducers, action types, and actions all into the same file.[source](https://medium.com/swlh/the-good-the-bad-of-react-redux-and-why-ducks-might-be-the-solution-1567d5bdc698)

Redux Toolkit's it's helps to simplify common Redux use cases. It is not intended to be a complete solution for everything you might want to do with Redux, but it should make a lot of Redux-related code you need to write a lot simpler. Redux Toolkit exports several individual functions that you can use in your application, and adds in dependencies on some other packages that are commonly used with Redux.


- What is the principle advantage of Redux Toolkit
Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code[source](https://redux.js.org/redux-toolkit/overview)

***

## Term

- redux toolkit slices:(It is a reducer for one state)Redux slice is a collection of reducer logic and actions for a single feature of application.
Redux state is typically organized into slices, defined by the reducers that are passed to combineReducers.

- namespace:(we use it in socket.io!)
Namespace refers to the programming paradigm of providing scope to the identifiers (names of types, functions, variables, etc) to prevent collisions between them. For instance, the same variable name might be required in a program in different contexts. Using namespaces in such a scenario will isolate these contexts such that the same identifier can be used in different namespaces. In this article, we will discuss how namespaces can be initialized and used in JavaScript. JavaScript does not provide namespace by default. However, we can replicate this functionality by making a global object which can contain all functions and variables.[source](https://www.geeksforgeeks.org/javascript-namespace/)

***

### Preparation Materials


React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code.


React Native is like React, but it uses native components instead of web components as building blocks. So to understand the basic structure of a React Native app, you need to understand some of the basic React concepts, like JSX, components, state, and props. If you already know React, you still need to learn some React-Native-specific stuff, like the native components.

```
import React from 'react';
import { Text, View } from 'react-native';

const HelloWorldApp = () => {
  return (
    <View
      style={{
        flex: 1,
        justifyContent: "center",
        alignItems: "center"
      }}>
      <Text>Hello, world!</Text>
    </View>
  )
}
export default HelloWorldApp;
```
***What's going on here?***

First of all, we need to import React to be able to use JSX, which will then be transformed to the native components of each platform.
On line 2, we import the Text and View components from react-native

Then we find the HelloWorldApp function, which is a functional component and behaves in the same way as in React for the web. This function returns a View component with some styles and aText as its child.

The Text component allows us to render a text, while the View component renders a container. This container has several styles applied, let's analyze what each one is doing.

The first style that we find is flex: 1, the flex prop will define how your items are going to "fill" over the available space along your main axis. Since we only have one container, it will take all the available space of the parent component. In this case, it is the only component, so it will take all the available screen space.

The following style is justifyContent: "center". This aligns children of a container in the center of the container's main axis. Finally, we have alignItems: "center", which aligns children of a container in the center of the container's cross axis.

***

***Introduction to Expo***

Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.

```
install the command line tools
npm install --global expo-cli
create new project:
expo init my-project
```
***
ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project -- one that you would normally create using Xcode, Android Studio, or react-native init.


***

[getting started with react native](https://facebook.github.io/react-native/docs/getting-started)

[react native basics (Tutorial)](https://facebook.github.io/react-native/docs/tutorial)

[react native](https://facebook.github.io/react-native/)

[expo](https://expo.io/)

[expo snack](https://snack.expo.io/)

[ejecting](https://docs.expo.io/versions/latest/expokit/eject)