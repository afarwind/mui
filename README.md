# MUI

[![Join the chat at https://gitter.im/amorey/mui](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/amorey/mui?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

[![Documentation](https://www.muicss.com/static/favicons/icon-192x192.png)](https://www.muicss.com)

A lightweight HTML/CSS/JS framework for sites that follow Google's Material Design guidelines.

[![Build Status](https://travis-ci.org/amorey/mui.svg?branch=master)](https://travis-ci.org/amorey/mui)
[![Dependency Status](https://david-dm.org/amorey/mui.svg)](https://david-dm.org/amorey/mui)
[![devDependency Status](https://david-dm.org/amorey/mui/dev-status.svg)](https://david-dm.org/amorey/mui#info=devDependencies)

**Use From the CDN:**

```html
<link href="//cdn.muicss.com/mui-0.0.8/css/mui.min.css" rel="stylesheet" type="text/css" />
<script src="//cdn.muicss.com/mui-0.0.8/js/mui.min.js"></script>
```

***Install with Bower:**

```shell
$ bower install mui
```

## Development Dependencies

* nodejs (http://nodejs.org/)
* npm (https://www.npmjs.org/)
* bower (http://bower.io/)
* sass (http://sass-lang.com/)
* http-server (via npm)

## Development Quickstart

1. Clone repository

   ```bash
   $ git clone git@github.com:amorey/mui.git
   $ cd mui
   ```

1. Install node dependencies using npm

   ```bash
   $ npm install
   ```

1. Install bower dependencies

   ```bash
   $ bower install
   ```

1. Build examples

   ```bash
   $ ./node_modules/.bin/gulp build-examples
   ```

   To view the examples you can use any static file server. To use the nodejs `http-server` module:

   ```bash
   $ npm install http-server
   $ ./node_modules/.bin/http-server -p 3000
   ```

   Then visit http://localhost:3000/examples

1. Watch changes and re-build

   ```bash
   $ ./node_modules/.bin/gulp watch
   ```

## Run tests

### Unit tests

To run the unit tests from the command line, run 'mocha':

```bash
$ ./node_modules/.bin/mocha
```

### E2E tests

To run the E2E tests first compile the unit test files into a version that runs in the browser:

```bash
$ ./node_modules/.bin/gulp build-e2e-tests
```

Then visit http://localhost:3000/e2e-tests

## Create a production build

To create a production build of the app, run `gulp build-dist`:

```bash
$ ./node_modules/.bin/gulp build-dist
```

The build will be located in the `dist` directory:

<pre>
dist/
├── css
│   ├── mui.css
│   └── mui.min.css
├── email
│   ├── mui-email-inline.css
|   └── mui-email-styletag.css
├── js
│   ├── mui.js
│   └── mui.min.js
├── react
│   ├── mui-react.js
│   └── mui-react.min.js
└── webcomponents
    ├── mui-webcomponents.js
    └── mui-webcomponents.min.js
</pre>
