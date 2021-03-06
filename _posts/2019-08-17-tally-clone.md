---
title: 'Tally Clone'
date: 2019-07-17
tags: [angular, firebase, business, javascript]
---

This is a accounting web app that can serve the purpose of tally. This is developed with angular and firebase. [View Demo](https://tally-clone.firebaseapp.com/)

## Get Started

#### Install Dependencies

- Install Your Project Dependencies

  ```bash
  npm install
  ```

- Install Firebase Depndencies

  ```bash
  cd firebase/functions
  npm install
  ```

#### Step Up Firebase Related Stuff:-

- Make a file src/environments/firebase.ts and add your firebase credentials in that file:-

  ```ts
  export const firebase = {your credentials}
  ```

#### Setup Firebase Functions and Firestore rules:-

- Install [firebase cli client](https://firebase.google.com/docs/cli) and login with your account.

- Make Your Firebase Project in firebase console.

- Make a file firebase/.firebaserc and add the following and replace your-project-name with your project name:-

  ```json
  { "projects": { "default": "your-project-name" } }
  ```

- Deploy Your Firebase Functions and Firestore Rules.

  ```bash
  firebase deploy --only functions
  firebase deploy --only firestore
  ```

#### Test Your Project :-

- Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

##### And You are done.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Deploy Web App to firebase Hosting

Run `npm run deploy` And It will deploy a production version to firebase hosting and you will be running the web app on the firebase.
