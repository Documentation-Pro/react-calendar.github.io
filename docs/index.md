<link rel="stylesheet" href="../stylesheets/extra.css" />

# Welcome to React Calendar

For full documentation visit [npm-React-Calendar](https://www.npmjs.com/package/react-calendar)

For React Calendars official webpage visit [React-Calendar](https://projects.wojtekmaj.pl/react-calendar/)

<figure markdown>
  ![React Calendar](https://camo.githubusercontent.com/366e44bda8cd8313fa3043f9ad8c50a205696527268fb410e22db006a917afa9/68747470733a2f2f70726f6a656374732e776f6a74656b6d616a2e706c2f72656163742d63616c656e6461722f72656163742d63616c656e6461722e6a7067){ width="300" }
  <figcaption>React Calendar</figcaption>
</figure>

# Pre-requisite
    React
    npm

## Install

* Install by executing `npm install react-calendar` or `yarn add react-calendar`
* Import by adding `import Calendar from 'react-calendar'`
* Use by adding `<Calendar />` 
* Use `onChange` prop for getting new values.

## Setup

* `Compatibility` Your project needs to use React 16.3 or later.

* `React-Calendar` uses modern web technologies. That's why it's so fast, lightweight and easy to style. This, however, comes at a cost of supporting only modern browsers.

* `Legacy browsers`
If you need to support legacy browsers like Internet Explorer 10, you will need to use Intl.js or another Intl polyfill along with React-Calendar.


## Usage
Here's an example of basic usage:

``` javaScript linenums="1"
    import React, { useState } from 'react';
    import Calendar from 'react-calendar';

    function MyApp() {
    const [value, onChange] = useState(new Date());

    return (
        <div>
        <Calendar onChange={onChange} value={value} />
        </div>
    );
    }
```

## Customizing your Calendar

* `Custom styling` - If you want to use default React-Calendar styling to build upon its existings syles, you can import React-Calendar's styles by importing react-calendars default css file (this will make it easier to customize as you can see existing styles):

```javascript
import 'react-calendar/dist/Calendar.css';
```