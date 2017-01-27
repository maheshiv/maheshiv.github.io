---
layout: post
title:  "Welcome to my blog"
categories: React-Native
excerpt: 'Hello, This is my first blog on React-Native'
---

This blog includes how I did app using React-Native.

>> I learned basics of ES6/7 which includes block variables, destructuring, template strings, arrow functions, spread operator, Promise, for-of, classes, modules, async/await functions

  I included few sites which explained es6 better,

  [ES6 features][lukehoban]
  [explore es6][core-features]
  [es6 & beyond][es6-beyond]
  [Async Await][async-await]
  Use Online editor to test any es6/7 feature
  [es6 online editor][es6-editor]

>> I learned [ReactJS][reactjs] basics, it does not take more time to understand. Then I checked redux. Dan abramov's redux tutorial videos [egghead.io][egghead]

>> As you know, React uses one way data flow and has component architecture(i.e., every UI block is treated as component).

>> Tips from my experience,

   >> Extend React.Component instead of React.createClass
   >> Use async operations inside componentDidMount method
   >> Create two separate folders one for containers(higher order components which includes async operations) and other for simple components(common simple components like button, alert, layout, header etc.). Check the difference in [presentational vs container components][presentaional-container].
   >> Redux has three concepts,
      ++ Action(It is a function which returns object which includes reducer method name and payload)
      ++ Dispatch (to dispatch an action i.e., to call an action which in-turn calls reducer method)
      ++ Reducer method, which returns current state

>> I learned [Immutable JS][immutable-js] map, setIn, getIn, Record, List etc.

  >> Redux uses single state object through out the app. When we want to do any modification on any property, we take the existing object, create the new state (using existing object) and add the new properties.
  >> Every-time we return new state on any property changes

>> Then I picked React-Native and checked the [difference][difference] with ReactJS. I have seen many youtube videos & blogs to understand react-native.

  >> Important things to remember on React-native
    ++ It is purely a javascript framework, when we build the project, compiler will convert Javascript code into native code(we can select the build platform).
    ++ We use `View`, `Text` in place of block and inline elements
    ++ We can use condition like Platform.OS to identify whether IOS/Android

>> I researched boilerplates on react-native. I found [React-Native Snowflake][snowflake] which is very promising and well structured. It uses redux for state management and also they have separate snowflake server project which uses HAPIJS/Parse.

>> For designing components, I looked for existing node modules. I found [native base][native-base] which has many UI components.

>> I understand snowflake project structure on client and server and develop the app in two months.

>> From my experience, understand the concepts and start doing.


[difference]: https://medium.com/@alexmngn/from-reactjs-to-react-native-what-are-the-main-differences-between-both-d6e8e88ebf24#.ls6zapbqo
[presentaional-container]: https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.2z07opcjt
[egghead]: https://egghead.io/courses/getting-started-with-redux
[reactjs]: https://facebook.github.io/react/tutorial/tutorial.html
[lukehoban]: https://github.com/lukehoban/es6features
[core-features]: http://exploringjs.com/es6/ch_core-features.html
[es6-beyond]: https://github.com/getify/You-Dont-Know-JS/tree/master/es6%20%26%20beyond
[es6-editor]: https://babeljs.io/repl/
[async-await]: http://www.2ality.com/2016/02/async-functions.html
[immutable-js]: https://facebook.github.io/immutable-js/
[snowflake]: https://github.com/bartonhammond/snowflake
[native-base]: http://nativebase.io/
