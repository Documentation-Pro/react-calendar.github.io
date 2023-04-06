
| **Symptoms** | **Probable Cause** | **Action** |
| ------------ | ------------------ | ---------- |
| Unable to load the localhost page | Your URL does not match your port number. | Double check in the browser if the app is running on localhost 3000. |
|     | The port 3000 is already taken | You can free a port using ```killall node``` command in the terminal.|
| No module found | Missing dependencies | Installl the missing dependencies using ```npm install dependency-name```
| Conflicting dependencies | Dependencies/Packages are incompatible. ```npm install``` gives error| use ```npm install --legacy-peer-deps``` instead. 