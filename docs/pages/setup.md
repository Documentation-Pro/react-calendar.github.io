## Setup React Calendar in a new project
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
## Setup React Calendar in an existing project


## General Usage
Read date value and set min date to todays date:
onClickDay is the props we pass to the Calendar component and the first argument is the value of the day 

``` javaScript linenums="1"
import Calendar from 'react-calendar'
function App() {
  return (
    <div className="App">
      <Calendar onClickDay={(value, event) => alert(value)} minDate={new Date()} />
    </div>
  );
}

export default App;
```


## Conclusion