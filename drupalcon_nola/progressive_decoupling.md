# Next-level Drupal: Progressive decoupling with JS
* risks and rewards for decoupling
  * decoupled: using a different front end than drupals
  * dynamic pages with rerendering
  * separation of concerns: data structure vs presentation
  * write once, publish everywhere
  * rich ecosystem
  * risks
    * additional point of failure, multi-servers
    * no automatic input sanitization
    * no in-place editing
    * no layout and display management
    * no accessible markup
    * no BigPipe cache tags
* When should you do it?
  * if you have a pre-existing drupal site, one that powers applications
  * better solution **progressive decoupling**
* Progressive decoupling
  * Use JS framework *with* drupal front-end
  * rewards
    * no additional point of failure
    * all input sanitization still there
    * all drupal front-end benefits still there
  * 
