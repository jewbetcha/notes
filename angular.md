# AngularJS Notes

* use this config setting to improve performance by removing Angular debugging classes/dom elements
```app.config(['$compileProvider', function ($compileProvider) {
    $compileProvider.debugInfoEnabled(false);
  }]);```
* set `HTML5` mode to be able to use URL params without a #
```app.config(function($locationProvider) {
    $locationProvider.html5Mode(true);
  });```
