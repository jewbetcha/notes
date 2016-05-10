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
  * better solution: **progressive decoupling**
* Progressive decoupling
  * Use JS framework *with* drupal front-end
  * rewards
    * no additional point of failure
    * all input sanitization still there
    * all drupal front-end/UI benefits still there
* weather.com - progressive decoupling
  * interpolates angular components with panels
  * concerns
    * performance/caching
    * in-house front-end team
    * editorial team
  * performance/caching
    * split page into wrapper and panels
    * same wrapper from origin to everyone
    * client-side rendering using angular
  * front-end team
    * they want to write javascript
    * want to keep up with JS ecosystem
  * editorial team
    * want to create content
    * want to create new pages/layouts without having to go to devs
  * presentation framework
    * put components on pages
    * supports angular, PHP and static templates
  * why panels?
    * reusable panels
    * context
    * drag-drop
    * variants
* framework-agnostic progressive coupling
  * give JS devs flexibility
  * keep guard rails
  * preserve strong editorial experience
* **Decoupled blocks module**
  * supports angular 2 and React
  * built on top of blocks
  * on github
  * configure JS components in UI
  * will be framework agnostic
  * pathing of components is simple
  * components can be contextually aware
* Use cases
  * Commerce
  * User-driven content
