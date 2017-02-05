---
layout: post
title:  "React-Native app development"
categories: React-Native
excerpt: 'Hello, This is my first blog on React-Native. Click on the header to know how I created a mobile app. Feel free to add any inputs.'
---

This blog includes how I did an app using React-Native and steps I followed to do so.

>> I learned basics of ES6/7 which includes block variables, destructuring, template strings, arrow functions, spread operator, Promise, for-of, classes, modules, async/await functions  

  >> I included few sites which explained es6 better,  
    [ES6 features][lukehoban]  
    [explore es6][core-features]  
    [es6 & beyond][es6-beyond]  
    [Async Await][async-await]  
    Use Online editor to test any es6/7 feature  
    [es6 online editor][es6-editor]  

>> Learn [ReactJS][reactjs] basics as it won't take long. Checkout Dan abramov's redux videos [egghead.io][egghead]  

>> As you know, React uses one way data flow and has component architecture(i.e., every UI block is treated as a component).  

>> Then I picked React-Native and checked the [difference][difference] with ReactJS. I have seen many youtube videos & blogs to understand react-native.  

  >> Important things to remember on React-native  
     It is purely a javascript framework, when we build the project(es6/es7 will be converted to es5), UI components will be converted to native code and other Javascript code will run on the device javascript core (We can select any build platform). [More Info][more-info]  
     We use `View`, `Text` in place of block and inline elements.  
     We can use condition Platform.OS to identify whether IOS/Android.   

>> I researched boilerplates on react-native. I found [React-Native Snowflake][snowflake] which is very promising and well structured. It uses redux for state management and also they have separate snowflake server project which uses HAPIJS/Parse.  
  >> New libraries used :- Immutable-js, Redux

>> I learned [Immutable JS][immutable-js] map, setIn, getIn, Record, List etc. As the name suggests it is immutable means we cannot update  existing arrays, objects instead it will create new one on every property/value change.

>> Redux uses single state object through out the app. When we want to do any modification on any properties, we take the existing object, create the new state and add the new properties.  
>> Every-time ImmutableJS returns new state on any property changes.

>> Tips from my experience,  
   >> Extend React.Component instead of React.createClass  
   >> Use async operations inside componentDidMount method  
   >> Create two separate folders one for containers(higher order components which includes async operations) and other for simple components(commonly used components like button, alert, layout, header etc.). Check the difference in [presentational vs container components][presentaional-container].  
   >> Redux has three concepts,  
      >> Action(It is a function which returns object which includes reducer method name and payload)  
      >> Dispatch (to dispatch an action i.e., to call an action which in-turn calls reducer method)  
      >> Reducer method, which returns current state  

>> For designing components, I looked for existing node modules. I found [native base][native-base] which has many UI components.  

>> From my experience, understand the concepts and then start doing.  

>> Finally I have to say thanks to my friends Darshan, Santhosh for there valuable suggestions. Without them it could not be possible.


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
[more-info]: https://medium.com/@shaheenghiassy/react-native-s-execution-context-d63e5d4930f4#.tzj40ma53
