# Decoupled D8 with React.js
* Why Decoupled?
  * use cases
    * offline capabilities - entire site
    * sales people, doing demos, no internet
    * doctor - getting information, not wanting to wait for internet
  * site deployed to web, just for editors
  * native mobile apps using API
* tech
  * D8 - modules
    * **deploy** module
    * Multiversion
    * Replication
    * Workspace
    * RELAXed
      * extends REST api that replicates easily
      * CouchDB
  * CouchDB
    * native to HTTP
  * PouchDB
    * offline version of CouchDB
    * javascript - can run in browser
  * ReactJS
    * components that get data
    * redux - unidirectional flow
* Architecture
  * D8 > RELAXed module/CouchDB > PouchDB > ReactJS
