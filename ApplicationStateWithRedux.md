#  Application State with Redux 

- What are the advantages of storing tokens in “Cookies” vs “Local Storage”
Cookies are automatically saved, sent and removed by the browser. When doing browser level navigation, only cookies are sent. Sharing the same session across subdomains can easily be done with cookies. Cookies have a special flag called httpOnly, which means that malicious JS code cannot send the access token to the attacker.

- Explain 3rd party cookies.
Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a "Like" button on your website which will store a cookie on a visitor's computer, that cookie can later be accessed by Facebook to identify visitors and see which websites they visited. Such a cookie is considered to be a 3rd party cookie.[source](https://cookie-script.com/all-you-need-to-know-about-third-party-cookies.html)
 as explained before, are cookies that are stored under a different domain than you are currently visiting. They are mostly used to track users between websites and display more relevant ads between websites. Another good example is a support chat functionality provided by a 3rd party service.

- How do pixel tags work?
A tracking pixel is an HTML code snippet which is loaded when a user visits a website or opens an email. It is useful for tracking user behavior and conversions.

A tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. Because it is so small, it can hardly be seen by visitors of a website or email recipients. These tracking pixels are partly or fully designed to be transparent, or camouflaged in the background color of the website so that they don't stand out to users. Users are usually not supposed to see the tracking pixel.

The website operator or sender of an email adds the tracking pixel using a code in the website’s HTML code or email. This code contains an external link to the pixel server. If a user visits the destination website, the HTML code is processed by the client – usually the user’s browser. The browser follows the link and opens the (invisible) graphic. This is registered and noted in the server’s log files.

In addition, various information about the user is also transmitted using this method. To some extent, combination with JavaScript is necessary in order to collect information about the operating system or browser type.[source](https://en.ryte.com/wiki/Tracking_Pixel)

## Term
- cookies:are small blocks of data created by a web server while a user is browsing a website and placed on the user's computer or other device by the user’s web browser. Cookies are placed on the device used to access a website, and more than one cookie may be placed on a user’s device during a session.

- authorization:Process of giving someone the ability to access a resource

- access control:data security that dictates who's allowed to access and use company information and resources. Through authentication and authorization, access control policies make sure users are who they say they are and that they have appropriate access to company data.

- conditional rendering:In React, conditional rendering refers to the process of delivering elements and components based on certain conditions.[source](https://blog.logrocket.com/conditional-rendering-in-react-c6b0e5af381e/)

***

### Preparation Materials

***Redux*** is a predictable state container for JavaScript apps.

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience.

You can use Redux together with React, or with any other view library. It is tiny (2kB, including dependencies), but has a large ecosystem of addons available.

- Installation
    - Redux Toolkit#
    Redux Toolkit is our official recommended approach for writing Redux logic. It wraps around the Redux core, and contains packages and functions that we think are essential for building a Redux app. Redux Toolkit builds in our suggested best practices, simplifies most Redux tasks, prevents common mistakes, and makes it easier to write Redux applications.


RTK includes utilities that help simplify many common use cases, including store setup, creating reducers and writing immutable update logic, and even creating entire "slices" of state at once.

***


[Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)

### Bookmark
[worlds easiest guide to redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)