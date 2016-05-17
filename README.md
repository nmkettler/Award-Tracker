## What is this?
 
 This application (initally built for my team) can help managers/teams to create internal awards and nominate other team members. Everyone can create their own profile. Built with an angularJS MVC type structure. Google's Firebase to control the user authentication and simple data storage(user profiles, awards, nominations, etc.). 
 
## Code Example
 
 $scope.giveLove = function(myCheckin, myGift) {
      var refLove = new Firebase(FIREBASE_URL + 'users/' +
        $scope.whichuser + '/meetings/' +
        $scope.whichmeeting + '/checkins/' + myCheckin.$id +
        '/awards');
      var checkinsArray = $firebaseArray(refLove);

      var myData = {
        name: myGift,
       date: Firebase.ServerValue.TIMESTAMP
      }; //myData

      checkinsArray.$add(myData);
    }; //giveLove
 
## Motivation
 
 Our team was having trouble with tracking what we call "Star Awards". Before, the solution was an ancient Excel document. Many times, names would be forgotten as well as the reason why they were nominated.  I wanted to organize all of the nominations by separating them between users who are logged in and individual nominations (meetins.js). By doing this, the controllers are clean and not cluttered. 
 
## Installation
 
 Just clone the repo in a folder on your Desktop. Make sure the CDNs are up to date. You may need to create your own Firebase account if you want to edit the database. 
 
## API Reference
 
 angularJS: https://docs.angularjs.org/api 
 
 Firebase: https://www.firebase.com/docs/web/libraries/angular/api.html#angularfire-users-and-authentication-requireauth 
 
## API Reference
 
 No tests as of yet. 
 
## Contributors
 
 Feel free to contribute! If you find a bug in the app and don't know how to fix it create an issue. If you do know how to patch the bug or have any new great ideas make a pull request with the code. More information on how to do this can be found here:

 https://guides.github.com/activities/contributing-to-open-source/ 
