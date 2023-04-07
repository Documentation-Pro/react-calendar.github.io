<link rel="stylesheet" href="../../stylesheets/extra.css" />

## Overview
This section will walk you through how to manipulate your calendar with code examples.

!!! Info
    [React Calendar](https://www.npmjs.com/package/react-calendar) is a powerful tool that can be used to create interactive and customizable calendars in your React applications. With React Calendar, you can manipulate the data and the calendar itself by using React props.


```js
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


## Props

React Calendar comes with several props that allow you to customize its appearance and behavior. Props are the arguements we can pass to a react component.

```onChange```

Type: function

A function that gets called every time the user selects a new date. The function receives the selected date as an argument.
```handleDateChange``` would be defined outside of your App function. The line ```<Calendar onChange={handleDateChange} />``` would be called inside the return statement of the App component.
```js
function handleDateChange(date) {
  console.log(`Selected date: ${date}`);
}

<Calendar onChange={handleDateChange} />
```

```value```
Type: Date

> The currently selected date. This prop is required if you want to use React Calendar as a controlled component.

```js
<Calendar value={new Date()} />
```
```minDate```
Type: Date

The minimum date that can be selected. Users won't be able to select a date earlier than this date.

```js
<Calendar minDate={new Date('2022-01-01')} />
```
```maxDate```
Type: Date

The maximum date that can be selected. Users won't be able to select a date later than this date.
```js
<Calendar maxDate={new Date('2022-12-31')} />
```

```tileClassName```
Type: function | string | string[]

A function that gets called for each tile and returns a string with the CSS class name(s) to apply to the tile. Alternatively, you can pass a string or an array of strings with the CSS class name(s) to apply to all tiles.

```js
function getTileClassName({ activeStartDate, date, view }) {
  if (view === 'month' && date.getDay() === 0) {
    return 'sunday';
  }
}

<Calendar tileClassName={getTileClassName} />
```

```tileContent```
Type: function | React.ReactNode

A function that gets called for each tile and returns a React node to render inside the tile. Alternatively, you can pass a React node to render inside all tiles.

```js
function getTileContent({ date }) {
  return <div>{date.getDate()}</div>;
}

<Calendar tileContent={getTileContent} />
```



## List of props 
[React Calendar](https://www.npmjs.com/package/react-calendar) provides many props that you can use to customize its appearance and behavior. Here are some of the most commonly used props:

- `value` : This prop allows you to set the currently selected date in the calendar. You can use it to control the calendar from outside.

- `view` : This prop allows you to set the initial view of the calendar (month, week, or day).

- `calendarType` : sets the calendar type (e.g., US or ISO 8601).

- `minDate` and `maxDate` : These props allow you to set the minimum and maximum selectable dates in the calendar. You can use them to restrict the dates that users can select.

- `onActiveStartDateChange` : This prop handles when the user navigates from one view to another using previous/next button. Note: This function will not be called when drilling up/down.

- `onChange` : This prop handles when the user clicks an item (day on month view, month on year view and so on) on the most detailed view available.

- `onViewChange` : This prop is called when the user navigates from one view to another using drill up button or by clicking a tile.

- `onDrillUp`/`onDrillDown` : Function called when the user drills up by clicking drill up button.

- `showNavigation` : shows or hides the navigation buttons.

- `tileClassName` : a function that is called for each tile to set the class name.

- `tileContent` : a function that is called for each tile to set the content.

- `onClickDay`/`onClickDecade`/`onClickMonth`/`onClickWeekNumber`/`onClickYear` : This prop allows you to set a callback function that is called when a user clicks on a certain area in the calendar. The function receives two arguments: the value of the clicked area, and the original click event.

- `onKeyDown` : This prop allows you to set a callback function that is called when a user presses a key while the calendar is in focus. The function receives two arguments: the key event, and the value of the currently focused date.


## Conclusion

!!! success
    Now you should have a react calendar component with event listeners attached to it!