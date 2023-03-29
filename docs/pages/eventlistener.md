## Overview
React Calendar is a simple and easy-to-use library for adding calendar functionality to your React application. As for event listening such as onCLick, React Calendar can customize the appearance and behavior of the calendar using various props.

## Customization
React Calendar provides many props that you can use to customize its appearance and behavior. Here are some of the most commonly used props:

`value`: This prop allows you to set the currently selected date in the calendar. You can use it to control the calendar from outside.

`view`: This prop allows you to set the initial view of the calendar (month, week, or day).

`minDate` and `maxDate`: These props allow you to set the minimum and maximum selectable dates in the calendar. You can use them to restrict the dates that users can select.

`onActiveStartDateChange`: This prop handles when the user navigates from one view to another using previous/next button. Note: This function will not be called when drilling up/down.

`onChange`: This prop handles when the user clicks an item (day on month view, month on year view and so on) on the most detailed view available.

`onViewChange`: This prop is called when the user navigates from one view to another using drill up button or by clicking a tile.

`onDrillUp`/`onDrillDown`: Function called when the user drills up by clicking drill up button.

`onClickDay`/`onClickDecade`/`onClickMonth`/`onClickWeekNumber`/`onClickYear`: This prop allows you to set a callback function that is called when a user clicks on a certain area in the calendar. The function receives two arguments: the value of the clicked area, and the original click event.

`onKeyDown`: This prop allows you to set a callback function that is called when a user presses a key while the calendar is in focus. The function receives two arguments: the key event, and the value of the currently focused date.

You can also use CSS to style the calendar as per your requirements. The calendar component exposes several class names that you can use to target specific elements in the calendar.

## Conclusion
As shown below, you can change the behaviour of your custom calendar by using props.
You can read the selected date value from the calendar using the onClickDay prop. The same logic applies to using other props that listen for other events. 

```js
import Calendar from 'react-calendar'

function App() {
  return (
    <div className="App">
      <Calendar onClickDay={(value, event) => alert(value)} minDate={new Date()} />
    </div>
  );

```