<link rel="stylesheet" href="../stylesheets/extra.css" />

<link rel="stylesheet" href="../stylesheets/extra.css" />

# React Calendar Documentation: Installation, Usage, and Customization Guide

Welcome to our documentation for React Calendar! 📖 In this guide, you will learn how to install and use the React Calendar package, as well as customize it to suit your needs.

For full official npm documentation visit [npm-React-Calendar](https://www.npmjs.com/package/react-calendar)

For React Calendars official webpage visit [React-Calendar](https://projects.wojtekmaj.pl/react-calendar/)

Want to try a live demo? Visit [Live Demo](https://projects.wojtekmaj.pl/react-calendar/)

## What is React Calendar? 📆

React Calendar is a lightweight calendar package designed for use in React applications. It provides a simple and customizable way to display calendars and schedule events. It is currently being managed by a developer under the name Wojciech Maj. The developer has made this amazing tool light and fast, extremely customizable, work with any language, rock-solid/bug-free, and best of all open source! (forever)

## Intended Users

Our documentation is targeted towards the following users:

Beginner developers who need to set up a React Calendar for a personal project.
  
!!! Info
    Prerequisites:

    - Basic understanding of Command Line Interface.
    - Basic understanding of Visual Studio Code.
    - Basic proficiency of Node package manager.


## Getting Started

To use React Calendar in your project, you'll need to have the following pre-requisites installed:

 > [Node JS](https://nodejs.org/en) Node Environment is required to use React and React Calendar

 > [Visual Studio Code](https://code.visualstudio.com/) Working with documentation requires a text editor, please install VS Code or you can work with your favorite text editor


<figure markdown>
  ![React Calendar](https://camo.githubusercontent.com/366e44bda8cd8313fa3043f9ad8c50a205696527268fb410e22db006a917afa9/68747470733a2f2f70726f6a656374732e776f6a74656b6d616a2e706c2f72656163742d63616c656e6461722f72656163742d63616c656e6461722e6a7067){ width="300" }
  <figcaption>React Calendar</figcaption>
</figure>


## Basic Usage
Once you have React Calendar installed, you can use it in your [React](https://react.dev/) application by importing the Calendar component and rendering it in your component. If you are not familiar with React, this may be a difficult task at first, that's why we are going to show you. 😎 Here's an example of how to use React Calendar in a basic React component:


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
export default MyApp;
```

So in this example, we are importing the Calendar component from the react-calendar package and using the useState hook to manage the state of the selected date. State manages the variables binded to a react component.

If you're not familiar with [React](https://react.dev/) hooks, you can find out more about them [here](https://react.dev/learn#using-hooks)

We then render the Calendar component with the onChange and value props to enable date selection and update the selected date state.

This is just a basic example of how to use [React Calendar](https://www.npmjs.com/package/react-calendar), and that you can definitely customize it to suit your needs by passing additional props and styles to the Calendar component as needed.

## Advanced Usage

Once you've gotten the hang of things mentioned above in the basic usage section, you might be interested in getting more advanced with [React Calendar](https://www.npmjs.com/package/react-calendar).

Thankfully, [React Calendar](https://www.npmjs.com/package/react-calendar) provides many props and options for customization. Here are some common props that you can use to customize your calendar:

!!! Info
    Again, please keep in mind that there are many more available props to use.

    You can find a list of all of the available props [here](https://www.npmjs.com/package/react-calendar)

### Props

Props are the arguements passed to a react component. Props determines the behavior of a component.


* `value` : sets the selected date.
* `onChange` : a function that is called when the date selection changes.
* `minDate` and `maxDate` : sets the minimum and maximum selectable dates.
* `calendarType` : sets the calendar type (e.g., US or ISO 8601).
* `showNavigation` : shows or hides the navigation buttons.
* `tileClassName` : a function that is called for each tile to set the class name.
* `tileContent` : a function that is called for each tile to set the content.

### Styling

If you want to use default Calendar styling to build upon its existings syles, you can import React-Calendar's styles by importing Calendar.css

```javascript
import 'react-calendar/dist/Calendar.css';
```

## Note and warning messages

In the documentation you will see a series of indicator messages with different meanings. The messages will be as follows:

!!! danger
    Specifies actions that may cause an error or will cause the application to crash.

!!! warning
    Specifies content that must be read before proceeding, so please pay attention!

!!! Info
    Indicates additional information or tips.

!!! success
    Indicates you successfully completed a section or task, good job!

# Conclusion

We hope you find our React Calendar documentation helpful! If you have any questions or feedback, please do not hesitate to contact us.

## Contributers

> Jack Boeri - jboeri@my.bcit.ca

> Paarth Dhammi - pdhammi@my.bcit.ca

Happy coding! 😄