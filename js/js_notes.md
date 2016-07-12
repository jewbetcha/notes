# JS Self Quiz

* what is typeof 'null'?
  * object/null
* what is a way to prevent bad syntax and write secure JS?
  * 'use strict' mode
* what are the parameters of jQuery AJAX calls?
  * url
  * type
  * dataType
  * success
  * error
  * async
  * ex:
  ```
  $.ajax({
      url: "google.com",
      type: "GET",
      dataType: "JSON",
      async: true,
      success: function (data) {
        console.log(data)
      },
      error: function (response) {
        var res = jQuery.parseJSON(response.responseText);
        console.log(res);
      }
    });
  ```
* what is a JS closure?
  * a function defined inside another function, and has access to variables that are declared and defined in the parent function scope
  * ex:
  ```
  function outer() {
      var name = "Bob";
      function inner() {
          console.log(name);    // 'Bob'
      }
      return inner;
  }
  var something = outer();
  something();     // 'Bob'
  ```
* what is a JS prototype?
  * all JS objects inherit properties and methods from their prototype. create an object prototype with a constructor function.
  * ex:
  ```
  function Person(first, last, age, eyecolor) {
      this.firstName = first;
      this.lastName = last;
      this.age = age;
      this.eyeColor = eyecolor;
  }
  ```
* More study stuff https://github.com/dxhackers/JSStudyGuide
