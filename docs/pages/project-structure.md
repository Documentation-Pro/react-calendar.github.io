<link rel="stylesheet" href="../../stylesheets/extra.css" />

## Overview
Having a clear project structure is essential to collaborate on a web application. Also, it is important as it helps developers create new files following the existing conventions and helps them edit the existing files.



We can create a new react application using the following command

```
npx create-react-app calendar
```
React provide a solid structure to work upon. The default file structure after creating a new react application would look like the below:

```
calendar-test
├── package.json
├── public
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── README.md
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    ├── reportWebVitals.js
    └── setupTests.js
```

Furture there are other ways to struture the app

!!! Info
    Grouping by features or routes
[comment]: <> (Grouping by features or routes)

```
common/
  Avatar.js
  Avatar.css
  APIUtils.js
  APIUtils.test.js
feed/
  index.js
  Feed.js
  Feed.css
  FeedStory.js
  FeedStory.test.js
  FeedAPI.js
profile/
  index.js
  Profile.js
  ProfileHeader.js
  ProfileHeader.css
  ProfileAPI.js

```

!!! Info
    Grouping by file type
[comment]: <> (Grouping by file type)

```
api/
  APIUtils.js
  APIUtils.test.js
  ProfileAPI.js
  UserAPI.js
components/
  Avatar.js
  Avatar.css
  Feed.js
  Feed.css
  FeedStory.js
  FeedStory.test.js
  Profile.js
  ProfileHeader.js
  ProfileHeader.css
```
## Creating and navigating between files and folders

Create a new directory test

> mkdir test

Change directory

> cd test

Create a new javascript file

> touch calendar.js

Opening file in Visual Studio Code

> code calendar.js

## Conclusion
!!! success
    By the end of this section, you will have successfully learned the following:

    -  Why project structure is important
    -  Different styles of project structures
    -  How to customize the project structure




