This Okta Login template is using the low-level okta-auth-js library. This library allows you to have full control over your HTML and just handles communication with Okta’s API. All of Okta’s JavaScript libraries are built on top of okta-auth-js.

## Tutorial:
https://developer.okta.com/blog/2020/01/21/angular-material-login#add-secure-sign-in-to-your-angular-app

https://github.com/oktadeveloper/okta-angular-material-login-example

## Add Angular Material
https://material.angular.io/guide/getting-started

`ng add @angular/material`

## Add components
`ng generate component toolbar`

`ng generate component home`

## Add Secure Sign In

`npm install -E @okta/okta-auth-js`

`ng generate service Auth`

`ng generate component login`

`ng generate service AuthGuard`

`ng generate component game`
