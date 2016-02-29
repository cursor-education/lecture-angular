# Angular 1.x

![](http://new.tinygrab.com/7020c0e8b075dac69e0da439ec6ad3a3f18bcf6a01.png)

## Intro

- Conventional (traditional) Web Applications
  - ![](http://new.tinygrab.com/7020c0e8b03d17dd0003089ae83719e30f670c2eaa.png)
   - full page reload with all nested resources
- SPA (Single Page Apps)
  - ![](http://new.tinygrab.com/7020c0e8b0d84eb0b09f17142b0827e236073d7a81.png)
   - one-page app, similar to a desktop application
   - no page refresh on page change   
   - dynamically load content
   - technologies
     - AJAX
     - Websockets
       - bidirectional stateful real-time client-server communication
       - over a single TCP connection
       - ![](http://orm-chimera-prod.s3.amazonaws.com/1230000000545/images/hpbn_1702.png)
     - Browser plugins (is outdated)
       - Silverlight, Flash, or Java applets
     - Data transport
       - XML, JSON and AJAX
        - client updates a partial area of the DOM
   - lifecycle
     - fully loaded in the initial page load
     - divided by small fragments (sections) of the page
     - actions & updates on each fragment of page

## Conceptual Overview
- is fully client-side SPA framework
- by Google, 2009
- ![](http://new.tinygrab.com/7020c0e8b009c1ab1600bcf42ef07b1ed32f40fb0e.png)
- https://angularjs.org/
- resolves problems
  - separate DOM manipulation & business logic (for testing purposes)
  - client & server parts are separated (for parallel development)
- includes
  - CRUD apps (data-binding, validation, routing, server communication, etc)
  - testing (end-to-end, mocks)
  - a
- lifecycle
  - ![](http://singlepageappbook.com/assets/overview.png)
   - compilation step creates pure HTML
   - browser re-renders into the live view
   - step is repeated for subsequent page views
   - (in server-side meaning - controller and model interact within a server process to produce new HTML views)
   - the controller and model state are maintained within the client browser
   - Therefore new pages are generated without any interaction with a server

## Angular
- Quick Start (\w example)
 - add external resource (angular cdn)
   - https://ajax.googleapis.com/ajax/libs/angularjs/1.5.0/angular.min.js
 - the basics (hello name)
   - https://jsfiddle.net/n4kkkm2q/
 - Add Some Control
   - 
- Installation
- View
 - is an projection of the model through the HTML template
 - when model changes the HTML view will be refreshed
- Templating
  - are written with HTML
  - contains Angular-specific elements and attributes
  - types
    - Directive interpolation & Markup
      - a markers on a DOM element (such as an attribute, element name, comment or CSS class), that tell AngularJS's HTML compiler to attach a specified behavior to that DOM element or even to transform the DOM element and its children
      - ngBind, ngModel, and ngClass
      - normalization process
        - cut "x-" & "data-"
        - cut ":", "-" and "_"
        - to camelCase
      - https://jsfiddle.net/nsrr123r/1/
      - @read https://docs.angularjs.org/guide/directive
    - Filter
      - {{ expression | filter }}
      - {{ expression | filter1 | filter2 | ... }}
      - {{ expression | filter1:argument1:argument2 | .. }}
      - {{ 1234 | number:2 }}
      - https://jsfiddle.net/yerps1cm/2/
    - Form control
- Bootstrap
  - the "ng-app" directive
  - the root element of our application
  - AngularJS script tag
  - Double-curly binding with an expression
  - {{'yet' + '!'}}
  - <p>1 + 2 = {{ 1 + 2 }}</p>
  - ![](https://docs.angularjs.org/img/guide/concepts-startup.png)
- Directives
 - ng-app
  - an root element
 - ng-bind
 - ng-model
  - for 2-way binding
 - ng-repeat
 - ng-class
  - ng-class="expression"
 - ng-controller
 - ng-repeat
 - ng-show & ng-hide
 - ng-submit
 - examples
    - in array - https://jsfiddle.net/w24dp9mn/1/
    - in object - https://jsfiddle.net/w24dp9mn/2/
    - add orderBy - https://jsfiddle.net/w24dp9mn/3/
    - add filter - https://jsfiddle.net/w24dp9mn/4/
    - add ng-click - https://jsfiddle.net/w24dp9mn/5/
    - add own filter - https://jsfiddle.net/w24dp9mn/8/
    - ng-class - https://jsfiddle.net/w24dp9mn/7/
- Two-way Data Binding
 - is an automatic way of updating the view whenever the model changes
- Controllers
- Scope
 - $scope / $rootScope
- Services
 - Constants & Values
 - Services
 - Factories
- Developing & Debugging
- Digest Cycle & Watches
 - The "watch"
- Form Validation
- Promises
 - Q and $q
 - The Deferred Object
 - Route Resolve
- Modules
- Directives

## Todo Simple Project
- add todo button - https://jsfiddle.net/dspk3u63/2/
- print todos - https://jsfiddle.net/dspk3u63/3/
- a

## Examples
- Hello World (https://www.youtube.com/watch?v=uFTFsKmkQnQ)
- ToDo (https://www.youtube.com/watch?v=WuiHuZq_cg4)

## Read & Watch
 - http://www.angularbasics.co.uk/#
 - https://egghead.io/technologies/angularjs
