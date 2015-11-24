# Admin SPA

## Contents

* [Install](#install)
* [Structure](#structure)
* [Scripts](#scripts)
* [JavaScript](#javascript)
* [CSS](#css)

## Prerequisites
We require some ruby gems to build the blog pages. This might need to be run with sudo but depends on how you've ruby setup locally.

### Jeckyll 
``` gem install jeckyll ```

### Bundler
``` gem install bundler ```


## Install

``` bundle install && npm install ```


## Structure

* lib/ - all application code
* less/ - all styling code
* www/ - files available via HTTP (includes compiled code)


## Scripts

### npm start
Starts the node server

### npm run start:dev
Starts the node server in development

### npm run build
Compiles production code

* build:js - builds javascript for UI
* build:css - builds css for UI


## JavaScript
All JavaScript is written with ES6 using Babel as a transpiler for browsers which
do not support features out-of-the-box. We use browserify to build a single file
of JavaScript for local caching and Application Cache for offline support.


## CSS
We use LESS as a CSS preprocessor with Autoprefixer to provide CSS3 support across
all browsers without notation.  