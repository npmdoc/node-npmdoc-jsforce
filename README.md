# npmdoc-jsforce

#### basic api documentation for  [jsforce (v1.7.2)](http://github.com/jsforce/jsforce)  [![npm package](https://img.shields.io/npm/v/npmdoc-jsforce.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jsforce) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jsforce.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jsforce)

#### Salesforce API Library for JavaScript

[![NPM](https://nodei.co/npm/jsforce.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jsforce)

- [https://npmdoc.github.io/node-npmdoc-jsforce/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jsforce/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jsforce/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jsforce/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jsforce/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jsforce/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Shinichi Tomita"
    },
    "bin": {
        "jsforce": "./bin/jsforce"
    },
    "browser": {
        "./index": "./lib/browser/jsforce",
        "./index.js": "./lib/browser/jsforce",
        "./core": "./lib/browser/core",
        "./core.js": "./lib/browser/core",
        "request": "./lib/browser/request.js"
    },
    "bugs": {
        "url": "https://github.com/jsforce/jsforce/issues"
    },
    "dependencies": {
        "co-prompt": "^1.0.0",
        "coffee-script": "^1.10.0",
        "commander": "^2.9.0",
        "csv-parse": "^1.1.1",
        "csv-stringify": "^1.0.4",
        "faye": "^1.2.0",
        "inherits": "^2.0.1",
        "lodash": "^4.11.1",
        "multistream": "^2.0.5",
        "open": "0.0.5",
        "promise": "^7.1.1",
        "readable-stream": "^2.1.0",
        "request": "^2.72.0",
        "xml2js": "^0.4.16"
    },
    "description": "Salesforce API Library for JavaScript",
    "devDependencies": {
        "archiver": "^1.0.0",
        "async": "^1.5.2",
        "babel": "^6.5.2",
        "babel-core": "^6.7.6",
        "babel-preset-es2015": "^6.5.0",
        "babel-register": "^6.5.2",
        "browserify": "^13.0.0",
        "dotenv": "^2.0.0",
        "envify": "^3.4.0",
        "espower-loader": "^1.0.0",
        "espowerify": "^1.0.0",
        "gulp": "github:gulpjs/gulp#4.0",
        "gulp-rename": "^1.2.2",
        "gulp-sourcemaps": "^1.6.0",
        "gulp-uglify": "^1.5.3",
        "intelli-espower-loader": "^1.0.1",
        "jsdoc": "^3.4.0",
        "mocha": "^2.4.5",
        "power-assert": "^1.3.0",
        "require-swapper": "^0.1.6",
        "testem": "^1.7.1",
        "through2": "^2.0.1",
        "vinyl-buffer": "^1.0.0",
        "vinyl-source-stream": "^1.1.0",
        "webdriverio": "^4.0.4"
    },
    "directories": {
        "test": "test/"
    },
    "dist": {
        "shasum": "03c8785d2f28e3fb7d6df1375fb4d3b148b00f7f",
        "tarball": "https://registry.npmjs.org/jsforce/-/jsforce-1.7.2.tgz"
    },
    "engines": {
        "node": ">=4.0"
    },
    "files": [
        "README.md",
        "bower.json",
        "LICENSE",
        "package.json",
        "bin",
        "build",
        "lib",
        "test",
        "core.js",
        "index.js"
    ],
    "gitHead": "4489c36558f609ef01e14bd2c18144fcb873adb4",
    "homepage": "http://github.com/jsforce/jsforce",
    "keywords": [
        "salesforce",
        "salesforce.com",
        "sfdc",
        "force.com",
        "database.com"
    ],
    "license": "MIT",
    "licenses": [
        {
            "type": "MIT",
            "url": "http://github.com/jsforce/jsforce/raw/master/LICENSE"
        }
    ],
    "main": "./index",
    "maintainers": [
        {
            "name": "stomita"
        }
    ],
    "name": "jsforce",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/jsforce/jsforce.git"
    },
    "scripts": {
        "build": "gulp build",
        "build:all": "gulp build:all",
        "build:test": "gulp build:test",
        "doc": "jsdoc lib -d doc --recurse --lenient",
        "prepublish": "node -e \"if(process.env.npm_package_version!==require('./lib/VERSION')){console.error('The pacakge.json version is not matching to ./lib/VERSION.js');process.exit(1)}\"",
        "test": "npm run test:node",
        "test:all": "npm run test:node && npm run test:browser",
        "test:browser": "testem",
        "test:node": "./test/bin/run-test"
    },
    "version": "1.7.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
