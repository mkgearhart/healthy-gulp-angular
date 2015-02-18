This project is a starting point for AngularJS projects using the [Gulp](http://gulpjs.com/) streaming build system. Almost everything important is in [gulpfile.js](https://github.com/paislee/healthy-gulp-angular/blob/master/gulpfile.js).

For a full discussion of the setup, please refer to the companion [blog post](http://paislee.io/a-healthy-gulp-setup-for-angularjs-projects).

## Installation

Before running any Gulp tasks:

1. Check out this repository
2. Ensure you have node installed
3. Run `npm install` in the root directory (this will install bower dependencies too)
4. For livereload functionality, install the [livereload Chrome extension](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei)

## Gulp Tasks

All of these are available from the command line:

__`gulp validate-partials`__ Checks html source files for syntax errors.

__`gulp validate-index`__ Checks index.html for syntax errors.

__`gulp build-partials-dev`__ Moves html source files into the dev environment.

__`gulp convert-partials-to-js`__ Converts partials to javascript using html2js.

__`gulp validate-devserver-scripts`__ Runs jshint on the dev server scripts.

__`gulp validate-app-scripts`__ Runs jshint on the app scripts.

__`gulp build-app-scripts-dev`__ Moves app scripts into the dev environment.

__`gulp build-app-scripts-prod`__ Concatenates, uglifies, and moves app scripts and partials into the prod environment.

__`gulp build-styles-dev`__ Compiles app sass and moves to the dev environment.

__`gulp build-styles-prod`__ Compiles and minifies app sass to css and moves to the prod environment.

__`gulp build-vendor-scripts-dev`__ Moves vendor scripts into the dev environment.

__`gulp build-vendor-scripts-prod`__ Concatenates, uglifies, and moves vendor scripts into the prod environment.

__`gulp build-index-dev`__ Validates and injects sources into index.html and moves it to the dev environment.

__`gulp build-index-prod`__ Validates and injects sources into index.html, minifies and moves it to the dev environment.

__`gulp build-app-dev`__ Builds a complete dev environment.

__`gulp build-app-prod`__ Builds a complete prod environment.

__`gulp clean-build-app-dev`__ Cleans and builds a complete dev environment.

__`gulp clean-build-app-prod`__ Cleans and builds a complete prod environment.

__`gulp watch-dev`__ Clean, build, and watch live changes to the dev environment.

__`gulp watch-prod`__ Clean, build, and watch live changes to the prod environment.

__`gulp`__ Default task builds for prod.