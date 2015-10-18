ionic-twitter-test
==================

A Twitter client powered by Ionic Framework that I presented at the RokkinCat Hack & Tell. This is how incredibly easy it is to setup a project using Ionic Framework.

###Development Environment
If you've never developed with Node or Ionic, you'll have to follow these steps:
* Install [node.js](https://nodejs.org/en/)
* Install [bower](http://bower.io/)
* Install [ionic command line tools](https://www.npmjs.com/package/ionic)
* Follow instructions in Cordova's [Android Platform Guide](http://cordova.apache.org/docs/en/5.1.1/guide/platforms/android/index.html)
  * Stop at "Create New Project"
* Follow instructions in Cordova's [iOS Platform Guide](http://cordova.apache.org/docs/en/5.1.1/guide/platforms/ios/index.html)
  * Stop at "Create New Project"
* Install [ios-sim](https://www.npmjs.com/package/ios-sim)
* Install [ios-deploy](https://www.npmjs.com/package/ios-deploy)
  * If you get this error "Agreeing to the Xcode/iOS license requires admin privileges, please re-run as root via sudo.", run Xcode and agree to the license.

###Accessing Twitter's API
To access Twitter's API you must create an application at [apps.twitter.com](https://apps.twitter.com/)

###How I created this project
* Follow Simon Reimler's instructions in his article [here](http://devdactic.com/twitter-rest-api-angularjs/)

###Or if you just want to clone this project
After cloning this project run

```bash
$ ionic platform add ios
$ ionic platform add android
$ npm install
```

Add your Consumer Key and Consumer Secret to app.js
```javascript
var clientId = '';
var clientSecret = '';
```

Then run
```bash
$ ionic emulate ios
$ ionic emulate android
```

Note: In this project, I've removed my Consumer Secret from app.js

Note: ngTwitter can't authenticate with a web browser on your local machine. You must run the application in an emulator or deploy it to a device.

Note: See more about the sources for [ng-twitter](https://github.com/saimon24/ng-twitter) and [ng-cordova](https://github.com/driftyco/ng-cordova/)
