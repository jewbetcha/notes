# AMPing up Drupal
* Mobile only - a way to make the mobile experience faster
* speed
  * goal - make pages load instantly everywhere
  * 4x faster
  * 10x less data
  * google prefers these pages = big benefit to SEO
* Google - Accelerated Mobile Pages project 2015
  * open source
  * Apache 2
* 3 parts of AMP
  * AMP HTML
    * loads in any browser
    * `<link rel="amphtml"`
    * `<amp-img>`, `<amp-video>`
    * AMP CSS - inline, max size 50kb
  * AMP JS
    * no author-written JS or 3rd party
  * Google AMP Cache
    * free CDN from Google
    * very fast
    * built in validation

### How to implement in drupal?
* `/url/path?amp` serves amp page
  * AMP view mode
  * AMP theme
* what do I need?
  * AMP module
    * d.o
    * D 7/8
    * PHP 5.5+
    * special field formatters
    * field templates and JS
    * takes in the url query
  * AMP theme
    * d.o
    * D 7/8
    * sitewide markup
    * styles
  * AMP library
    * **lullabot github**
    * process text fields
    * final pass of full HTML
  * Composer manger
  * Drush
  * Library + theme then module

### How to configure??
* view modes for each content type
* select amp theme
  * base theme sets up defaults
  * ExAMPle subtheme
  * create your own
* configure your block layout
* analytics
  * `amp-pixel` for tracking
* test & validate

### What are concerns?
* why take the effort?
  * speed matters
* no more m.site!
* different view, same content, like RSS
