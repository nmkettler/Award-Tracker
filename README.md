# Award-Tracker

# Angular-Registration
 
## What is this?
 
 A great basis for user registration you would like to implement on your site. Built with an angularJS MVC type structure. Google's Firebase to control the user authentication and simple data storage. 
 
## Code Example
 
 myApp.factory('Authentication', 
   ['$rootScope', '$firebaseAuth', '$firebaseObject',
   '$location', 'FIREBASE_URL',
   function($rootScope, $firebaseAuth, $firebaseObject,
     $location, FIREBASE_URL) {...
 
## Motivation
 
 I have created several other user registrations with PHP but this is by far the cleanest/elegant solutions I have come up with. I wanted to organize all of the authentication into one javascript file (authentication.js). By doing this, the controllers are clean and not cluttered. 
 
## Installation
 
 Just clone the repo in a folder on your Desktop. Make sure the CDNs are up to date. I decided to download angularJS instead of using the CDN however either way should be fine. 
 
## API Reference
 
 angularJS: https://docs.angularjs.org/api 
 
 Firebase: https://www.firebase.com/docs/web/libraries/angular/api.html#angularfire-users-and-authentication-requireauth 
 
## Tests
 
 No tests as of yet. Plan on testing through the Jasmine Framework
 
## Contributors
 
 Feel free to contribute! If you find a bug in the app and don't know how to fix it create an issue. If you do know how to patch the bug or have any new great ideas make a pull request with the code. More information on how to do this can be found here:
 
 https://guides.github.com/activities/contributing-to-open-source/ 
