# Building rich apps with Angular 2 and Drupal
* Angular
  * aims to simplify testing/development
  * lets developers run code on the visitors browser or server, eliminate page refreshes
* Ng2
  * in RC status
  * framework to platform
  * ng1 lacked guidelines to keep it maintainable
  * CLI
  * Augury, material design,
  * shift to typescript/ES6
* Angular universal
  * server-side code
  * sensitive to setup for devs and specific needs
  * payload sensitive
* Loading Angular within Drupal
  * native approach demo
    * ng2 renders comments
    * module determines library dependencies
      * dependencies go in `yml` file
    * bootstrap application
    * render components
      * ng2 components
  * Progressively Decoupled blocks demo
    * only loads framework if you have a component block on the page
* The Future
  * clone PDB (decoupled blocks) repo into modules folder
  * find examples in there
  * build components
* Progressive web app (google)
  * allows browser to use the site as an application
* @stephenfluin 
