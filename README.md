# Tut's Plus Getting Started With Angular 2
https://github.com/tutsplus/get-started-with-angular-2
https://code.tutsplus.com/courses/get-started-with-angular-2
https://angular.io/

### Overview Notes
* angular 2 completely diff framework from angularjs
* typescript with angular 2
* google built platform and incorporated in ionic and foundation
* build using typescript which uses es6 syntax
* features a simple login system (login.component.js)
* uses Google Youtube APIs (ytube.service.js)
* style directive causes login button to be pink on mouse hover using fallback main.html (style.directive.js | templates/main.html)
* student-center files inside this folder = modular portion of the app. /student-center/students > /student-center/student/1002

package.json
```json
{
  "name": "angular2-tutsplus",
  "version": "1.0.0",
  "scripts": {
    "postinstall": "npm run typings install",
    "tsc": "tsc",
    "tsc:w": "tsc -w",
    "lite": "lite-server",
    "start": "concurrent \"npm run tsc:w\" \"npm run lite\" ",
    "typings": "typings"
  },
  "license": "ISC",
  "dependencies": {
    "angular2": "2.0.0-beta.3",
    "systemjs": "0.19.6", //module loader
    "es6-promise": "^3.0.2",
    "es6-shim": "^0.33.3",  //compatibility for legacy js engines
    "reflect-metadata": "0.1.2",  //for declorators
    "rxjs": "5.0.0-beta.0",
    "zone.js": "0.5.11" //alow for zones
  },
  "devDependencies": {
    "concurrently": "^1.0.0",
    "lite-server": "^2.0.1",
    "typescript": "^1.7.5",
    "typings":"^0.6.8"
  }
}
```

### Get Started 
* create package.json, tsconfig.json, typings.json
* download [skeleton](http://getskeleton.com/) and put the files in the css folder
* with IIS you'll need to create a website within IIS Manager and edit the VHOST
* create an empty app and template folder for the following script to auto-create the needed files
* running npm install will create the node_modules with some errors which is ok.
* running npm start will create the app.js within the app folder and load up the browser with the application running


```
npm install
npm start
```

Brower will automatically open browser and show the angular app.

* Youtube API key is needed.  Go to GoogleAPIs.com and enter the keys in ytube.service.ts
