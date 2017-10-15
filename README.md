# **Yugur.io Online Dictionary: Front-end Webapp**

This webapp is a frontend interface providing simple user access to the Yugur.io backend system.

The webapp consists of four primary systems: 
* **React.js framework** -- The primary building tool
* **Redux.js** -- Used for managing global state data, including search results, focused entries and UI language
* **Webpack** -- Used for managing the build process and dependencies
* **NPM (Node Package Manager)** -- This is the package manager for Node.js (used by the project), and all library imports should be done through npm. 
Npm's docs can be found [here](https://docs.npmjs.com/)

## *Install Process*

To get started, first install all the necessary dependencies.
```
> npm install
```

Run an initial webpack build
```
> webpack
```

Start the development server (changes will now update live in browser)
```
> npm run start
       OR
> npm run start & (This will leave the process running on the live server, even after you've disconnected)
```

To view your project running locally, go to: [http://localhost:3000/](http://localhost:3000/)

## *Project Architecture*

All code is contained within the ***dev*** folder. 

The root React component, ***index.js***, is found here, and loads the parent component for the rest of the app, ***App.js***, which is located in the ***components*** folder.

All other components can be found within the ***containers*** folder.

Redux *Actions* and *reducers* can be found in the ***actions*** and ***reducers*** folders, respectively.

The project builds into the ***src*** folder found in the root directory. This folder should **never be manually changed**, as this is purely a location for Webpack to bundle the app into.

