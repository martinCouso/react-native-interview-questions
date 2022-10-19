# react-native-interview-questions

<h1>Questions</h1>

### Jr Questions
<p>The idea behind this first set of questions is to know if the developer have had a contact with the technology and that it's comfortable with the core concepts of React/React Native.</p>

| #id | Question                                                                                                                       |
|:---:|:-------------------------------------------------------------------------------------------------------------------------------|
|  1  | [What is React Native?](#what-is-react-native)                                                                                 |
|  2  | [What are the difference between React Native and React?](#what-is-react-native)                                               |
|  3  | [What are the main characteristics of React Native?](#what-is-react-native)                                                    |
|  4  | [Do you know any other tools similar to React Native? If so, mention some pros and cons](#what-is-react-native)                |
|  5  | [What is JSX?](#what-is-react-native)                                                                                          |
|  6  | [What are the Components?Please name the different types](#what-is-react-native)                                               |
|  7  | [What are the Props?](#what-is-react-native)                                                                                   |
|  8  | [What is the State?](#what-is-react-native)                                                                                    |
|  9  | [What is the ScrollView used for?](#what-is-react-native)                                                                      |
| 10  | [What are list Views? Name the two most common implementations of List Views](#what-is-react-native)                           |
| 11  | [Name the two main approaches to create Platform Specific Code? Please Specify when you would use each](#what-is-react-native) |
| 12  | [To which platforms is React Native able to compile to?](#what-is-react-native)                                                |
| 13  | [What are Life Cycles? Enumerate and describe what each of them do](#what-is-react-native)                                     |
| 14  | [What are Hooks? Enumerate and describe what each of them do](#what-is-react-native)                                           |
| 15  | [Which ways do you know to communicate a React Native application with a Backend?](#what-is-react-native)                      |
| 16  | [What are common ways to debug a React Native application?](#what-is-react-native)                                             |
| 17  | [Does react native provides navigation tools?](#what-is-react-native)                                                          |
| 18  | [How are Styles handled in React Native?](#what-is-react-native)                                                               |
| 19  | [What is the Async Storage?](#what-is-react-native)                                                                            |
| 20  | [What animation systems are provided by React Native?](#what-is-react-native)                                                  |

### Ssr Questions

|  #  | Question                                                                                                                              |
|:---:|:--------------------------------------------------------------------------------------------------------------------------------------|
|  1  | [Does React Native works with any syntax transformer by default? if it does which do you think is the reason?](#what-is-react-native) |
|  2  | [Name the main characteristics of React Navigation and React Native Navigation](#what-is-react-native)                                |
|  3  | [What are Error Boundaries? What kind of errors can not be caught with this type of component?](#what-is-react-native)                |
|  4  | [What are common ways to optimize a Flat List?](#what-is-react-native)                                                                |
|  5  | [What type of tests can be performed on React Native?](#what-is-react-native)                                                         |
|  6  | [How many times is the useEffect Hook called by default?](#what-is-react-native)                                                      |
|  7  | [What is a HOC? In which scenarios are a good idea to implement one?](#what-is-react-native)                                          |
|  8  | [What is the Render Props pattern? When should you use it?](#what-is-react-native)                                                    |
|  9  | [What](#what-is-react-native)                                                                                                         |
| 10  | [What are Native Modules?](#what-is-react-native)                                                                                     |
| 11  | [What are Native Components?](#what-is-react-native)                                                                                  |
| 12  | [Does React Native supports accessibility? What tools are provided to the developers?](#what-is-react-native)                         |
| 13  | [Name the 3 core concepts of Redux](#what-is-react-native)                                                                            |
| 14  | [Describe the information flow in Redux](#what-is-react-native)                                                                       |
| 15  | [What is Redux Toolkit?](#what-is-react-native)                                                                                       |
| 16  | [What is Mobx?](#what-is-react-native)                                                                                                |
| 17  | [What is GraphQL?](#what-is-react-native)                                                                                             |
| 18  | [What is React Query?](#what-is-react-native)                                                                                         |
| 19  | [What is Reanimated2?](#what-is-react-native)                                                                                         |
| 20  | [What is Lottie React Native?](#what-is-react-native)                                                                                 |

### Sr Questions

|  #  | Question                                                                                                                              |
|:---:|:--------------------------------------------------------------------------------------------------------------------------------------|
|  1  | [What is the New Architecture on React Native?](#what-is-react-native)                                                                |
|  2  | [What is the InteractionManager? What are common scenarios to implement it?](#what-is-react-native)                                   |
|  3  | [How do you create Native Modules?](#what-is-react-native)                                                                            |
|  4  | [How do you create Native Components?](#what-is-react-native)                                                                         |
|  5  | [What is Headless Js and which are common uses for it?](#what-is-react-native)                                                        |
|  6  | [What approach can you take to find a memory leak?](#what-is-react-native)                                                            |


### What is React Native?
- React Native is an open source framework for building Android and iOS applications using React and the app platform’s native capabilities. With React Native, you use JavaScript to access your platform’s APIs as well as to describe the appearance and behavior of your UI using React components: bundles of reusable, nestable code. You can learn more about React in the next section. But first, let’s cover how components work in React Native.

### What are the difference between React Native and React?
- While the js library React is meant to be use as a tool to develop web applications the framework React Native is used to build Android and IOS applications.
- React is a fundamental part of React Native, but the inverse is not true.
- In React Js components are compiled to HTML elements while in React Native are converted to native components on each platform.

### What are the main characteristics of React Native?
- Is Multiplatform, officially maintained by Meta for Android and IOS, and by third parties for Windows and Web.
- Most of the code is written in JavaScript and rendered with native code, enabling web developers to rapidly create applications with native platform UI.
- On top of supporting building for multiple platforms it allows to share most of the code between those platforms, meaning that most applications will share near 85% of business logic and UI code between IOS and Android.
- Rapid development experience, thanks to the Fast Refresh there's no need to wait to see the changes like happens for example with native builds.

### Do you know any other tools similar to React Native? If so, mention some pros and cons
- Flutter and Ionic 

### What is JSX?     
- JSX stands for JavaScript XML, is basically a syntax extension to JavaScript and allows us to create components inside JS by providing a syntactic sugar for the React.createElement function.
    ```jsx
    const element = (
      <Text>
        Hello, world!
      </Text>
    )
    const element = React.createElement(
      'Text',
      [],
      'Hello, world!'
    );
    ```
- React needs to be on scope to be able to utilize JSX.
    ```jsx
  import React from 'react';
  ```
- Babel compiles JSX down to React.createElement() calls.
- It provides an easy and visual syntax to set an elements children, we just need to wrap the children/s between the opening and closing tags of the parent.
  ```jsx
  const element = (
  <Parent>
    <ChildrenOne>Hello!</ChildrenOne>
    <ChildrenTwo>Good to see you here.</ChildrenTwo>
  </Parent>);
  ```

### What are the Components?Please name the different types.
- Conceptually, components are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
- Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.
- There are two types ways to build a components, it can be a Functional Component(FN) or a Class Component(CC), in the past if you wanted to for the component to have internal state CC were the only option, in the present (thanks to React Hooks) you chose either.
  ```jsx
  // Functional Component
  function CustomGrettingFC(props) {
    return <Text style={styles.grettingText}>Hello, {props.name}</Text>;
  }
  
  //Class Component
  class CustomGrettingCC extends React.Component {
    render() {
        return <h1>Hello, {this.props.name}</h1>;
    }
  }
  ```
- React also provides a third type of Component, or a subtype of CC if you will, called Pure Component (PC). That is meant to be used in cases where the performance is a requirement. As long as the component’s render() function renders the same result given the same props and state, you can use React.PureComponent for a performance boost in some cases.
  ```jsx
  class CustomGrettingPC extends React.PureComponent {
    render() {
        return <h1>Hello, {this.props.name}</h1>;
    }
  }
  ```
- React Native offers several core components like View, Text, Image, etc. But you also can create your own custom components or use the ones created by the community.
### What are Props?
- When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.
- An easy way to describe this concept is that Props are to React Components what arguments are to JavaScript Functions.
- Props are read-only, a Component never should change the value of the properties that receives.
- Everytime that a prop value is updated by a parent component the child will rerender unless we specifically prevent it.
- We can set  default values for Props by setting defaultProps, and those values are going to be use for undefined props (but not for null props).
```jsx
  // Functional Component
  function CustomGrettingFC(props) {
    return <Text style={styles.grettingText}>Hello, {props.name}</Text>;
  }
  CustomGrettingFC.defaultProps = {
    name: 'User'
  }
  
  //Class Component
  class CustomGrettingCC extends React.Component {
    render() {
        return <h1>Hello, {this.props.name}</h1>;
    }
  
    static defaultProps = {
        name: "User",
    }
  }
  ```
### What is State?
- In a similar fashion as the Props, State is a mechanism to hold information on a Component that in case to be updated it will trigger a rerender, but it's intern and controlled by the Component itself.
- In the past only CC could use this mechanism, but in RN 0.59 hooks were introduced allowing FC to have their own way to handle State.
- The State can't be updated directly, instead `this.setState` for CC and the setter function returned by `useState` for FC are needed.
- The State updates are not always run instantly, they may be asynchronous since React waits for the most efficient moment to update the state, it's possible that several calls to update the state will be executed in a batch.
- The changes in the state are merged, meaning that if we have a complex state in a component and we only update a part the rest of the state won't be touched, just the intended part.
### What is the ScrollView used for?
- The ScrollView is a scrolling container meant to be used to hold a small set of heterogeneous elements that can't be displayed entirely in the height or width of the screen.
- It can be use vertically or horizontally.
- TODO: CODE E.G.
### What are the List Views? Name the two most common implementations of List Views in RN.
- List Views are the tools that we have to render a scrollable medium/big set of homogenous items, like a list of cards, photos, etc.
- Currently, the two most common List Views that we utilize are FlatList and SectionList
- FlatList is a performant scrollable list that requires at the minimum to set two properties `data` and `renderItem`, data expects the array of items to be displayed and renderItem a function that returns a component that will be rendered for each element of the array.
- Section list is similar to the FlatList, but it will require a property called `sections` instead of `data` and an extra property called `renderSectionHeader`, sections expects Array<{title:string, data: Array<T>}> while renderHeader expects a function to know how to render each of the section headers. 
### Name the two main approaches to create Platform Specific Code? Please Specify when you would use each 
### To which platforms is React Native able to compile to?                                                
### What are Life Cycles? Enumerate and describe what each of them do                                     
### What are Hooks? Enumerate and describe what each of them do                                           
### Which ways do you know to communicate a React Native application with a Backend?                      
### What are common ways to debug a React Native application?                                             
### Does react native provides navigation tools?                                                          
### How are Styles handled in React Native?                                                               
### What is the Async Storage?                                                                            
### What animation systems are provided by React Native?                                                  
