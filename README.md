# The Angular Full-Stack Generator

![](.gitbook/assets/angular-fullstack-logo.svg)

![Build Status](https://img.shields.io/circleci/project/angular-fullstack/generator-angular-fullstack/master.svg) [![npm version](https://img.shields.io/npm/v/generator-angular-fullstack.svg)](https://www.npmjs.com/package/generator-angular-fullstack) [![Dependency Status](https://img.shields.io/david/angular-fullstack/generator-angular-fullstack.svg)](https://david-dm.org/angular-fullstack/generator-angular-fullstack) [![Dev-Dependency Status](https://img.shields.io/david/dev/angular-fullstack/generator-angular-fullstack.svg)](https://david-dm.org/angular-fullstack/generator-angular-fullstack#type=dev) [![Gitter chat](https://img.shields.io/gitter/room/angular-fullstack/generator-angular-fullstack.svg)](https://gitter.im/angular-fullstack/generator-angular-fullstack)

> Yeoman generator for creating MEAN/SEAN stack applications, using ES2017, MongoDB/SQL, Express, Angular, and Node - lets you quickly set up a project following best practices.

### Generated project:

[![Dependency Status](https://img.shields.io/david/angular-fullstack/angular-fullstack-deps.svg)](https://david-dm.org/angular-fullstack/angular-fullstack-deps) [![Dev-Dependency Status](https://img.shields.io/david/dev/angular-fullstack/angular-fullstack-deps.svg)](https://david-dm.org/angular-fullstack/angular-fullstack-deps?type=dev) [![Known Vulnerabilities](https://snyk.io/package/npm/angular-fullstack-deps/badge.svg)](https://snyk.io/package/npm/angular-fullstack-deps)

## Usage

Install `yo`, `gulp-cli`, and `generator-angular-fullstack`:

```text
npm install -g yo gulp-cli generator-angular-fullstack
```

**Please note**: If you run into trouble compiling native add-ons during the installation, follow [`node-gyp`](https://github.com/nodejs/node-gyp)'s short guide on [required compilation tools](https://github.com/nodejs/node-gyp#installation).

Then, to run your app \(make sure the MongoDB daemon is running if you selected Mongo\), run the following to start your server:

```bash
npm run start:server
```

and the following to start the Webpack dev server for the front-end:

```bash
npm run start:client
```

The Webpack server will tell you which port to access the app at \(usually [http://localhost:8080/](http://localhost:8080/)\).

Run `yo angular-fullstack`

```text
yo angular-fullstack
```

**See the** [**Getting Started**](https://angular-fullstack.github.io/get-started/) **guide for more information.**

## Prerequisites.

* MongoDB - Download and Install [MongoDB](https://www.mongodb.com/download-center#community) - If you plan on scaffolding your project with mongoose, you'll need mongoDB to be installed and have the `mongod` process running.
  * If you have [Docker](https://www.docker.com/) installed, you can easily run a test database with `docker run -p 27017:27017 --name afs-mongo -d mongo`
* The project's JavaScript is written in ECMAScript 2015. If you're unfamiliar with the latest changes to the specification for JavaScript, check out [http://es6-features.org/](http://es6-features.org/)

## Supported Configurations

**General**

* Build Systems: `Gulp`
* Testing: 
  * `Jasmine`
  * `Mocha + Chai + Sinon`
    * Chai assertions:
      * `Expect`
      * `Should`

**Client**

* Scripts: `JavaScript (Babel)`, `TypeScript`
* Module Systems: `Webpack`
* Markup:  `HTML`, `Pug`
* Stylesheets: `CSS`, `Stylus`, `Sass`, `Less`
* CSS Frameworks: `Bootstrap`
  * Option to include `UI Bootstrap`

**Server**

* Scripts: `JavaScript (Babel)`, `TypeScript` \(planned\)
* Database:
  * `None`,
  * `MongoDB`, `SQL`
    * Authentication boilerplate: `Yes`, `No`
    * oAuth integrations: `Facebook`, `Twitter`, `Google`
    * Socket.io integration: `Yes`, `No`

## Generators.

Available generators:

* App
  * [angular-fullstack](https://angular-fullstack.github.io/generators/app/) \(aka [angular-fullstack:app](https://angular-fullstack.github.io/generators/app/)\)
* Server Side
  * [angular-fullstack:endpoint](https://angular-fullstack.github.io/generators/endpoint)
* Client Side \(via [generator-angular-fullstack-component](https://github.com/angular-fullstack/generator-angular-fullstack-component)\)
  * [angular-fullstack:route](https://angular-fullstack.github.io/generators/route)
* To be re-updated:
  * [angular-fullstack:component](https://angular-fullstack.github.io/generators/component)
  * [angular-fullstack:controller](https://angular-fullstack.github.io/generators/controller)
  * [angular-fullstack:filter](https://angular-fullstack.github.io/generators/filter)
  * [angular-fullstack:directive](https://angular-fullstack.github.io/generators/directive)
  * [angular-fullstack:service](https://angular-fullstack.github.io/generators/service)
  * [angular-fullstack:provider](https://angular-fullstack.github.io/generators/service)
  * [angular-fullstack:factory](https://angular-fullstack.github.io/generators/service)
  * [angular-fullstack:decorator](https://angular-fullstack.github.io/generators/decorator)
* Deployment
  * [angular-fullstack:openshift](https://angular-fullstack.github.io/generators/openshift)
  * [angular-fullstack:heroku](https://angular-fullstack.github.io/generators/heroku)

## Documentation.

Check out our [documentation home page](https://awk34.gitbook.io/generator-angular-fullstack).

## Contribute.

See the [contributing docs](https://github.com/angular-fullstack/generator-angular-fullstack/blob/master/contributing.md)

When submitting an issue, please follow the [Yeoman issue guidelines](https://github.com/yeoman/yeoman/blob/master/contributing.md#issue-submission). Especially important is to make sure Yeoman is up-to-date, and providing the command or commands that cause the issue, as well as any stack traces.

## License.

[BSD license](http://opensource.org/licenses/bsd-license.php)

[![generator-angular-fullstack](https://angular-fullstack.github.io/assets/angular-fullstack-boxes.svg)](https://awk34.gitbook.io/generator-angular-fullstack)

