<link rel="stylesheet" href="../stylesheets/extra.css" />

# Welcome to React Calendar


React-Calendar is the ultimate lightweight Calendar for your React application. Please note that React-Calendar is under constant development and if you would like to see official documentation, please go to the following link.

For full documentation visit [npm-React-Calendar](https://www.npmjs.com/package/react-calendar)

For React Calendars official webpage visit [React-Calendar](https://projects.wojtekmaj.pl/react-calendar/)

Want to try a live demo? Visit [Live Demo](https://projects.wojtekmaj.pl/react-calendar/)


## Intended Users

This documentation is targeted towards the following users:

- Beginner to intermediate developers who need to setup a React Calendar for a personal project.
- Software development teams working on small or medium-sized web applications.



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
* Use by adding render component `<Calendar />` 

for a more detailed install guide, click <a href='/pages/setup'>here</a>

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

Custom styling - If you want to use default React-Calendar styling to build upon its existings syles, you can import React-Calendar's styles by importing react-calendars default css file (this will make it easier to customize as you can see existing styles):

```javascript
import 'react-calendar/dist/Calendar.css';
```

## Note and warning messages

!!! danger
    Specifies actions that may cause an error or will cause the application to crash.

[comment]: <> (!!! failure)

[comment]: <> (    Specifies actions that may lead to unexpected behaviour.)

[comment]: <> (!!! bug)

[comment]: <> (    Specifies actions that may cause an error.)

!!! warning
    Specifies content that must be read before proceeding.

!!! Info
    Indicates additional information or tips.

!!! success
    Indicates what success looks like.