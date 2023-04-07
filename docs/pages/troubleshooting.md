<link rel="stylesheet" href="../../stylesheets/extra.css" />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Scope+One&display=swap" rel="stylesheet">

| **Symptoms** | **Probable Cause** | **Action** |
| ------------ | ------------------ | ---------- |
| Unable to load the localhost page | Your URL does not match your port number. | Double check in the browser if the app is running on localhost 3000. |
|     | The port 3000 is already taken | You can free a port using ```killall node``` command in the terminal.|
| No module found | Missing dependencies | Installl the missing dependencies using ```npm install dependency-name```
| Conflicting dependencies | Dependencies/Packages are incompatible. ```npm install``` gives error| use ```npm install --legacy-peer-deps``` instead. 
| Calendar is not defined | Missing import statement for react calendar | Add ```import Calendar from 'react-calendar'``` in the file where react calendar component is being called.


