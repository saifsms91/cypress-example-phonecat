# Phonecat [![Build status][ci-image] ][ci-url][![Build status](https://ci.appveyor.com/api/projects/status/i5jmxcm0d36o1yef?svg=true)](https://ci.appveyor.com/project/cypress-io/cypress-example-phonecat) [![renovate-app badge][renovate-badge]][renovate-app]

[ci-image]: https://circleci.com/gh/cypress-io/cypress-example-phonecat/tree/master.svg?style=svg
[ci-url]: https://circleci.com/gh/cypress-io/cypress-example-phonecat/tree/master

This repo contains a forked version of [the original  Angular Phonecat example app](https://github.com/angular/angular-phonecat) with the e2e tests written in Cypress.

The Cypress tests match up 1:1 so they can be directly compared to the [original e2e protractor tests](e2e-tests/scenarios.js).

Each test covers the same functionality found in the protractor tests, and additionally new tests have been added to showcase functionality that exists only in Cypress.

The [tests are heavily commented](cypress/integration/app_spec.js) to ease you into the Cypress API.

Read [Angular + Cypress = Love](https://www.cypress.io/blog/2018/03/20/angular-cypress-love/) and [An Alternative to Protractor for Angular Projects](https://www.cypress.io/blog/2017/12/11/an-alternative-to-protractor-for-angular-projects/)

## Help + Testing

The steps below will take you all the way through Cypress. It is assumed you have nothing installed except for node + git.

**If you get stuck, here is more help:**

* [Cypress Support](https://on.cypress.io/support)

### 1. Install Cypress

[Follow these instructions to install Cypress.](https://on.cypress.io/installing-cypress)

### 2. Fork this repo

If you want to experiment with running this project in Continuous Integration, you'll need to [fork](https://github.com/cypress-io/cypress-example-phonecat#fork-destination-box) it first.

After forking this project in `Github`, run these commands:

```bash
## clone this repo to a local directory
git clone https://github.com/<your-username>/cypress-example-phonecat.git

## cd into the cloned repo
cd cypress-example-phonecat

## install the node_modules
npm install

## start the local webserver
npm start
```

The `npm start` script will spawn a webserver on port `8000` which hosts the Phonecat app.

You can verify this by opening your browser and navigating to: [`http://localhost:8000`](http://localhost:8000)

You should see the Phonecat app up and running. We are now ready to run Cypress tests.

### 3. Add the project to Cypress

[Follow these instructions to add the project to Cypress.](https://on.cypress.io/writing-your-first-test)

### 4. Run in Continuous Integration

[Follow these instructions to run the tests in CI.](https://on.cypress.io/continuous-integration)

[renovate-badge]: https://img.shields.io/badge/renovate-app-blue.svg
[renovate-app]: https://renovateapp.com/
