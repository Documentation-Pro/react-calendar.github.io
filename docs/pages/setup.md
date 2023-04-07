<link rel="stylesheet" href="../../stylesheets/extra.css" />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Scope+One&display=swap" rel="stylesheet">

## Overview
In this section, we will walk through the installation of [React Calendar](https://www.npmjs.com/package/react-calendar), which involves creating a new project directory, installing [React 16.3](https://react.dev/) or later, and importing the Calendar component in the App.js file. 

## Installation Steps for React Calendar

!!! warning
    As for [Compatibility](https://github.com/wojtekmaj/react-calendar#compatibility), your project needs to use [React 16.3](https://react.dev/) or later.

[React Calendar](https://www.npmjs.com/package/react-calendar) uses modern web technologies. That's why it's fast, lightweight, and easy to style. However, it comes at the cost of supporting only modern browsers.
 
!!! info
    Please be patient, as installing React on your system may take a few minutes
 
1. Create a new project directory
  > npx create-react-app my-app
1. In Visual Studio Code, open your desired terminal in your current project directory
  > cd my-app
1. To install react-calendar
  > npm install react-calendar
1. Run the following commands in order:
  > npm start

![image of react app](../images/reactexample.png "Upon installing react")
4. In `my-app/src/App.js` import react-calendar
```js
import Calendar from 'react-calendar'
```
5. Replace the return code block of the App function with code below 
```js
return (
    <Calendar />
  );
```

Example of `/App.js` file:
```js
import './App.css';
import Calendar from 'react-calendar'

function App() {
  return (
    <Calendar />
  );
}

export default App;
```

Everything you need to access/manipulate with React Calendar is going to be found on the Calendar Components props. You can find more about the interactivity and customization of your calendar here: <a href='../eventlistener/'>Event Listeners</a>, <a href='../styling/'>Styling</a>



## Conclusion

<!-- !!! warning
    Specifies content that must be read before proceeding.

!!! Info
    Indicates additional information or tips. -->

!!! success
    You have successfully integrated react calendar with react application.

  You should now have a working React Calendar in your React Application. Great work!