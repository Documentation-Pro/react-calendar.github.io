<link rel="stylesheet" href="../../stylesheets/extra.css" />

## Setup React Calendar
1. Create a new project directory
2. Open your desired terminal
3. Run the following commands in order:
```js
npx create-react-app my-app
cd my-app
npm start
```
![image of react app](../images/reactexample.png "Upon installing react")
4. In `my-app/src/App.js` import react-calendar
```js
import Calendar from 'react-calendar'
```
5. return the Calendar component in your App function
```js
return (
    <Calendar />
  );
```

Your App.js file should look like this:
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

## General Usage
Everything you need to access/manipulate with React Calendar is going to be found on the Calendar Components props. You can find about more about the interactivity of your calendar here: <a href='../eventlistener/'>Event Listeners</a>


