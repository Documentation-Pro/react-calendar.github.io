## Overview
## Customization


## Usage
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