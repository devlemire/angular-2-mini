<img src="https://devmounta.in/img/logowhiteblue.png" width="250" align="right">

# Project Summary

In this project, we'll cover how to use Angular services to separate the management of data from the controller. We'll also cover how to use `$http` to fetch data from a live API. 

Live example: <a href="#">Click Me!</a>

## Step 1

### Summary

In this step, we'll create a service file and move the local user data from the controller into it.

### Instructions

* Create a new javascript file called `service.js` in `js/`.
* Open `js/service.js`.
* Create a new Angular service called `mainService`.
* Open `js/controller.js` and copy the value of `$scope.users` and then delete `$scope.users`.
* In `js/service.js` create a new variable called `data` and paste the value from your clipboard. 

### Solution

<details>

<summary> <code> js/controller.js </code> </summary>

```js
angular.module('userProfiles').controller('MainController', function($scope) {

});
```

</details>

<details>

<summary> <code> js/service.js </code> </summary>

```js
angular.module('userProfiles').service('mainService', function() {
  var data = [
    {
      "id": 0,
      "first_name": "george",
      "last_name": "bluth",
      "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/calebogden/128.jpg"
    },
    {
      "id": 1,
      "first_name": "lucille",
      "last_name": "bluth",
      "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/josephstein/128.jpg"
    },
    {
      "id": 2,
      "first_name": "oscar",
      "last_name": "bluth",
      "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/olegpogodaev/128.jpg"
    }
  ];
});
```

</details>

## Step 2

### Summary

In this step, we'll add a method to the service that provides the local user data. We'll then update the controller to use this service method.

### Instructions

### Solution

## Step 3

### Summary

In this step, we'll modify the service to use `$http` to get data from a live API.

### Instructions

### Solution

## Contributions

If you see a problem or a typo, please fork, make the necessary changes, and create a pull request so we can review your changes and merge them into the master repo and branch.

## Copyright

© DevMountain LLC, 2017. Unauthorized use and/or duplication of this material without express and written permission from DevMountain, LLC is strictly prohibited. Excerpts and links may be used, provided that full and clear credit is given to DevMountain with appropriate and specific direction to the original content.

<p align="center">
<img src="https://devmounta.in/img/logowhiteblue.png" width="250">
</p>
 

