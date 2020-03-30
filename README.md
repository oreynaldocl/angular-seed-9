# MyApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.1.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## Creation
```sh
ng new my-app --routing=true --style=scss
```

## Bootstrap files
Install the following library
```sh
npm install --save @ng-bootstrap/ng-bootstrap@6.0.2 bootstrap@4.4.1
```

Create the following files
```
|- src/
    |- scss/
        |- _variables.scss
        |- _mixins.scss
        |- _styles.scss
```
Add following lines in `src/styles.scss`
```SCSS
// LIBRARIES
@import "~bootstrap/dist/css/bootstrap.css";

// CUSTOM SCSS
@import './scss/variables';
@import './scss/styles';
```

## FontAwesome files
Install font awesome library. 
```sh
npm install --save @fortawesome/fontawesome-free
```
Add following file with this content:
```SCSS
// Allows overriding Font Awesome variables https://github.com/FortAwesome/Font-Awesome/blob/master/web-fonts-with-css/scss/_variables.scss

// For loadiong the Web Fonts based on an absolute route instead of a relative route
$fa-font-path: "~@fortawesome/fontawesome-free/webfonts";

// Importing main Font Awesome scss library
@import "~@fortawesome/fontawesome-free/scss/fontawesome.scss";

// Importing Font Awesome Web Fonts
@import "~@fortawesome/fontawesome-free/scss/solid.scss";
@import "~@fortawesome/fontawesome-free/scss/regular.scss";
@import "~@fortawesome/fontawesome-free/scss/brands.scss";
```
Add following lines in `src/styles.scss`
```SCSS
// LIBRARIES
@import "~bootstrap/scss/bootstrap.scss";
@import "./scss/font-awesome/font-awesome";
```
