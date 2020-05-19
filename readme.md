# staticweb-aurelia

This project is bootstrapped by [aurelia/new](https://github.com/aurelia/new).

## Start dev web server

    npm start

## Build the app

Build files to dist folder.

    npm run build

## Unit Tests

    npm run test

Run unit tests in watch mode.

    npm run test:watch



## Clear tracing cache

In rare situation, you might need to run clear-cache after upgrading to new version of dumber bundler.

    npm run clear-cache

## index.html

`index.html` is generated from `_index.html` every time `npm run build` runs. It is handled by dumber's `onManifest()` option, check `gulpfile.js` for details.


## Cypress e2e test

All e2e tests are in `cypress/integration/`.
Note the source code of the app and unit tests is in TypeScript, but e2e tests are in plain ESNext JavaScript. You can however [write e2e tests in TypeScript too for Cypress](https://docs.cypress.io/guides/tooling/typescript-support.html#Transpiling-TypeScript-test-files).

First, run the app in dev mode

    npm start

Then run e2e tests in another terminal window with

    npm run test:e2e

Note if your dev app is not running on port 9000, you need to modify `cypress.json` to update dev app port.

To run Cypress interactively, do

    npx cypress open

For more information, visit https://www.cypress.io
