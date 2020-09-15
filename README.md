# NgMaterialOktaTemplate

This is a skeleton and an entry point which you can use to develop Angular apps with Google's Material Design and the single-sign-on service Okta.

You can view a demo [here](https://ng-material-okta-template.web.app).

Just clone this repository. In auth.service.ts file fill in your Okta app parameters you created for this app. Then use 'npm install' to get ready to develop your app.

What do you get here? A login form, which uses Okta's authentication service, and a navigation bar where you can add further components which are guarded by Okta. All visually set up with Angular Material design with default style cheat.

## Table of contents
- [What is Angular Material](#What-is-Angular-Material)
- [What is Okta](#What-is-Okta)
- [Set up your development environment](#Set-up-your-development-environment)
- [Used app versions and dependencies](#Used-app-versions-and-dependencies)
- [Start a development server](#Development-server)
- [Code scaffolding](#Code-scaffolding)
- [Build](#Build)
- [Running unit tests](#Running-unit-tests)
- [Running end-to-end tests](#Running-end-to-end-tests)
- [Get more info and further help](#Get-more-info-and-further-help)
- [Shell commands and things I used to build this skeleton app](#Shell-commands-and-things-I-used-to-build-this-skeleton-app)

---

## What is Angular Material

Material Design is an UI JavaScript library with which you can create a common user experience across Android devices and web applications. It consists of a number of components that are available for both Android and JavaScript applications.

## What is Okta

Many modern applications make use of single-sign-on services such as Okta. In its default configuration, Okta will redirect the user to a hosted login page. And after a successful sign-in Oktra redirects the user back to the application.

This Okta Login template is using the low-level okta-auth-js library. This library allows you to have full control over your HTML and just handles communication with Okta’s API. All of Okta’s JavaScript libraries are built on top of okta-auth-js.

## Set up your development environment

- Install the latest Node.js LTS version which also comes with npm.
- Open a shell and navigate to the project folder where you just git-cloned or downloaded this source code.
- Now run `npm install -g @angular/cli` to install Angular.
- In auth.service.ts file fill in your Okta app parameters you created for this app. You need an Okta developer account and created an app there to get the app's clientId and use your Okta-domain.
- At last run `npm install` to download and install all dependencies.

## Used app versions and dependencies

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 10.1.1.
- Angular CLI 10.1.1
- NodeJS 12.11.1
- @okta/okta-auth-js 4.0.0"
- @angular/material 10.2.0
- @angular/flex-layout 10.0.0

## Development server

Run `ng serve --open` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

~~~
ng build --prod
~~~

This production build which you can find in the `dist/` directory is ready for deployment. The files in the `dist/my-project-name` folder are static. This means you can host them on any web server capable of serving files (such as Node.js, Java, .NET), or any backend (such as Firebase, Google Cloud, or App Engine).

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Get more info and further help

The tutorials I used to build this app:

- https://developer.okta.com/blog/2020/01/21/angular-material-login#add-secure-sign-in-to-your-angular-app

- https://github.com/oktadeveloper/okta-angular-material-login-example

## Shell commands and things I used to build this skeleton app

~~~
## Install dependencies

`npm install -g @angular/cli@10.1.1`

`npm install -E @angular/material@10.2.0 @angular/cdk@10.2.0 @angular/flex-layout@10.0.0`

## Add Angular Material
https://material.angular.io/guide/getting-started

`ng add @angular/material`

Used an Angular Module (material-module.ts) to bundle and provide all Angular Material Elements to this app.

## Add components
`ng generate component toolbar`

`ng generate component home`

## Add Okta's Secure Sign In

`npm install -E @okta/okta-auth-js@4.0.0`

`ng generate service Auth`

`ng generate component login`

`ng generate service AuthGuard`

`ng generate component game`

~~~
