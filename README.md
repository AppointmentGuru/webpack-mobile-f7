# vue-webpack-boilerplate

> A full-featured Webpack setup with Cordova, Framework7, hot-reload, lint-on-save, unit testing & css extraction.

> This template is Vue 2.0 compatible.

![Preview](http://blog.toast38coza.me/content/images/2017/01/Screen-Shot-2017-01-13-at-9.05.12-AM.png)

## Documentation

- [For this template](http://vuejs-templates.github.io/webpack): common questions specific to this template are answered and each part is described in greater detail
- [For Vue 2.0](http://vuejs.org/guide/): general information about how to work with Vue, not specific to this template

## Usage

This is a project template for [vue-cli](https://github.com/vuejs/vue-cli). **It is recommended to use npm 3+ for a more efficient dependency tree.**

``` bash
$ npm install -g vue-cli
$ vue init AppointmentGuru/webpack-mobile-f7 my-project
$ cd my-project
$ npm install
$ npm run dev
```

**To run on the cordova platform**

(requires cordova (`npm install -g cordova`))

```bash
# add the platforms you need
cordova platform add browser ios android
# build
npm run cordova-build
# run on desired platform:
# browser
npm run cordova-run 
# ios
npm run cordova-run-ios
# android
npm run cordova-run-android
```

Note: the above commands combine a build of the VueJS project and the relevant cordova command. e.g.:

```bash
npm run build
cordova run browser
```

**NB:** To update the app that cordova is aware of, you need to build the Vue app with `npm run build`. This will clean and build the `www` folder. 

**Note:** for now, this only allows for the standard eslint option

## What's Included

- `npm run dev`: first-in-class development experience.
  - Webpack + `vue-loader` for single file Vue components.
  - State preserving hot-reload
  - State preserving compilation error overlay
  - Lint-on-save with ESLint
  - Source maps

- `npm run build`: Production ready build.
  - JavaScript minified with [UglifyJS](https://github.com/mishoo/UglifyJS2).
  - HTML minified with [html-minifier](https://github.com/kangax/html-minifier).
  - CSS across all components extracted into a single file and minified with [cssnano](https://github.com/ben-eb/cssnano).
  - All static assets compiled with version hashes for efficient long-term caching, and a production `index.html` is auto-generated with proper URLs to these generated assets.

- `npm run unit`: Unit tests run in PhantomJS with [Karma](http://karma-runner.github.io/0.13/index.html) + [Mocha](http://mochajs.org/) + [karma-webpack](https://github.com/webpack/karma-webpack).
  - Supports ES2015 in test files.
  - Supports all webpack loaders.
  - Easy mock injection.

- `npm run e2e`: End-to-end tests with [Nightwatch](http://nightwatchjs.org/).
  - Run tests in multiple browsers in parallel.
  - Works with one command out of the box:
    - Selenium and chromedriver dependencies automatically handled.
    - Automatically spawns the Selenium server.

### Fork It And Make Your Own

You can fork this repo to create your own boilerplate, and use it with `vue-cli`:

``` bash
vue init username/repo my-project
```
