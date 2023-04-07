<link rel="stylesheet" href="../../stylesheets/extra.css" />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Scope+One&display=swap" rel="stylesheet">


Here are some links to official documentations that could be helpful for developers.

<div class="grid" markdown>

=== "ReactJS"
    :material-react:{ .lg .middle } __ReactJS__

    The library for web and native user interfaces · React lets you build user interfaces out of individual pieces called components

    [:octicons-arrow-right-24: READ MORE](https://react.dev/)
   

=== "CSS"

    :fontawesome-brands-css3:{ .lg .middle } __CSS__

    Cascading Style Sheets (CSS) is a simple mechanism for adding style (e.g., fonts, colors, spacing) to Web documents.

    [:octicons-arrow-right-24: READ MORE](https://www.w3.org/Style/CSS/Overview.en.html)

=== "React Calendar"

    :calendar:{ .lg .middle } __React Calendar__

    Ultimate calendar for your React app. Pick days, months, years, or even decades.Supports range selection.Supports virtually any language

    [:octicons-arrow-right-24: READ MORE](https://www.npmjs.com/package/react-calendar)

=== "JS Date Object"

    :date:{ .lg .middle } __Javascript Date Object__

    JavaScript Date objects represent a single moment in time in a platform-independent format.

    [:octicons-arrow-right-24: READ MORE](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)

</div>

Below are some most common problems developers may encounter

| **Symptoms** | **Probable Cause** | **Action** |
| ------------ | ------------------ | ---------- |
| Unable to load the localhost page | Your URL does not match your port number. | Double check in the browser if the app is running on localhost 3000. |
|     | The port 3000 is already taken | You can free a port using ```killall node``` command in the terminal.|
| No module found | Missing dependencies | Installl the missing dependencies using ```npm install dependency-name```
| Conflicting dependencies | Dependencies/Packages are incompatible. ```npm install``` gives error| use ```npm install --legacy-peer-deps``` instead. 
| Calendar is not defined | Missing import statement for react calendar | Add ```import Calendar from 'react-calendar'``` in the file where react calendar component is being called.
| react-scripts: command not found| Packages in package.json are not installed | Install node-modules using `npm install` command from the root of your project

