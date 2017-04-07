# api documentation for  [jsforce (v1.7.1)](http://github.com/jsforce/jsforce)  [![npm package](https://img.shields.io/npm/v/npmdoc-jsforce.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jsforce) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jsforce.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jsforce)
#### Salesforce API Library for JavaScript

[![NPM](https://nodei.co/npm/jsforce.png?downloads=true)](https://www.npmjs.com/package/jsforce)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jsforce/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-jsforce_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jsforce/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jsforce/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jsforce/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Shinichi Tomita",
        "email": "shinichi.tomita@gmail.com"
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
        "shasum": "b3a4adb3e946d05606f8e9978c4e5105833a7875",
        "tarball": "https://registry.npmjs.org/jsforce/-/jsforce-1.7.1.tgz"
    },
    "engines": {
        "node": ">=0.12.0"
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
    "gitHead": "e071c308250c39239bb484e9a516399c13dde018",
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
            "name": "stomita",
            "email": "shinichi.tomita@gmail.com"
        }
    ],
    "name": "jsforce",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "1.7.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jsforce](#apidoc.module.jsforce)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>Connection (options)](#apidoc.element.jsforce.Connection)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>Date (literal)](#apidoc.element.jsforce.Date)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>OAuth2 (options)](#apidoc.element.jsforce.OAuth2)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>Promise (fn)](#apidoc.element.jsforce.Promise)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>RecordStream ()](#apidoc.element.jsforce.RecordStream)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>RecordStream.Parsable ()](#apidoc.element.jsforce.RecordStream.Parsable)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>RecordStream.Serializable ()](#apidoc.element.jsforce.RecordStream.Serializable)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>RecordStream.super_ (options)](#apidoc.element.jsforce.RecordStream.super_)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>SfDate (literal)](#apidoc.element.jsforce.SfDate)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>cache ()](#apidoc.element.jsforce.cache)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>http_api (conn, options)](#apidoc.element.jsforce.http_api)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>logger (logLevel)](#apidoc.element.jsforce.logger)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>query (conn, config, options)](#apidoc.element.jsforce.query)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>quick_action (conn, path)](#apidoc.element.jsforce.quick_action)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>record (conn, type, id)](#apidoc.element.jsforce.record)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>require (name)](#apidoc.element.jsforce.require)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>soap (conn, options)](#apidoc.element.jsforce.soap)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>sobject (conn, type)](#apidoc.element.jsforce.sobject)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>transport ()](#apidoc.element.jsforce.transport)
1.  number <span class="apidocSignatureSpan">jsforce.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">jsforce.</span>Connection.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>OAuth2.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>Promise.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>RecordStream.Parsable.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>RecordStream.Serializable.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>RecordStream.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>RecordStream.super_.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>RecordStream.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>SfDate.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>_events
1.  object <span class="apidocSignatureSpan">jsforce.</span>_required
1.  object <span class="apidocSignatureSpan">jsforce.</span>cache.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>csv
1.  object <span class="apidocSignatureSpan">jsforce.</span>domain
1.  object <span class="apidocSignatureSpan">jsforce.</span>http_api.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>logger.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>query.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>quick_action.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>record.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>registry
1.  object <span class="apidocSignatureSpan">jsforce.</span>soap.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>sobject.prototype
1.  object <span class="apidocSignatureSpan">jsforce.</span>soql_builder
1.  object <span class="apidocSignatureSpan">jsforce.</span>transport.prototype
1.  string <span class="apidocSignatureSpan">jsforce.</span>VERSION

#### [module jsforce.Connection](#apidoc.module.jsforce.Connection)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>Connection (options)](#apidoc.element.jsforce.Connection.Connection)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.</span>super_ ()](#apidoc.element.jsforce.Connection.super_)

#### [module jsforce.Connection.prototype](#apidoc.module.jsforce.Connection.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>_baseUrl ()](#apidoc.element.jsforce.Connection.prototype._baseUrl)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>_normalizeUrl (url)](#apidoc.element.jsforce.Connection.prototype._normalizeUrl)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>authorize (code, callback)](#apidoc.element.jsforce.Connection.prototype.authorize)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>create (type, records, options, callback)](#apidoc.element.jsforce.Connection.prototype.create)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>del (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.del)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>delete (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.delete)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>deleted (type, start, end, callback)](#apidoc.element.jsforce.Connection.prototype.deleted)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>describe (type, callback)](#apidoc.element.jsforce.Connection.prototype.describe)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>describeGlobal (callback)](#apidoc.element.jsforce.Connection.prototype.describeGlobal)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>describeSObject (type, callback)](#apidoc.element.jsforce.Connection.prototype.describeSObject)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>destroy (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>identity (options, callback)](#apidoc.element.jsforce.Connection.prototype.identity)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>initialize (options)](#apidoc.element.jsforce.Connection.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>insert (type, records, options, callback)](#apidoc.element.jsforce.Connection.prototype.insert)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>limits (callback)](#apidoc.element.jsforce.Connection.prototype.limits)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>login (username, password, callback)](#apidoc.element.jsforce.Connection.prototype.login)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>loginByOAuth2 (username, password, callback)](#apidoc.element.jsforce.Connection.prototype.loginByOAuth2)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>loginBySoap (username, password, callback)](#apidoc.element.jsforce.Connection.prototype.loginBySoap)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>logout (callback)](#apidoc.element.jsforce.Connection.prototype.logout)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>logoutByOAuth2 (callback)](#apidoc.element.jsforce.Connection.prototype.logoutByOAuth2)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>logoutBySoap (callback)](#apidoc.element.jsforce.Connection.prototype.logoutBySoap)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>query (soql, options, callback)](#apidoc.element.jsforce.Connection.prototype.query)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>queryAll (soql, options, callback)](#apidoc.element.jsforce.Connection.prototype.queryAll)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>queryMore (locator, options, callback)](#apidoc.element.jsforce.Connection.prototype.queryMore)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>quickAction (actionName)](#apidoc.element.jsforce.Connection.prototype.quickAction)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>quickActions (callback)](#apidoc.element.jsforce.Connection.prototype.quickActions)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>recent (type, limit, callback)](#apidoc.element.jsforce.Connection.prototype.recent)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>request (request, options, callback)](#apidoc.element.jsforce.Connection.prototype.request)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestDelete (url, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestDelete)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestGet (url, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestGet)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestPatch (url, body, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestPatch)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestPost (url, body, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestPost)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestPut (url, body, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestPut)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>retrieve (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.retrieve)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>search (sosl, callback)](#apidoc.element.jsforce.Connection.prototype.search)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>sobject (type)](#apidoc.element.jsforce.Connection.prototype.sobject)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>tabs (callback)](#apidoc.element.jsforce.Connection.prototype.tabs)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>theme (callback)](#apidoc.element.jsforce.Connection.prototype.theme)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>update (type, records, options, callback)](#apidoc.element.jsforce.Connection.prototype.update)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>updated (type, start, end, callback)](#apidoc.element.jsforce.Connection.prototype.updated)
1.  [function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>upsert (type, records, extIdField, options, callback)](#apidoc.element.jsforce.Connection.prototype.upsert)

#### [module jsforce.OAuth2](#apidoc.module.jsforce.OAuth2)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>OAuth2 (options)](#apidoc.element.jsforce.OAuth2.OAuth2)

#### [module jsforce.OAuth2.prototype](#apidoc.module.jsforce.OAuth2.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>_postParams (params, callback)](#apidoc.element.jsforce.OAuth2.prototype._postParams)
1.  [function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>authenticate (username, password, callback)](#apidoc.element.jsforce.OAuth2.prototype.authenticate)
1.  [function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>getAuthorizationUrl (params)](#apidoc.element.jsforce.OAuth2.prototype.getAuthorizationUrl)
1.  [function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>refreshToken (refreshToken, callback)](#apidoc.element.jsforce.OAuth2.prototype.refreshToken)
1.  [function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>requestToken (code, callback)](#apidoc.element.jsforce.OAuth2.prototype.requestToken)
1.  [function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>revokeToken (accessToken, callback)](#apidoc.element.jsforce.OAuth2.prototype.revokeToken)

#### [module jsforce.Promise](#apidoc.module.jsforce.Promise)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>Promise (fn)](#apidoc.element.jsforce.Promise.Promise)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.</span>_61 ()](#apidoc.element.jsforce.Promise._61)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.</span>all (arr)](#apidoc.element.jsforce.Promise.all)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.</span>defer ()](#apidoc.element.jsforce.Promise.defer)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.</span>race (values)](#apidoc.element.jsforce.Promise.race)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.</span>reject (value)](#apidoc.element.jsforce.Promise.reject)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.</span>resolve (value)](#apidoc.element.jsforce.Promise.resolve)
1.  object <span class="apidocSignatureSpan">jsforce.Promise.</span>_10
1.  object <span class="apidocSignatureSpan">jsforce.Promise.</span>_97

#### [module jsforce.Promise.prototype](#apidoc.module.jsforce.Promise.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>catch (onRejected)](#apidoc.element.jsforce.Promise.prototype.catch)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>fail (onRejected)](#apidoc.element.jsforce.Promise.prototype.fail)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>then (onFulfilled, onRejected)](#apidoc.element.jsforce.Promise.prototype.then)
1.  [function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>thenCall (callback)](#apidoc.element.jsforce.Promise.prototype.thenCall)

#### [module jsforce.RecordStream](#apidoc.module.jsforce.RecordStream)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>RecordStream ()](#apidoc.element.jsforce.RecordStream.RecordStream)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Parsable ()](#apidoc.element.jsforce.RecordStream.Parsable)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Serializable ()](#apidoc.element.jsforce.RecordStream.Serializable)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>filter (fn)](#apidoc.element.jsforce.RecordStream.filter)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>map (fn)](#apidoc.element.jsforce.RecordStream.map)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>recordMapStream (record, noeval)](#apidoc.element.jsforce.RecordStream.recordMapStream)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>super_ (options)](#apidoc.element.jsforce.RecordStream.super_)
1.  object <span class="apidocSignatureSpan">jsforce.RecordStream.</span>DataStreamConverters

#### [module jsforce.RecordStream.Parsable](#apidoc.module.jsforce.RecordStream.Parsable)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Parsable ()](#apidoc.element.jsforce.RecordStream.Parsable.Parsable)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.</span>super_ ()](#apidoc.element.jsforce.RecordStream.Parsable.super_)

#### [module jsforce.RecordStream.Parsable.prototype](#apidoc.module.jsforce.RecordStream.Parsable.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.prototype.</span>addListener (ev, fn)](#apidoc.element.jsforce.RecordStream.Parsable.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.prototype.</span>on (ev, fn)](#apidoc.element.jsforce.RecordStream.Parsable.prototype.on)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.prototype.</span>stream (type, options)](#apidoc.element.jsforce.RecordStream.Parsable.prototype.stream)

#### [module jsforce.RecordStream.Serializable](#apidoc.module.jsforce.RecordStream.Serializable)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Serializable ()](#apidoc.element.jsforce.RecordStream.Serializable.Serializable)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.Serializable.</span>super_ ()](#apidoc.element.jsforce.RecordStream.Serializable.super_)

#### [module jsforce.RecordStream.Serializable.prototype](#apidoc.module.jsforce.RecordStream.Serializable.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.Serializable.prototype.</span>stream (type, options)](#apidoc.element.jsforce.RecordStream.Serializable.prototype.stream)

#### [module jsforce.RecordStream.prototype](#apidoc.module.jsforce.RecordStream.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.prototype.</span>_transform (record, enc, callback)](#apidoc.element.jsforce.RecordStream.prototype._transform)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.prototype.</span>filter (fn)](#apidoc.element.jsforce.RecordStream.prototype.filter)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.prototype.</span>map (fn)](#apidoc.element.jsforce.RecordStream.prototype.map)

#### [module jsforce.RecordStream.super_](#apidoc.module.jsforce.RecordStream.super_)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>super_ (options)](#apidoc.element.jsforce.RecordStream.super_.super_)

#### [module jsforce.RecordStream.super_.prototype](#apidoc.module.jsforce.RecordStream.super_.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>_read (n)](#apidoc.element.jsforce.RecordStream.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.prototype._transform)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.jsforce.RecordStream.super_.prototype.push)

#### [module jsforce.RecordStream.super_.super_.prototype](#apidoc.module.jsforce.RecordStream.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>cork ()](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>uncork ()](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>_writev

#### [module jsforce.SfDate](#apidoc.module.jsforce.SfDate)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>SfDate (literal)](#apidoc.element.jsforce.SfDate.SfDate)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_DAYS (num)](#apidoc.element.jsforce.SfDate.LAST_N_DAYS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_FISCAL_QUARTERS (num)](#apidoc.element.jsforce.SfDate.LAST_N_FISCAL_QUARTERS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_FISCAL_YEARS (num)](#apidoc.element.jsforce.SfDate.LAST_N_FISCAL_YEARS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_MONTHS (num)](#apidoc.element.jsforce.SfDate.LAST_N_MONTHS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_QUARTERS (num)](#apidoc.element.jsforce.SfDate.LAST_N_QUARTERS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_WEEKS (num)](#apidoc.element.jsforce.SfDate.LAST_N_WEEKS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_YEARS (num)](#apidoc.element.jsforce.SfDate.LAST_N_YEARS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_DAYS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_DAYS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_FISCAL_QUARTERS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_FISCAL_QUARTERS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_FISCAL_YEARS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_FISCAL_YEARS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_MONTHS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_MONTHS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_QUARTERS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_QUARTERS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_WEEKS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_WEEKS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_YEARS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_YEARS)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>parseDate (str)](#apidoc.element.jsforce.SfDate.parseDate)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>toDateLiteral (date)](#apidoc.element.jsforce.SfDate.toDateLiteral)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.</span>toDateTimeLiteral (date)](#apidoc.element.jsforce.SfDate.toDateTimeLiteral)
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_90_DAYS
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_FISCAL_QUARTER
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_FISCAL_YEAR
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_MONTH
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_QUARTER
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_WEEK
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_YEAR
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_90_DAYS
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_FISCAL_QUARTER
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_FISCAL_YEAR
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_MONTH
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_QUARTER
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_WEEK
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_YEAR
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>THIS_FISCAL_QUARTER
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>THIS_FISCAL_YEAR
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>THIS_MONTH
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>THIS_QUARTER
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>THIS_WEEK
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>THIS_YEAR
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>TODAY
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>TOMORROW
1.  object <span class="apidocSignatureSpan">jsforce.SfDate.</span>YESTERDAY

#### [module jsforce.SfDate.prototype](#apidoc.module.jsforce.SfDate.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.prototype.</span>toJSON ()](#apidoc.element.jsforce.SfDate.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">jsforce.SfDate.prototype.</span>toString ()](#apidoc.element.jsforce.SfDate.prototype.toString)

#### [module jsforce._required](#apidoc.module.jsforce._required)
1.  [function <span class="apidocSignatureSpan">jsforce._required.</span>inherits (ctor, superCtor)](#apidoc.element.jsforce._required.inherits)
1.  [function <span class="apidocSignatureSpan">jsforce._required.</span>multistream (streams, opts)](#apidoc.element.jsforce._required.multistream)
1.  [function <span class="apidocSignatureSpan">jsforce._required.</span>readable-stream (options)](#apidoc.element.jsforce._required.readable-stream)

#### [module jsforce.cache](#apidoc.module.jsforce.cache)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>cache ()](#apidoc.element.jsforce.cache.cache)

#### [module jsforce.cache.prototype](#apidoc.module.jsforce.cache.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>clear (key)](#apidoc.element.jsforce.cache.prototype.clear)
1.  [function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>get (key)](#apidoc.element.jsforce.cache.prototype.get)
1.  [function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>makeCacheable (fn, scope, options)](#apidoc.element.jsforce.cache.prototype.makeCacheable)
1.  [function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>makeResponseCacheable (fn, scope, options)](#apidoc.element.jsforce.cache.prototype.makeResponseCacheable)

#### [module jsforce.csv](#apidoc.module.jsforce.csv)
1.  [function <span class="apidocSignatureSpan">jsforce.csv.</span>parseCSV (str, options)](#apidoc.element.jsforce.csv.parseCSV)
1.  [function <span class="apidocSignatureSpan">jsforce.csv.</span>parseCSVStream (options)](#apidoc.element.jsforce.csv.parseCSVStream)
1.  [function <span class="apidocSignatureSpan">jsforce.csv.</span>serializeCSVStream (options)](#apidoc.element.jsforce.csv.serializeCSVStream)
1.  [function <span class="apidocSignatureSpan">jsforce.csv.</span>toCSV (records, options)](#apidoc.element.jsforce.csv.toCSV)

#### [module jsforce.http_api](#apidoc.module.jsforce.http_api)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>http_api (conn, options)](#apidoc.element.jsforce.http_api.http_api)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.</span>SessionRefreshDelegate (conn, refreshFn)](#apidoc.element.jsforce.http_api.SessionRefreshDelegate)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.</span>super_ ()](#apidoc.element.jsforce.http_api.super_)

#### [module jsforce.http_api.prototype](#apidoc.module.jsforce.http_api.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>beforeSend (request)](#apidoc.element.jsforce.http_api.prototype.beforeSend)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getError (response, body)](#apidoc.element.jsforce.http_api.prototype.getError)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getRefreshDelegate ()](#apidoc.element.jsforce.http_api.prototype.getRefreshDelegate)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getResponseBody (response)](#apidoc.element.jsforce.http_api.prototype.getResponseBody)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getResponseContentType (response)](#apidoc.element.jsforce.http_api.prototype.getResponseContentType)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>hasErrorInResponseBody (body)](#apidoc.element.jsforce.http_api.prototype.hasErrorInResponseBody)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>isErrorResponse (response)](#apidoc.element.jsforce.http_api.prototype.isErrorResponse)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>isSessionExpired (response)](#apidoc.element.jsforce.http_api.prototype.isSessionExpired)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>parseError (body)](#apidoc.element.jsforce.http_api.prototype.parseError)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>parseResponseBody (response)](#apidoc.element.jsforce.http_api.prototype.parseResponseBody)
1.  [function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>request (request, callback)](#apidoc.element.jsforce.http_api.prototype.request)

#### [module jsforce.logger](#apidoc.module.jsforce.logger)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>logger (logLevel)](#apidoc.element.jsforce.logger.logger)
1.  object <span class="apidocSignatureSpan">jsforce.logger.</span>LogLevels

#### [module jsforce.logger.prototype](#apidoc.module.jsforce.logger.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>debug (message)](#apidoc.element.jsforce.logger.prototype.debug)
1.  [function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>error (message)](#apidoc.element.jsforce.logger.prototype.error)
1.  [function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>fatal (message)](#apidoc.element.jsforce.logger.prototype.fatal)
1.  [function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>info (message)](#apidoc.element.jsforce.logger.prototype.info)
1.  [function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>log (level, message)](#apidoc.element.jsforce.logger.prototype.log)
1.  [function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>warn (message)](#apidoc.element.jsforce.logger.prototype.warn)

#### [module jsforce.query](#apidoc.module.jsforce.query)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>query (conn, config, options)](#apidoc.element.jsforce.query.query)
1.  [function <span class="apidocSignatureSpan">jsforce.query.</span>super_ (options)](#apidoc.element.jsforce.query.super_)
1.  object <span class="apidocSignatureSpan">jsforce.query.</span>ResponseTargets

#### [module jsforce.query.prototype](#apidoc.module.jsforce.query.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>_execute (options)](#apidoc.element.jsforce.query.prototype._execute)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>_expandFields ()](#apidoc.element.jsforce.query.prototype._expandFields)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>_read (size)](#apidoc.element.jsforce.query.prototype._read)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>addListener (e, fn)](#apidoc.element.jsforce.query.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>autoFetch (autoFetch)](#apidoc.element.jsforce.query.prototype.autoFetch)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>del (type, callback)](#apidoc.element.jsforce.query.prototype.del)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>delete (type, callback)](#apidoc.element.jsforce.query.prototype.delete)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>destroy (type, callback)](#apidoc.element.jsforce.query.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>exec (options, callback)](#apidoc.element.jsforce.query.prototype.exec)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>execute (options, callback)](#apidoc.element.jsforce.query.prototype.execute)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>explain (callback)](#apidoc.element.jsforce.query.prototype.explain)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>filter (fn)](#apidoc.element.jsforce.query.prototype.filter)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>include (childRelName, conditions, fields, options)](#apidoc.element.jsforce.query.prototype.include)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>limit (limit)](#apidoc.element.jsforce.query.prototype.limit)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>map (fn)](#apidoc.element.jsforce.query.prototype.map)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>maxFetch (maxFetch)](#apidoc.element.jsforce.query.prototype.maxFetch)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>offset (offset)](#apidoc.element.jsforce.query.prototype.offset)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>on (e, fn)](#apidoc.element.jsforce.query.prototype.on)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>orderby (sort, dir)](#apidoc.element.jsforce.query.prototype.orderby)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>run (options, callback)](#apidoc.element.jsforce.query.prototype.run)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>scanAll (scanAll)](#apidoc.element.jsforce.query.prototype.scanAll)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>select (fields)](#apidoc.element.jsforce.query.prototype.select)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>setResponseTarget (responseTarget)](#apidoc.element.jsforce.query.prototype.setResponseTarget)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>skip (offset)](#apidoc.element.jsforce.query.prototype.skip)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>sort (sort, dir)](#apidoc.element.jsforce.query.prototype.sort)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>stream (type, options)](#apidoc.element.jsforce.query.prototype.stream)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>then (onResolved, onReject)](#apidoc.element.jsforce.query.prototype.then)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>thenCall (callback)](#apidoc.element.jsforce.query.prototype.thenCall)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>toSOQL (callback)](#apidoc.element.jsforce.query.prototype.toSOQL)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>update (mapping, type, callback)](#apidoc.element.jsforce.query.prototype.update)
1.  [function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>where (conditions)](#apidoc.element.jsforce.query.prototype.where)

#### [module jsforce.quick_action](#apidoc.module.jsforce.quick_action)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>quick_action (conn, path)](#apidoc.element.jsforce.quick_action.quick_action)

#### [module jsforce.quick_action.prototype](#apidoc.module.jsforce.quick_action.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.quick_action.prototype.</span>defaultValues (contextId, callback)](#apidoc.element.jsforce.quick_action.prototype.defaultValues)
1.  [function <span class="apidocSignatureSpan">jsforce.quick_action.prototype.</span>describe (callback)](#apidoc.element.jsforce.quick_action.prototype.describe)
1.  [function <span class="apidocSignatureSpan">jsforce.quick_action.prototype.</span>execute (contextId, record, callback)](#apidoc.element.jsforce.quick_action.prototype.execute)

#### [module jsforce.record](#apidoc.module.jsforce.record)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>record (conn, type, id)](#apidoc.element.jsforce.record.record)

#### [module jsforce.record.prototype](#apidoc.module.jsforce.record.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>blob (fieldName)](#apidoc.element.jsforce.record.prototype.blob)
1.  [function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>del (options, callback)](#apidoc.element.jsforce.record.prototype.del)
1.  [function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>delete (options, callback)](#apidoc.element.jsforce.record.prototype.delete)
1.  [function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>destroy (options, callback)](#apidoc.element.jsforce.record.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>retrieve (options, callback)](#apidoc.element.jsforce.record.prototype.retrieve)
1.  [function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>update (record, options, callback)](#apidoc.element.jsforce.record.prototype.update)

#### [module jsforce.soap](#apidoc.module.jsforce.soap)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>soap (conn, options)](#apidoc.element.jsforce.soap.soap)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.</span>super_ (conn, options)](#apidoc.element.jsforce.soap.super_)

#### [module jsforce.soap.prototype](#apidoc.module.jsforce.soap.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>_createEnvelope (message)](#apidoc.element.jsforce.soap.prototype._createEnvelope)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>beforeSend (request)](#apidoc.element.jsforce.soap.prototype.beforeSend)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>getResponseBody (response)](#apidoc.element.jsforce.soap.prototype.getResponseBody)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>invoke (method, args, schema, callback)](#apidoc.element.jsforce.soap.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>isSessionExpired (response)](#apidoc.element.jsforce.soap.prototype.isSessionExpired)
1.  [function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>parseError (body)](#apidoc.element.jsforce.soap.prototype.parseError)

#### [module jsforce.sobject](#apidoc.module.jsforce.sobject)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>sobject (conn, type)](#apidoc.element.jsforce.sobject.sobject)

#### [module jsforce.sobject.prototype](#apidoc.module.jsforce.sobject.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>approvalLayouts (callback)](#apidoc.element.jsforce.sobject.prototype.approvalLayouts)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>bulkload (operation, options, input, callback)](#apidoc.element.jsforce.sobject.prototype.bulkload)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>compactLayouts (callback)](#apidoc.element.jsforce.sobject.prototype.compactLayouts)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>count (conditions, callback)](#apidoc.element.jsforce.sobject.prototype.count)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>create (records, options, callback)](#apidoc.element.jsforce.sobject.prototype.create)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>createBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.createBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>del (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.del)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>delete (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.delete)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>deleteBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.deleteBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>deleteHardBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.deleteHardBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>deleted (start, end, callback)](#apidoc.element.jsforce.sobject.prototype.deleted)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>describe (callback)](#apidoc.element.jsforce.sobject.prototype.describe)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>destroy (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>destroyBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.destroyBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>destroyHardBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.destroyHardBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>find (conditions, fields, options, callback)](#apidoc.element.jsforce.sobject.prototype.find)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>findOne (conditions, fields, options, callback)](#apidoc.element.jsforce.sobject.prototype.findOne)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>insert (records, options, callback)](#apidoc.element.jsforce.sobject.prototype.insert)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>insertBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.insertBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>layouts (layoutName, callback)](#apidoc.element.jsforce.sobject.prototype.layouts)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>listview (id)](#apidoc.element.jsforce.sobject.prototype.listview)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>listviews (callback)](#apidoc.element.jsforce.sobject.prototype.listviews)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>quickAction (actionName)](#apidoc.element.jsforce.sobject.prototype.quickAction)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>quickActions (callback)](#apidoc.element.jsforce.sobject.prototype.quickActions)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>recent (callback)](#apidoc.element.jsforce.sobject.prototype.recent)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>record (id)](#apidoc.element.jsforce.sobject.prototype.record)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>retrieve (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.retrieve)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>select (fields, callback)](#apidoc.element.jsforce.sobject.prototype.select)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>update (records, options, callback)](#apidoc.element.jsforce.sobject.prototype.update)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>updateBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.updateBulk)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>updated (start, end, callback)](#apidoc.element.jsforce.sobject.prototype.updated)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>upsert (records, extIdField, options, callback)](#apidoc.element.jsforce.sobject.prototype.upsert)
1.  [function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>upsertBulk (input, extIdField, callback)](#apidoc.element.jsforce.sobject.prototype.upsertBulk)

#### [module jsforce.soql_builder](#apidoc.module.jsforce.soql_builder)
1.  [function <span class="apidocSignatureSpan">jsforce.soql_builder.</span>createSOQL (query)](#apidoc.element.jsforce.soql_builder.createSOQL)

#### [module jsforce.transport](#apidoc.module.jsforce.transport)
1.  [function <span class="apidocSignatureSpan">jsforce.</span>transport ()](#apidoc.element.jsforce.transport.transport)
1.  [function <span class="apidocSignatureSpan">jsforce.transport.</span>CanvasTransport (signedRequest)](#apidoc.element.jsforce.transport.CanvasTransport)
1.  [function <span class="apidocSignatureSpan">jsforce.transport.</span>JsonpTransport (jsonpParam)](#apidoc.element.jsforce.transport.JsonpTransport)
1.  [function <span class="apidocSignatureSpan">jsforce.transport.</span>ProxyTransport (proxyUrl)](#apidoc.element.jsforce.transport.ProxyTransport)

#### [module jsforce.transport.prototype](#apidoc.module.jsforce.transport.prototype)
1.  [function <span class="apidocSignatureSpan">jsforce.transport.prototype.</span>_getHttpRequestModule ()](#apidoc.element.jsforce.transport.prototype._getHttpRequestModule)
1.  [function <span class="apidocSignatureSpan">jsforce.transport.prototype.</span>httpRequest (params, callback)](#apidoc.element.jsforce.transport.prototype.httpRequest)



# <a name="apidoc.module.jsforce"></a>[module jsforce](#apidoc.module.jsforce)

#### <a name="apidoc.element.jsforce.Connection"></a>[function <span class="apidocSignatureSpan">jsforce.</span>Connection (options)](#apidoc.element.jsforce.Connection)
- description and source-code
```javascript
Connection = function (options) {
  options = options || {};

  this._logger = new Logger(options.logLevel);

  var oauth2 = options.oauth2 || {
    loginUrl : options.loginUrl,
    clientId : options.clientId,
    clientSecret : options.clientSecret,
    redirectUri : options.redirectUri,
    proxyUrl: options.proxyUrl
  };

<span class="apidocCodeCommentSpan">  /**
   * OAuth2 object
   * @member {OAuth2} Connection#oauth2
   */
</span>  this.oauth2 = oauth2 = oauth2 instanceof OAuth2 ? oauth2 : new OAuth2(oauth2);

  this.loginUrl = options.loginUrl || oauth2.loginUrl || defaults.loginUrl;
  this.version = options.version || defaults.version;
  this.maxRequest = options.maxRequest || this.maxRequest || 10;

  /** @private */
  this._transport =
    options.proxyUrl ? new Transport.ProxyTransport(options.proxyUrl) : new Transport();

  this.callOptions = options.callOptions;

  /*
   * Fire connection:new event to notify jsforce plugin modules
   */
  var jsforce = require('./core');
  jsforce.emit('connection:new', this);

  /**
   * Streaming API object
   * @member {Streaming} Connection#streaming
   */
  // this.streaming = new Streaming(this);
  /**
   * Bulk API object
   * @member {Bulk} Connection#bulk
   */
  // this.bulk = new Bulk(this);
  /**
   * Tooling API object
   * @member {Tooling} Connection#tooling
   */
  // this.tooling = new Tooling(this);
  /**
   * Analytics API object
   * @member {Analytics} Connection#analytics
   */
  // this.analytics = new Analytics(this);
  /**
   * Chatter API object
   * @member {Chatter} Connection#chatter
   */
  // this.chatter = new Chatter(this);
  /**
   * Metadata API object
   * @member {Metadata} Connection#metadata
   */
  // this.metadata = new Metadata(this);

  /**
   * SOAP API object
   * @member {SoapApi} Connection#soap
   */
  // this.soap = new SoapApi(this);

  /**
   * Apex REST API object
   * @member {Apex} Connection#apex
   */
  // this.apex = new Apex(this);

  /**
   * @member {Process} Connection#process
   */
  this.process = new Process(this);

  /**
   * Cache object for result
   * @member {Cache} Connection#cache
   */
  this.cache = new Cache();

  // Allow to delegate connection refresh to outer function
  var self = this;
  var refreshFn = options.refreshFn;
  if (!refreshFn && this.oauth2.clientId && this.oauth2.clientSecret) {
    refreshFn = oauthRefreshFn;
  }
  if (refreshFn) {
    this._refreshDelegate = new HttpApi.SessionRefreshDelegate(this, refreshFn);
  }

  var cacheOptions = {
    key: function(type) { return type ? "describe." + type : "describe"; }
  };
  this.describe$ = this.cache.makeCacheable(this.describe, this, cacheOptions);
  this.describe = this.cache.makeResponseCacheable(this.describe, this, cacheOptions);
  this.describeSObject$ = this.describe$;
  this.describeSObject = this.describe;

  cacheOptions = { key: 'describeGlobal' };
  this.describeGlobal$ = this.cache.makeCacheable(this.describeGlobal, this, cacheOptions);
  this.describeGlobal = this.cache.makeResponseCacheable(this.describeGlobal, this, cacheOptions);

  this.initialize(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Date"></a>[function <span class="apidocSignatureSpan">jsforce.</span>Date (literal)](#apidoc.element.jsforce.Date)
- description and source-code
```javascript
Date = function (literal) {
  this._literal = literal;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.OAuth2"></a>[function <span class="apidocSignatureSpan">jsforce.</span>OAuth2 (options)](#apidoc.element.jsforce.OAuth2)
- description and source-code
```javascript
OAuth2 = function (options) {
  if (options.authzServiceUrl && options.tokenServiceUrl) {
    this.loginUrl = options.authzServiceUrl.split('/').slice(0, 3).join('/');
    this.authzServiceUrl = options.authzServiceUrl;
    this.tokenServiceUrl = options.tokenServiceUrl;
    this.revokeServiceUrl = options.revokeServiceUrl;
  } else {
    this.loginUrl = options.loginUrl || defaults.loginUrl;
    this.authzServiceUrl = this.loginUrl + "/services/oauth2/authorize";
    this.tokenServiceUrl = this.loginUrl + "/services/oauth2/token";
    this.revokeServiceUrl = this.loginUrl + "/services/oauth2/revoke";
  }
  this.clientId = options.clientId;
  this.clientSecret = options.clientSecret;
  this.redirectUri = options.redirectUri;
  this._transport =
    options.proxyUrl ? new Transport.ProxyTransport(options.proxyUrl) : new Transport();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Promise"></a>[function <span class="apidocSignatureSpan">jsforce.</span>Promise (fn)](#apidoc.element.jsforce.Promise)
- description and source-code
```javascript
function Promise(fn) {
  if (typeof this !== 'object') {
    throw new TypeError('Promises must be constructed via new');
  }
  if (typeof fn !== 'function') {
    throw new TypeError('not a function');
  }
  this._45 = 0;
  this._81 = 0;
  this._65 = null;
  this._54 = null;
  if (fn === noop) return;
  doResolve(fn, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream"></a>[function <span class="apidocSignatureSpan">jsforce.</span>RecordStream ()](#apidoc.element.jsforce.RecordStream)
- description and source-code
```javascript
RecordStream = function () {
  RecordStream.super_.call(this, { objectMode: true });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Parsable"></a>[function <span class="apidocSignatureSpan">jsforce.</span>RecordStream.Parsable ()](#apidoc.element.jsforce.RecordStream.Parsable)
- description and source-code
```javascript
RecordStream.Parsable = function () {
  Parsable.super_.call(this);
  this._dataStream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Serializable"></a>[function <span class="apidocSignatureSpan">jsforce.</span>RecordStream.Serializable ()](#apidoc.element.jsforce.RecordStream.Serializable)
- description and source-code
```javascript
RecordStream.Serializable = function () {
  Serializable.super_.call(this);
  this._dataStream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_"></a>[function <span class="apidocSignatureSpan">jsforce.</span>RecordStream.super_ (options)](#apidoc.element.jsforce.RecordStream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er, data) {
      done(stream, er, data);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate"></a>[function <span class="apidocSignatureSpan">jsforce.</span>SfDate (literal)](#apidoc.element.jsforce.SfDate)
- description and source-code
```javascript
SfDate = function (literal) {
  this._literal = literal;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.cache"></a>[function <span class="apidocSignatureSpan">jsforce.</span>cache ()](#apidoc.element.jsforce.cache)
- description and source-code
```javascript
cache = function () {
  this._entries = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.http_api"></a>[function <span class="apidocSignatureSpan">jsforce.</span>http_api (conn, options)](#apidoc.element.jsforce.http_api)
- description and source-code
```javascript
http_api = function (conn, options) {
  options = options || {};
  this._conn = conn;
  this.on('resume', function(err) { conn.emit('resume', err); });
  this._responseType = options.responseType;
  this._transport = options.transport || conn._transport;
  this._noContentResponse = options.noContentResponse;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.logger"></a>[function <span class="apidocSignatureSpan">jsforce.</span>logger (logLevel)](#apidoc.element.jsforce.logger)
- description and source-code
```javascript
logger = function (logLevel) {
  if (typeof logLevel === 'string') {
    logLevel = LogLevels[logLevel];
  }
  if (!logLevel) {
    logLevel = LogLevels.INFO;
  }
  this._logLevel = logLevel;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query"></a>[function <span class="apidocSignatureSpan">jsforce.</span>query (conn, config, options)](#apidoc.element.jsforce.query)
- description and source-code
```javascript
query = function (conn, config, options) {
  Query.super_.call(this, { objectMode: true });

  this._conn = conn;
  if (_.isString(config)) { // if query config is string, it is given in SOQL.
    this._soql = config;
  } else if (config.locator && config.locator.indexOf("/") >= 0) { // if locator given in url for next records
    this._locator = config.locator.split("/").pop();
  } else {
    this._config = config;
    this.select(config.fields);
    if (config.includes) {
      this.include(config.includes);
    }
  }
  this._options = _.defaults({
    maxFetch: 10000,
    autoFetch: false,
    scanAll: false,
    responseTarget: ResponseTargets.QueryResult
  }, options || {});
  this._executed = false;
  this._finished = false;
  this._chaining = false;

  this._deferred = Promise.defer();

  var self = this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.quick_action"></a>[function <span class="apidocSignatureSpan">jsforce.</span>quick_action (conn, path)](#apidoc.element.jsforce.quick_action)
- description and source-code
```javascript
quick_action = function (conn, path) {
  this._conn = conn;
  this._path = path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.record"></a>[function <span class="apidocSignatureSpan">jsforce.</span>record (conn, type, id)](#apidoc.element.jsforce.record)
- description and source-code
```javascript
record = function (conn, type, id) {
  this._conn = conn;
  this.type = type;
  this.id = id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.require"></a>[function <span class="apidocSignatureSpan">jsforce.</span>require (name)](#apidoc.element.jsforce.require)
- description and source-code
```javascript
require = function (name) {
  if (name === './jsforce' || name === 'jsforce') {
    name = './core';
  }
  var m = required[name];
  if (typeof m === 'undefined') {
    throw new Error("Cannot find module '" + name + "'");
  }
  return m;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.soap"></a>[function <span class="apidocSignatureSpan">jsforce.</span>soap (conn, options)](#apidoc.element.jsforce.soap)
- description and source-code
```javascript
soap = function (conn, options) {
  SOAP.super_.apply(this, arguments);
  this._endpointUrl = options.endpointUrl;
  this._xmlns = options.xmlns || 'urn:partner.soap.sforce.com';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject"></a>[function <span class="apidocSignatureSpan">jsforce.</span>sobject (conn, type)](#apidoc.element.jsforce.sobject)
- description and source-code
```javascript
sobject = function (conn, type) {
  this._conn = conn;
  this.type = type;
  var cacheOptions = { key: "describe." + this.type };
  this.describe$ = conn.cache.makeCacheable(this.describe, this, cacheOptions);
  this.describe = conn.cache.makeResponseCacheable(this.describe, this, cacheOptions);

  cacheOptions = { key: "layouts." + this.type };
  this.layouts$ = conn.cache.makeCacheable(this.layouts, this, cacheOptions);
  this.layouts = conn.cache.makeResponseCacheable(this.layouts, this, cacheOptions);

  cacheOptions = { key: "compactLayouts." + this.type };
  this.compactLayouts$ = conn.cache.makeCacheable(this.compactLayouts, this, cacheOptions);
  this.compactLayouts = conn.cache.makeResponseCacheable(this.compactLayouts, this, cacheOptions);

  cacheOptions = { key: "approvalLayouts." + this.type };
  this.approvalLayouts$ = conn.cache.makeCacheable(this.approvalLayouts, this, cacheOptions);
  this.approvalLayouts = conn.cache.makeResponseCacheable(this.approvalLayouts, this, cacheOptions);
}
```
- example usage
```shell
...
  callback = type;
  type = null;
}
type = type || (this._config && this._config.table);
if (!type) {
  throw new Error("SOQL based query needs SObject type information to bulk delete.");
}
var batch = this._conn.sobject(type).deleteBulk();
var deferred = Promise.defer();
var handleError = function(err) {
  if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
  else { deferred.reject(err); }
};
this.on('error', handleError)
  .pipe(batch)
...
```

#### <a name="apidoc.element.jsforce.transport"></a>[function <span class="apidocSignatureSpan">jsforce.</span>transport ()](#apidoc.element.jsforce.transport)
- description and source-code
```javascript
transport = function () {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.Connection"></a>[module jsforce.Connection](#apidoc.module.jsforce.Connection)

#### <a name="apidoc.element.jsforce.Connection.Connection"></a>[function <span class="apidocSignatureSpan">jsforce.</span>Connection (options)](#apidoc.element.jsforce.Connection.Connection)
- description and source-code
```javascript
Connection = function (options) {
  options = options || {};

  this._logger = new Logger(options.logLevel);

  var oauth2 = options.oauth2 || {
    loginUrl : options.loginUrl,
    clientId : options.clientId,
    clientSecret : options.clientSecret,
    redirectUri : options.redirectUri,
    proxyUrl: options.proxyUrl
  };

<span class="apidocCodeCommentSpan">  /**
   * OAuth2 object
   * @member {OAuth2} Connection#oauth2
   */
</span>  this.oauth2 = oauth2 = oauth2 instanceof OAuth2 ? oauth2 : new OAuth2(oauth2);

  this.loginUrl = options.loginUrl || oauth2.loginUrl || defaults.loginUrl;
  this.version = options.version || defaults.version;
  this.maxRequest = options.maxRequest || this.maxRequest || 10;

  /** @private */
  this._transport =
    options.proxyUrl ? new Transport.ProxyTransport(options.proxyUrl) : new Transport();

  this.callOptions = options.callOptions;

  /*
   * Fire connection:new event to notify jsforce plugin modules
   */
  var jsforce = require('./core');
  jsforce.emit('connection:new', this);

  /**
   * Streaming API object
   * @member {Streaming} Connection#streaming
   */
  // this.streaming = new Streaming(this);
  /**
   * Bulk API object
   * @member {Bulk} Connection#bulk
   */
  // this.bulk = new Bulk(this);
  /**
   * Tooling API object
   * @member {Tooling} Connection#tooling
   */
  // this.tooling = new Tooling(this);
  /**
   * Analytics API object
   * @member {Analytics} Connection#analytics
   */
  // this.analytics = new Analytics(this);
  /**
   * Chatter API object
   * @member {Chatter} Connection#chatter
   */
  // this.chatter = new Chatter(this);
  /**
   * Metadata API object
   * @member {Metadata} Connection#metadata
   */
  // this.metadata = new Metadata(this);

  /**
   * SOAP API object
   * @member {SoapApi} Connection#soap
   */
  // this.soap = new SoapApi(this);

  /**
   * Apex REST API object
   * @member {Apex} Connection#apex
   */
  // this.apex = new Apex(this);

  /**
   * @member {Process} Connection#process
   */
  this.process = new Process(this);

  /**
   * Cache object for result
   * @member {Cache} Connection#cache
   */
  this.cache = new Cache();

  // Allow to delegate connection refresh to outer function
  var self = this;
  var refreshFn = options.refreshFn;
  if (!refreshFn && this.oauth2.clientId && this.oauth2.clientSecret) {
    refreshFn = oauthRefreshFn;
  }
  if (refreshFn) {
    this._refreshDelegate = new HttpApi.SessionRefreshDelegate(this, refreshFn);
  }

  var cacheOptions = {
    key: function(type) { return type ? "describe." + type : "describe"; }
  };
  this.describe$ = this.cache.makeCacheable(this.describe, this, cacheOptions);
  this.describe = this.cache.makeResponseCacheable(this.describe, this, cacheOptions);
  this.describeSObject$ = this.describe$;
  this.describeSObject = this.describe;

  cacheOptions = { key: 'describeGlobal' };
  this.describeGlobal$ = this.cache.makeCacheable(this.describeGlobal, this, cacheOptions);
  this.describeGlobal = this.cache.makeResponseCacheable(this.describeGlobal, this, cacheOptions);

  this.initialize(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.super_"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.</span>super_ ()](#apidoc.element.jsforce.Connection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.Connection.prototype"></a>[module jsforce.Connection.prototype](#apidoc.module.jsforce.Connection.prototype)

#### <a name="apidoc.element.jsforce.Connection.prototype._baseUrl"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>_baseUrl ()](#apidoc.element.jsforce.Connection.prototype._baseUrl)
- description and source-code
```javascript
_baseUrl = function () {
  return [ this.instanceUrl, "services/data", "v" + this.version ].join('/');
}
```
- example usage
```shell
...
var responseTarget = options.responseTarget;
var autoFetch = options.autoFetch;
var maxFetch = options.maxFetch;
var scanAll = options.scanAll;

return Promise.resolve(
  self._locator ?
  self._conn._baseUrl() + "/query/" + self._locator :
  self.toSOQL().then(function(soql) {
    self.totalFetched = 0;
    logger.debug("SOQL = " + soql);
    return self._conn._baseUrl() + "/" + (scanAll ? "queryAll" : "query") + "?q=" + encodeURIComponent(soql);
  })
).then(function(url) {
  return self._conn.request({
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype._normalizeUrl"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>_normalizeUrl (url)](#apidoc.element.jsforce.Connection.prototype._normalizeUrl)
- description and source-code
```javascript
_normalizeUrl = function (url) {
  if (url[0] === '/') {
    if (url.indexOf('/services/') === 0) {
      return this.instanceUrl + url;
    } else {
      return this._baseUrl() + url;
    }
  } else {
    return url;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.authorize"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>authorize (code, callback)](#apidoc.element.jsforce.Connection.prototype.authorize)
- description and source-code
```javascript
authorize = function (code, callback) {
  var self = this;
  var logger = this._logger;

  return this.oauth2.requestToken(code).then(function(res) {
    logger.debug("OAuth2 token response = " + JSON.stringify(res));
    var userInfo = parseIdUrl(res.id);
    self.initialize({
      instanceUrl : res.instance_url,
      accessToken : res.access_token,
      refreshToken : res.refresh_token,
      userInfo: userInfo
    });
    logger.debug("<login> completed. user id = " + userInfo.id + ", org id = " + userInfo.organizationId);
    return userInfo;

  }).thenCall(callback);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.create"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>create (type, records, options, callback)](#apidoc.element.jsforce.Connection.prototype.create)
- description and source-code
```javascript
create = function (type, records, options, callback) {
  if (!_.isString(type)) {
    // reverse order
    callback = options;
    options = records;
    records = type;
    type = null;
  }
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(records);
  records = isArray ? records : [ records ];
  if (records.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(records, function(record) {
      var sobjectType = type || (record.attributes && record.attributes.type) || record.type;
      if (!sobjectType) {
        throw new Error('No SObject Type defined in record');
      }
      record = _.clone(record);
      delete record.Id;
      delete record.type;
      delete record.attributes;

      var url = [ self._baseUrl(), "sobjects", sobjectType ].join('/');
      return self.request({
        method : 'POST',
        url : url,
        body : JSON.stringify(record),
        headers : _.defaults(options.headers || {}, {
          "Content-Type" : "application/json"
        })
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
...
*/
SObject.prototype.insert =
SObject.prototype.create = function(records, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.create(this.type, records, options, callback);
};

/**
* Retrieve specified records
*
* @param {String|Array.<String>} ids - A record ID or array of record IDs
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.del"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>del (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.del)
- description and source-code
```javascript
del = function (type, ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(ids);
  ids = isArray ? ids : [ ids ];
  if (ids.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(ids, function(id) {
      var url = [ self._baseUrl(), "sobjects", type, id ].join('/');
      return self.request({
        method : 'DELETE',
        url : url,
        headers: options.headers || null
      }, {
        noContentResponse: { id : id, success : true, errors : [] }
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.delete"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>delete (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.delete)
- description and source-code
```javascript
delete = function (type, ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(ids);
  ids = isArray ? ids : [ ids ];
  if (ids.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(ids, function(id) {
      var url = [ self._baseUrl(), "sobjects", type, id ].join('/');
      return self.request({
        method : 'DELETE',
        url : url,
        headers: options.headers || null
      }, {
        noContentResponse: { id : id, success : true, errors : [] }
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.deleted"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>deleted (type, start, end, callback)](#apidoc.element.jsforce.Connection.prototype.deleted)
- description and source-code
```javascript
deleted = function (type, start, end, callback) {
  var url = [ this._baseUrl(), "sobjects", type, "deleted" ].join('/');

  if (typeof start === 'string') {
    start = new Date(start);
  }

  if (start instanceof Date) {
    start = formatDate(start);
  }

  if (start) {
    url += "?start=" + encodeURIComponent(start);
  }

  if (typeof end === 'string') {
    end = new Date(end);
  }

  if (end instanceof Date) {
    end = formatDate(end);
  }

  if (end) {
    url += "&end=" + encodeURIComponent(end);
  }

  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
...
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
* @param {Callback.<DeletedRecordsInfo>} [callback] - Callback function
* @returns {Promise.<DeletedRecordsInfo>}
*/
SObject.prototype.deleted = function (start, end, callback) {
 return this._conn.deleted(this.type, start, end, callback);
};

/**
* @typedef {Object} LayoutInfo
* @prop {Array.<Object>} layouts - Array of layouts
* @prop {Array.<Object>} recordTypeMappings - Array of record type mappings
*/
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.describe"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>describe (type, callback)](#apidoc.element.jsforce.Connection.prototype.describe)
- description and source-code
```javascript
describe = function (type, callback) {
  var url = [ this._baseUrl(), "sobjects", type, "describe" ].join('/');
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
...
/**
* Describe SObject metadata
*
* @param {Callback.<DescribeSObjectResult>} [callback] - Callback function
* @returns {Promise.<DescribeSObjectResult>}
*/
SObject.prototype.describe = function(callback) {
 return this._conn.describe(this.type, callback);
};

/**
* Get record representation instance by given id
*
* @param {String} id - A record ID
* @returns {RecordReference}
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.describeGlobal"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>describeGlobal (callback)](#apidoc.element.jsforce.Connection.prototype.describeGlobal)
- description and source-code
```javascript
describeGlobal = function (callback) {
  var url = this._baseUrl() + "/sobjects";
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.describeSObject"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>describeSObject (type, callback)](#apidoc.element.jsforce.Connection.prototype.describeSObject)
- description and source-code
```javascript
describeSObject = function (type, callback) {
  var url = [ this._baseUrl(), "sobjects", type, "describe" ].join('/');
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.destroy"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>destroy (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.destroy)
- description and source-code
```javascript
destroy = function (type, ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(ids);
  ids = isArray ? ids : [ ids ];
  if (ids.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(ids, function(id) {
      var url = [ self._baseUrl(), "sobjects", type, id ].join('/');
      return self.request({
        method : 'DELETE',
        url : url,
        headers: options.headers || null
      }, {
        noContentResponse: { id : id, success : true, errors : [] }
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
...
* @returns {Promise.<RecordResult>}
*/
RecordReference.prototype.destroy = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.destroy(this.type, this.id, options, callback);
};

/**
* Get blob field as stream
*
* @param {String} fieldName - Blob field name
* @returns {stream.Stream}
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.identity"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>identity (options, callback)](#apidoc.element.jsforce.Connection.prototype.identity)
- description and source-code
```javascript
identity = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var idUrl = this.userInfo && this.userInfo.url;
  return Promise.resolve(
    idUrl ?
    { identity: idUrl } :
    this.request({ method: 'GET', url: this._baseUrl(), headers: options.headers })
  ).then(function(res) {
    var url = res.identity;
    url += '?format=json&oauth_token=' + encodeURIComponent(self.accessToken);
    var transport = Transport.JsonpTransport.supported ?
      new Transport.JsonpTransport('callback') :
      undefined;
    return self.request({ method: 'GET', url: url }, { transport: transport });
  }).then(function(res) {
    self.userInfo = {
      id: res.user_id,
      organizationId: res.organization_id,
      url: res.id
    };
    return res;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.initialize"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>initialize (options)](#apidoc.element.jsforce.Connection.prototype.initialize)
- description and source-code
```javascript
initialize = function (options) {
  if (!options.instanceUrl && options.serverUrl) {
    options.instanceUrl = options.serverUrl.split('/').slice(0, 3).join('/');
  }
  this.instanceUrl = options.instanceUrl || options.serverUrl || this.instanceUrl || defaults.instanceUrl;

  this.accessToken = options.sessionId || options.accessToken || this.accessToken;
  this.refreshToken = options.refreshToken || this.refreshToken;
  if (this.refreshToken && !this._refreshDelegate) {
    throw new Error("Refresh token is specified without oauth2 client information or refresh function");
  }

  this.signedRequest = options.signedRequest && parseSignedRequest(options.signedRequest);
  if (this.signedRequest) {
    this.accessToken = this.signedRequest.client.oauthToken;
    if (Transport.CanvasTransport.supported) {
      this._transport = new Transport.CanvasTransport(this.signedRequest);
    }
  }

  if (options.userInfo) {
    this.userInfo = options.userInfo;
  }

  this.limitInfo = {};

  this.sobjects = {};
  this.cache.clear();
  this.cache.get('describeGlobal').on('value', _.bind(function(res) {
    if (res.result) {
      var types = _.map(res.result.sobjects, function(so) { return so.name; });
      types.forEach(this.sobject, this);
    }
  }, this));

  if (this.tooling) {
    this.tooling.initialize();
  }

  this._sessionType = options.sessionId ? "soap" : "oauth2";

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.insert"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>insert (type, records, options, callback)](#apidoc.element.jsforce.Connection.prototype.insert)
- description and source-code
```javascript
insert = function (type, records, options, callback) {
  if (!_.isString(type)) {
    // reverse order
    callback = options;
    options = records;
    records = type;
    type = null;
  }
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(records);
  records = isArray ? records : [ records ];
  if (records.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(records, function(record) {
      var sobjectType = type || (record.attributes && record.attributes.type) || record.type;
      if (!sobjectType) {
        throw new Error('No SObject Type defined in record');
      }
      record = _.clone(record);
      delete record.Id;
      delete record.type;
      delete record.attributes;

      var url = [ self._baseUrl(), "sobjects", sobjectType ].join('/');
      return self.request({
        method : 'POST',
        url : url,
        body : JSON.stringify(record),
        headers : _.defaults(options.headers || {}, {
          "Content-Type" : "application/json"
        })
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.limits"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>limits (callback)](#apidoc.element.jsforce.Connection.prototype.limits)
- description and source-code
```javascript
limits = function (callback) {
  var url = [ this._baseUrl(), "limits" ].join('/');
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.login"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>login (username, password, callback)](#apidoc.element.jsforce.Connection.prototype.login)
- description and source-code
```javascript
login = function (username, password, callback) {
  // register refreshDelegate for session expiration
  this._refreshDelegate = new HttpApi.SessionRefreshDelegate(this, createUsernamePasswordRefreshFn(username, password));
  if (this.oauth2 && this.oauth2.clientId && this.oauth2.clientSecret) {
    return this.loginByOAuth2(username, password, callback);
  } else {
    return this.loginBySoap(username, password, callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.loginByOAuth2"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>loginByOAuth2 (username, password, callback)](#apidoc.element.jsforce.Connection.prototype.loginByOAuth2)
- description and source-code
```javascript
loginByOAuth2 = function (username, password, callback) {
  var self = this;
  var logger = this._logger;
  return this.oauth2.authenticate(username, password).then(function(res) {
    logger.debug("OAuth2 token response = " + JSON.stringify(res));
    var userInfo = parseIdUrl(res.id);
    self.initialize({
      instanceUrl : res.instance_url,
      accessToken : res.access_token,
      userInfo: userInfo
    });
    logger.debug("<login> completed. user id = " + userInfo.id + ", org id = " + userInfo.organizationId);
    return userInfo;

  }).thenCall(callback);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.loginBySoap"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>loginBySoap (username, password, callback)](#apidoc.element.jsforce.Connection.prototype.loginBySoap)
- description and source-code
```javascript
loginBySoap = function (username, password, callback) {
  var self = this;
  var logger = this._logger;
  var body = [
    '<se:Envelope xmlns:se="http://schemas.xmlsoap.org/soap/envelope/">',
      '<se:Header/>',
      '<se:Body>',
        '<login xmlns="urn:partner.soap.sforce.com">',
          '<username>' + esc(username) + '</username>',
          '<password>' + esc(password) + '</password>',
        '</login>',
      '</se:Body>',
    '</se:Envelope>'
  ].join('');

  var soapLoginEndpoint = [ this.loginUrl, "services/Soap/u", this.version ].join('/');

  return this._transport.httpRequest({
    method : 'POST',
    url : soapLoginEndpoint,
    body : body,
    headers : {
      "Content-Type" : "text/xml",
      "SOAPAction" : '""'
    }
  }).then(function(response) {
    var m;
    if (response.statusCode >= 400) {
      m = response.body.match(/<faultstring>([^<]+)<\/faultstring>/);
      var faultstring = m && m[1];
      throw new Error(faultstring || response.body);
    }
    logger.debug("SOAP response = " + response.body);
    m = response.body.match(/<serverUrl>([^<]+)<\/serverUrl>/);
    var serverUrl = m && m[1];
    m = response.body.match(/<sessionId>([^<]+)<\/sessionId>/);
    var sessionId = m && m[1];
    m = response.body.match(/<userId>([^<]+)<\/userId>/);
    var userId = m && m[1];
    m = response.body.match(/<organizationId>([^<]+)<\/organizationId>/);
    var orgId = m && m[1];
    var idUrl = soapLoginEndpoint.split('/').slice(0, 3).join('/');
    idUrl += "/id/" + orgId + "/" + userId;
    var userInfo = {
      id: userId,
      organizationId: orgId,
      url: idUrl
    };
    self.initialize({
      serverUrl: serverUrl.split('/').slice(0, 3).join('/'),
      sessionId: sessionId,
      userInfo: userInfo
    });
    logger.debug("<login> completed. user id = " + userId + ", org id = " + orgId);
    return userInfo;

  }).thenCall(callback);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.logout"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>logout (callback)](#apidoc.element.jsforce.Connection.prototype.logout)
- description and source-code
```javascript
logout = function (callback) {
  if (this._sessionType === "oauth2") {
    return this.logoutByOAuth2(callback);
  } else {
    return this.logoutBySoap(callback);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.logoutByOAuth2"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>logoutByOAuth2 (callback)](#apidoc.element.jsforce.Connection.prototype.logoutByOAuth2)
- description and source-code
```javascript
logoutByOAuth2 = function (callback) {
  var self = this;
  var logger = this._logger;

  return this.oauth2.revokeToken(this.accessToken).then(function() {
    // Destroy the session bound to this connection
    self.accessToken = null;
    self.userInfo = null;
    self.refreshToken = null;
    self.instanceUrl = null;
    self.cache.clear();

    // nothing useful returned by logout API, just return
    return undefined;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.logoutBySoap"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>logoutBySoap (callback)](#apidoc.element.jsforce.Connection.prototype.logoutBySoap)
- description and source-code
```javascript
logoutBySoap = function (callback) {
  var self = this;
  var logger = this._logger;

  var body = [
    '<se:Envelope xmlns:se="http://schemas.xmlsoap.org/soap/envelope/">',
      '<se:Header>',
        '<SessionHeader xmlns="urn:partner.soap.sforce.com">',
          '<sessionId>' + esc(this.accessToken) + '</sessionId>',
        '</SessionHeader>',
      '</se:Header>',
      '<se:Body>',
        '<logout xmlns="urn:partner.soap.sforce.com"/>',
      '</se:Body>',
    '</se:Envelope>'
  ].join('');

  return this._transport.httpRequest({
    method : 'POST',
    url : [ this.instanceUrl, "services/Soap/u", this.version ].join('/'),
    body : body,
    headers : {
      "Content-Type" : "text/xml",
      "SOAPAction" : '""'
    }
  }).then(function(response) {
    logger.debug("SOAP statusCode = " + response.statusCode + ", response = " + response.body);
    if (response.statusCode >= 400) {
      var m = response.body.match(/<faultstring>([^<]+)<\/faultstring>/);
      var faultstring = m && m[1];
      throw new Error(faultstring || response.body);
    }

    // Destroy the session bound to this connection
    self.accessToken = null;
    self.userInfo = null;
    self.refreshToken = null;
    self.instanceUrl = null;
    self.cache.clear();

    // nothing useful returned by logout API, just return
    return undefined;

  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.query"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>query (soql, options, callback)](#apidoc.element.jsforce.Connection.prototype.query)
- description and source-code
```javascript
query = function (soql, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = undefined;
  }
  var query = new Query(this, soql, options);
  if (callback) {
    query.run(callback);
  }
  return query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.queryAll"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>queryAll (soql, options, callback)](#apidoc.element.jsforce.Connection.prototype.queryAll)
- description and source-code
```javascript
queryAll = function (soql, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = undefined;
  }
  var query = new Query(this, soql, options);
  query.scanAll(true);
  if (callback) {
    query.run(callback);
  }
  return query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.queryMore"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>queryMore (locator, options, callback)](#apidoc.element.jsforce.Connection.prototype.queryMore)
- description and source-code
```javascript
queryMore = function (locator, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = undefined;
  }
  var query = new Query(this, { locator: locator }, options);
  if (callback) {
    query.run(callback);
  }
  return query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.quickAction"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>quickAction (actionName)](#apidoc.element.jsforce.Connection.prototype.quickAction)
- description and source-code
```javascript
quickAction = function (actionName) {
  return new QuickAction(this, "/quickActions/" + actionName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.quickActions"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>quickActions (callback)](#apidoc.element.jsforce.Connection.prototype.quickActions)
- description and source-code
```javascript
quickActions = function (callback) {
  return this.request("/quickActions").thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.recent"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>recent (type, limit, callback)](#apidoc.element.jsforce.Connection.prototype.recent)
- description and source-code
```javascript
recent = function (type, limit, callback) {
  if (!_.isString(type)) {
    callback = limit;
    limit = type;
    type = undefined;
  }
  if (!_.isNumber(limit)) {
    callback = limit;
    limit = undefined;
  }
  var url;
  if (type) {
    url = [ this._baseUrl(), "sobjects", type ].join('/');
    return this.request(url).then(function(res) {
      return limit ? res.recentItems.slice(0, limit) : res.recentItems;
    }).thenCall(callback);
  } else {
    url = this._baseUrl() + "/recent";
    if (limit) {
      url += "?limit=" + limit;
    }
    return this.request(url).thenCall(callback);
  }

}
```
- example usage
```shell
...
/**
* Retrieve recently accessed records
*
* @param {Callback.<Array.<RecordResult>>} [callback] - Callback function
* @returns {Promise.<Array.<RecordResult>>}
*/
SObject.prototype.recent = function (callback) {
 return this._conn.recent(this.type, callback);
};

/**
* Retrieve the updated records
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.request"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>request (request, options, callback)](#apidoc.element.jsforce.Connection.prototype.request)
- description and source-code
```javascript
request = function (request, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = null;
  }
  options = options || {};
  var self = this;

  // if request is simple string, regard it as url in GET method
  if (_.isString(request)) {
    request = { method: 'GET', url: request };
  }
  // if url is given in relative path, prepend base url or instance url before.
  request.url = this._normalizeUrl(request.url);

  var httpApi = new HttpApi(this, options);

  // log api usage and its quota
  httpApi.on('response', function(response) {
    if (response.headers && response.headers["sforce-limit-info"]) {
      var apiUsage = response.headers["sforce-limit-info"].match(/api\-usage=(\d+)\/(\d+)/);
      if (apiUsage) {
        self.limitInfo = {
          apiUsage: {
            used: parseInt(apiUsage[1], 10),
            limit: parseInt(apiUsage[2], 10)
          }
        };
      }
    }
  });
  return httpApi.request(request).thenCall(callback);
}
```
- example usage
```shell
...
  if(lastInstanceUrl !== conn.instanceUrl){
    // if the instance url has changed
    // then replace the current request urls instance url fragment
    // with the updated instance url
    request.url = request.url.replace(lastInstanceUrl,conn.instanceUrl);
  }

  self.request(request).then(function(response) {
    deferred.resolve(response);
  }, function(err) {
    deferred.reject(err);
  });
};

if (refreshDelegate && refreshDelegate._refreshing) {
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.requestDelete"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestDelete (url, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestDelete)
- description and source-code
```javascript
requestDelete = function (url, options, callback) {
  var request = {
    method: "DELETE",
    url: url
  };
  return this.request(request, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.requestGet"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestGet (url, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestGet)
- description and source-code
```javascript
requestGet = function (url, options, callback) {
  var request = {
    method: "GET",
    url: url
  };
  return this.request(request, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.requestPatch"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestPatch (url, body, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestPatch)
- description and source-code
```javascript
requestPatch = function (url, body, options, callback) {
  var request = {
    method: "PATCH",
    url: url,
    body: JSON.stringify(body),
    headers: { "content-type": "application/json" }
  };
  return this.request(request, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.requestPost"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestPost (url, body, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestPost)
- description and source-code
```javascript
requestPost = function (url, body, options, callback) {
  var request = {
    method: "POST",
    url: url,
    body: JSON.stringify(body),
    headers: { "content-type": "application/json" }
  };
  return this.request(request, options, callback);
}
```
- example usage
```shell
...
 * @returns {Promise.<QuickAction~QuickActionResult>}
 */
QuickAction.prototype.execute = function(contextId, record, callback) {
  var body = {
    contextId: contextId,
    record: record
  };
  return this._conn.requestPost(this._path, body).thenCall(callback);
};
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.requestPut"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>requestPut (url, body, options, callback)](#apidoc.element.jsforce.Connection.prototype.requestPut)
- description and source-code
```javascript
requestPut = function (url, body, options, callback) {
  var request = {
    method: "PUT",
    url: url,
    body: JSON.stringify(body),
    headers: { "content-type": "application/json" }
  };
  return this.request(request, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.retrieve"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>retrieve (type, ids, options, callback)](#apidoc.element.jsforce.Connection.prototype.retrieve)
- description and source-code
```javascript
retrieve = function (type, ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(ids);
  ids = isArray ? ids : [ ids ];
  if (ids.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(ids, function(id) {
      if (!id) { return Promise.reject(new Error('Invalid record ID. Specify valid record ID value')).thenCall(callback); }
      var url = [ self._baseUrl(), "sobjects", type, id ].join('/');
      return self.request({ method: 'GET', url: url, headers: options.headers });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
...
* @returns {Promise.<Record>}
*/
RecordReference.prototype.retrieve = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.retrieve(this.type, this.id, options, callback);
};

/**
* Update record field information
*
* @param {Record} record - A Record which includes fields to update
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.search"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>search (sosl, callback)](#apidoc.element.jsforce.Connection.prototype.search)
- description and source-code
```javascript
search = function (sosl, callback) {
  var url = this._baseUrl() + "/search?q=" + encodeURIComponent(sosl);
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.sobject"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>sobject (type)](#apidoc.element.jsforce.Connection.prototype.sobject)
- description and source-code
```javascript
sobject = function (type) {
  this.sobjects = this.sobjects || {};
  var sobject = this.sobjects[type] =
    this.sobjects[type] || new SObject(this, type);
  return sobject;
}
```
- example usage
```shell
...
  callback = type;
  type = null;
}
type = type || (this._config && this._config.table);
if (!type) {
  throw new Error("SOQL based query needs SObject type information to bulk delete.");
}
var batch = this._conn.sobject(type).deleteBulk();
var deferred = Promise.defer();
var handleError = function(err) {
  if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
  else { deferred.reject(err); }
};
this.on('error', handleError)
  .pipe(batch)
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.tabs"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>tabs (callback)](#apidoc.element.jsforce.Connection.prototype.tabs)
- description and source-code
```javascript
tabs = function (callback) {
  var url = [ this._baseUrl(), "tabs" ].join('/');
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.theme"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>theme (callback)](#apidoc.element.jsforce.Connection.prototype.theme)
- description and source-code
```javascript
theme = function (callback) {
  var url = [ this._baseUrl(), "theme" ].join('/');
  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Connection.prototype.update"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>update (type, records, options, callback)](#apidoc.element.jsforce.Connection.prototype.update)
- description and source-code
```javascript
update = function (type, records, options, callback) {
  if (!_.isString(type)) {
    // reverse order
    callback = options;
    options = records;
    records = type;
    type = null;
  }
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(records);
  records = isArray ? records : [ records ];
  if (records.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(records, function(record) {
      var id = record.Id;
      if (!id) {
        throw new Error('Record id is not found in record.');
      }
      var sobjectType = type || (record.attributes && record.attributes.type) || record.type;
      if (!sobjectType) {
        throw new Error('No SObject Type defined in record');
      }
      record = _.clone(record);
      delete record.Id;
      delete record.type;
      delete record.attributes;

      var url = [ self._baseUrl(), "sobjects", sobjectType, id ].join('/');
      return self.request({
        method : 'PATCH',
        url : url,
        body : JSON.stringify(record),
        headers : _.defaults(options.headers || {}, {
          "Content-Type" : "application/json"
        })
      }, {
        noContentResponse: { id : id, success : true, errors : [] }
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
...
RecordReference.prototype.update = function(record, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 record = _.clone(record);
 record.Id = this.id;
 return this._conn.update(this.type, record, options, callback);
};

/**
* Synonym of Record#destroy()
*
* @method RecordReference#delete
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.updated"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>updated (type, start, end, callback)](#apidoc.element.jsforce.Connection.prototype.updated)
- description and source-code
```javascript
updated = function (type, start, end, callback) {
  var url = [ this._baseUrl(), "sobjects", type, "updated" ].join('/');

  if (typeof start === 'string') {
    start = new Date(start);
  }

  if (start instanceof Date) {
    start = formatDate(start);
  }

  if (start) {
    url += "?start=" + encodeURIComponent(start);
  }

  if (typeof end === 'string') {
    end = new Date(end);
  }

  if (end instanceof Date) {
    end = formatDate(end);
  }

  if (end) {
    url += "&end=" + encodeURIComponent(end);
  }

  return this.request(url).thenCall(callback);
}
```
- example usage
```shell
...
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
* @param {Callback.<UpdatedRecordsInfo>} [callback] - Callback function
* @returns {Promise.<UpdatedRecordsInfo>}
*/
SObject.prototype.updated = function (start, end, callback) {
 return this._conn.updated(this.type, start, end, callback);
};

/**
* Retrieve the deleted records
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
...
```

#### <a name="apidoc.element.jsforce.Connection.prototype.upsert"></a>[function <span class="apidocSignatureSpan">jsforce.Connection.prototype.</span>upsert (type, records, extIdField, options, callback)](#apidoc.element.jsforce.Connection.prototype.upsert)
- description and source-code
```javascript
upsert = function (type, records, extIdField, options, callback) {
  // You can omit "type" argument, when the record includes type information.
  if (!_.isString(type)) {
    // reverse order
    callback = options;
    options = extIdField;
    extIdField = records;
    records = type;
    type = null;
  }
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  options = options || {};
  var self = this;
  var isArray = _.isArray(records);
  records = isArray ? records : [ records ];
  if (records.length > self.maxRequest) {
    return Promise.reject(new Error("Exceeded max limit of concurrent call")).thenCall(callback);
  }
  return Promise.all(
    _.map(records, function(record) {
      var sobjectType = type || (record.attributes && record.attributes.type) || record.type;
      var extId = record[extIdField];
      if (!extId) {
        return Promise.reject(new Error('External ID is not defined in the record'));
      }
      record = _.clone(record);
      delete record[extIdField];
      delete record.type;
      delete record.attributes;

      var url = [ self._baseUrl(), "sobjects", sobjectType, extIdField, extId ].join('/');
      return self.request({
        method : 'PATCH',
        url : url,
        body : JSON.stringify(record),
        headers : _.defaults(options.headers || {}, {
          "Content-Type" : "application/json"
        })
      }, {
        noContentResponse: { success : true, errors : [] }
      });
    })
  ).then(function(results) {
    return !isArray && _.isArray(results) ? results[0] : results;
  }).thenCall(callback);
}
```
- example usage
```shell
...
* @returns {Promise.<RecordResult|Array.<RecordResult>>}
*/
SObject.prototype.upsert = function(records, extIdField, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.upsert(this.type, records, extIdField, options, callback);
};

/**
* Synonym of SObject#destroy()
*
* @method SObject#delete
* @param {String|Array.<String>} ids - A ID or array of IDs to delete
...
```



# <a name="apidoc.module.jsforce.OAuth2"></a>[module jsforce.OAuth2](#apidoc.module.jsforce.OAuth2)

#### <a name="apidoc.element.jsforce.OAuth2.OAuth2"></a>[function <span class="apidocSignatureSpan">jsforce.</span>OAuth2 (options)](#apidoc.element.jsforce.OAuth2.OAuth2)
- description and source-code
```javascript
OAuth2 = function (options) {
  if (options.authzServiceUrl && options.tokenServiceUrl) {
    this.loginUrl = options.authzServiceUrl.split('/').slice(0, 3).join('/');
    this.authzServiceUrl = options.authzServiceUrl;
    this.tokenServiceUrl = options.tokenServiceUrl;
    this.revokeServiceUrl = options.revokeServiceUrl;
  } else {
    this.loginUrl = options.loginUrl || defaults.loginUrl;
    this.authzServiceUrl = this.loginUrl + "/services/oauth2/authorize";
    this.tokenServiceUrl = this.loginUrl + "/services/oauth2/token";
    this.revokeServiceUrl = this.loginUrl + "/services/oauth2/revoke";
  }
  this.clientId = options.clientId;
  this.clientSecret = options.clientSecret;
  this.redirectUri = options.redirectUri;
  this._transport =
    options.proxyUrl ? new Transport.ProxyTransport(options.proxyUrl) : new Transport();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.OAuth2.prototype"></a>[module jsforce.OAuth2.prototype](#apidoc.module.jsforce.OAuth2.prototype)

#### <a name="apidoc.element.jsforce.OAuth2.prototype._postParams"></a>[function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>_postParams (params, callback)](#apidoc.element.jsforce.OAuth2.prototype._postParams)
- description and source-code
```javascript
_postParams = function (params, callback) {
  return this._transport.httpRequest({
    method : 'POST',
    url : this.tokenServiceUrl,
    body : querystring.stringify(params),
    headers : {
      "content-type" : "application/x-www-form-urlencoded"
    }
  }).then(function(response) {
    var res;
    try {
      res = JSON.parse(response.body);
    } catch(e) {}
    if (response.statusCode >= 400) {
      res = res || { error: "ERROR_HTTP_"+response.statusCode, error_description: response.body };
      var err = new Error(res.error_description);
      err.name = res.error;
      throw err;
    }
    return res;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.OAuth2.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>authenticate (username, password, callback)](#apidoc.element.jsforce.OAuth2.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (username, password, callback) {
  return this._postParams({
    grant_type : "password",
    username : username,
    password : password,
    client_id : this.clientId,
    client_secret : this.clientSecret,
    redirect_uri : this.redirectUri
  }, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.OAuth2.prototype.getAuthorizationUrl"></a>[function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>getAuthorizationUrl (params)](#apidoc.element.jsforce.OAuth2.prototype.getAuthorizationUrl)
- description and source-code
```javascript
getAuthorizationUrl = function (params) {
  params = _.extend({
    response_type : "code",
    client_id : this.clientId,
    redirect_uri : this.redirectUri
  }, params || {});
  return this.authzServiceUrl +
    (this.authzServiceUrl.indexOf('?') >= 0 ? "&" : "?") +
    querystring.stringify(params);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.OAuth2.prototype.refreshToken"></a>[function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>refreshToken (refreshToken, callback)](#apidoc.element.jsforce.OAuth2.prototype.refreshToken)
- description and source-code
```javascript
refreshToken = function (refreshToken, callback) {
  return this._postParams({
    grant_type : "refresh_token",
    refresh_token : refreshToken,
    client_id : this.clientId,
    client_secret : this.clientSecret
  }, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.OAuth2.prototype.requestToken"></a>[function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>requestToken (code, callback)](#apidoc.element.jsforce.OAuth2.prototype.requestToken)
- description and source-code
```javascript
requestToken = function (code, callback) {
  return this._postParams({
    grant_type : "authorization_code",
    code : code,
    client_id : this.clientId,
    client_secret : this.clientSecret,
    redirect_uri : this.redirectUri
  }, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.OAuth2.prototype.revokeToken"></a>[function <span class="apidocSignatureSpan">jsforce.OAuth2.prototype.</span>revokeToken (accessToken, callback)](#apidoc.element.jsforce.OAuth2.prototype.revokeToken)
- description and source-code
```javascript
revokeToken = function (accessToken, callback) {
  var req;
  if (Transport.JsonpTransport.supported) {
    var jsonpTransport = new Transport.JsonpTransport('callback');
    req = jsonpTransport.httpRequest({
      method: 'GET',
      url : this.revokeServiceUrl + '?' + querystring.stringify({ token: accessToken })
    });
  } else {
    req = this._transport.httpRequest({
      method : 'POST',
      url : this.revokeServiceUrl,
      body: querystring.stringify({ token: accessToken }),
      headers: {
        "Content-Type": "application/x-www-form-urlencoded"
      }
    });
  }
  return req.then(function(response) {
    if (response.statusCode >= 400) {
      var res = querystring.parse(response.body);
      if (!res || !res.error) {
        res = { error: "ERROR_HTTP_"+response.statusCode, error_description: response.body };
      }
      var err = new Error(res.error_description);
      err.name = res.error;
      throw err;
    }
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.Promise"></a>[module jsforce.Promise](#apidoc.module.jsforce.Promise)

#### <a name="apidoc.element.jsforce.Promise.Promise"></a>[function <span class="apidocSignatureSpan">jsforce.</span>Promise (fn)](#apidoc.element.jsforce.Promise.Promise)
- description and source-code
```javascript
function Promise(fn) {
  if (typeof this !== 'object') {
    throw new TypeError('Promises must be constructed via new');
  }
  if (typeof fn !== 'function') {
    throw new TypeError('not a function');
  }
  this._45 = 0;
  this._81 = 0;
  this._65 = null;
  this._54 = null;
  if (fn === noop) return;
  doResolve(fn, this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Promise._61"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.</span>_61 ()](#apidoc.element.jsforce.Promise._61)
- description and source-code
```javascript
function noop() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Promise.all"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.</span>all (arr)](#apidoc.element.jsforce.Promise.all)
- description and source-code
```javascript
all = function (arr) {
  var args = Array.prototype.slice.call(arr);

  return new Promise(function (resolve, reject) {
    if (args.length === 0) return resolve([]);
    var remaining = args.length;
    function res(i, val) {
      if (val && (typeof val === 'object' || typeof val === 'function')) {
        if (val instanceof Promise && val.then === Promise.prototype.then) {
          while (val._81 === 3) {
            val = val._65;
          }
          if (val._81 === 1) return res(i, val._65);
          if (val._81 === 2) reject(val._65);
          val.then(function (val) {
            res(i, val);
          }, reject);
          return;
        } else {
          var then = val.then;
          if (typeof then === 'function') {
            var p = new Promise(then.bind(val));
            p.then(function (val) {
              res(i, val);
            }, reject);
            return;
          }
        }
      }
      args[i] = val;
      if (--remaining === 0) {
        resolve(args);
      }
    }
    for (var i = 0; i < args.length; i++) {
      res(i, args[i]);
    }
  });
}
```
- example usage
```shell
...
var logger = self._conn._logger;
var conn = this._conn;
var table = this._config.table;
var fields = this._config.fields || [];

logger.debug('_expandFields: table = ' + table + ', fields = ' + fields.join(', '));

return Promise.all([
  Promise.resolve(self._parent ? findRelationTable(table) : table)
    .then(function(table) {
      return Promise.all(
        _.map(fields, function(field) { return expandAsteriskField(table, field); })
      ).then(function(expandedFields) {
        self._config.fields = _.flatten(expandedFields);
      });
...
```

#### <a name="apidoc.element.jsforce.Promise.defer"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.</span>defer ()](#apidoc.element.jsforce.Promise.defer)
- description and source-code
```javascript
defer = function () {
  return new Deferred();
}
```
- example usage
```shell
...
var self = this;
var conn = this._conn;
var logger = conn._logger;
var refreshDelegate = this.getRefreshDelegate();
// remember previous instance url in case it changes after a refresh
var lastInstanceUrl = conn.instanceUrl;

var deferred = Promise.defer();

var onResume = function(err) {
  if (err) {
    deferred.reject(err);
    return;
  }
  // check to see if the token refresh has changed the instance url
...
```

#### <a name="apidoc.element.jsforce.Promise.race"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.</span>race (values)](#apidoc.element.jsforce.Promise.race)
- description and source-code
```javascript
race = function (values) {
  return new Promise(function (resolve, reject) {
    values.forEach(function(value){
      Promise.resolve(value).then(resolve, reject);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Promise.reject"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.</span>reject (value)](#apidoc.element.jsforce.Promise.reject)
- description and source-code
```javascript
reject = function (value) {
  return new Promise(function (resolve, reject) {
    reject(value);
  });
}
```
- example usage
```shell
...
// remember previous instance url in case it changes after a refresh
var lastInstanceUrl = conn.instanceUrl;

var deferred = Promise.defer();

var onResume = function(err) {
  if (err) {
    deferred.reject(err);
    return;
  }
  // check to see if the token refresh has changed the instance url
  if(lastInstanceUrl !== conn.instanceUrl){
    // if the instance url has changed
    // then replace the current request urls instance url fragment
    // with the updated instance url
...
```

#### <a name="apidoc.element.jsforce.Promise.resolve"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.</span>resolve (value)](#apidoc.element.jsforce.Promise.resolve)
- description and source-code
```javascript
resolve = function (value) {
  if (value instanceof Promise) return value;

  if (value === null) return NULL;
  if (value === undefined) return UNDEFINED;
  if (value === true) return TRUE;
  if (value === false) return FALSE;
  if (value === 0) return ZERO;
  if (value === '') return EMPTYSTRING;

  if (typeof value === 'object' || typeof value === 'function') {
    try {
      var then = value.then;
      if (typeof then === 'function') {
        return new Promise(then.bind(value));
      }
    } catch (ex) {
      return new Promise(function (resolve, reject) {
        reject(ex);
      });
    }
  }
  return valuePromise(value);
}
```
- example usage
```shell
...
    // if the instance url has changed
    // then replace the current request urls instance url fragment
    // with the updated instance url
    request.url = request.url.replace(lastInstanceUrl,conn.instanceUrl);
  }

  self.request(request).then(function(response) {
    deferred.resolve(response);
  }, function(err) {
    deferred.reject(err);
  });
};

if (refreshDelegate && refreshDelegate._refreshing) {
  refreshDelegate.once('resume', onResume);
...
```



# <a name="apidoc.module.jsforce.Promise.prototype"></a>[module jsforce.Promise.prototype](#apidoc.module.jsforce.Promise.prototype)

#### <a name="apidoc.element.jsforce.Promise.prototype.catch"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>catch (onRejected)](#apidoc.element.jsforce.Promise.prototype.catch)
- description and source-code
```javascript
catch = function (onRejected) {
  return this.then(null, onRejected);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.Promise.prototype.fail"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>fail (onRejected)](#apidoc.element.jsforce.Promise.prototype.fail)
- description and source-code
```javascript
fail = function (onRejected) {
  return this.then(null, onRejected);
}
```
- example usage
```shell
...
  // flag to prevent re-execution
  this._executed = true;

  // start actual query
  logger.debug('>>> Query start >>>');
  this._execute(options).then(function() {
    logger.debug('*** Query finished ***');
  }).fail(function(err) {
    logger.debug('--- Query error ---');
    self.emit('error', err);
  });

  // return Query instance for chaining
  return this;
};
...
```

#### <a name="apidoc.element.jsforce.Promise.prototype.then"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>then (onFulfilled, onRejected)](#apidoc.element.jsforce.Promise.prototype.then)
- description and source-code
```javascript
then = function (onFulfilled, onRejected) {
  if (this.constructor !== Promise) {
    return safeThen(this, onFulfilled, onRejected);
  }
  var res = new Promise(noop);
  handle(this, new Handler(onFulfilled, onRejected, res));
  return res;
}
```
- example usage
```shell
...
try {
  ret = fn.apply(scope || this, args);
} catch(e) {
  error = e;
}
if (ret && _.isFunction(ret.then)) { // if the returned value is promise
  if (!callback) {
    return ret.then(function(result) {
      entry.set({ error: undefined, result: result });
      return result;
    }, function(err) {
      entry.set({ error: err, result: undefined });
      throw err;
    });
  } else {
...
```

#### <a name="apidoc.element.jsforce.Promise.prototype.thenCall"></a>[function <span class="apidocSignatureSpan">jsforce.Promise.prototype.</span>thenCall (callback)](#apidoc.element.jsforce.Promise.prototype.thenCall)
- description and source-code
```javascript
thenCall = function (callback) {
  if (_.isFunction(callback)) {
    this.then(function(res) {
      process.nextTick(function() {
        callback(null, res);
      });
    }, function(err) {
      process.nextTick(function() {
        callback(err);
      });
    });
  }
  return this;
}
```
- example usage
```shell
...
  }, function(err) {
    deferred.reject(err);
  });
};

if (refreshDelegate && refreshDelegate._refreshing) {
  refreshDelegate.once('resume', onResume);
  return deferred.promise.thenCall(callback);
}

// hook before sending
self.beforeSend(request);

self.emit('request', request);
logger.debug("<request> method=" + request.method + ", url=" + request.url);
...
```



# <a name="apidoc.module.jsforce.RecordStream"></a>[module jsforce.RecordStream](#apidoc.module.jsforce.RecordStream)

#### <a name="apidoc.element.jsforce.RecordStream.RecordStream"></a>[function <span class="apidocSignatureSpan">jsforce.</span>RecordStream ()](#apidoc.element.jsforce.RecordStream.RecordStream)
- description and source-code
```javascript
RecordStream = function () {
  RecordStream.super_.call(this, { objectMode: true });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Parsable"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Parsable ()](#apidoc.element.jsforce.RecordStream.Parsable)
- description and source-code
```javascript
Parsable = function () {
  Parsable.super_.call(this);
  this._dataStream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Serializable"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Serializable ()](#apidoc.element.jsforce.RecordStream.Serializable)
- description and source-code
```javascript
Serializable = function () {
  Serializable.super_.call(this);
  this._dataStream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.filter"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>filter (fn)](#apidoc.element.jsforce.RecordStream.filter)
- description and source-code
```javascript
filter = function (fn) {
  var filterStream = new RecordStream.Serializable();
  filterStream._transform = function(record, enc, callback) {
    if (fn(record)) { this.push(record); }
    callback();
  };
  return filterStream;
}
```
- example usage
```shell
...
      op = cond.key === "$or" ? "OR" :
           cond.key === "$and" ? "AND" :
           "NOT";
      return createConditionClause(cond.value, op, d);
    default:
      return createFieldExpression(cond.key, cond.value);
  }
}).filter(function(expr) { return expr; });

var paren;
if (operator === 'NOT') {
  paren = depth > 0;
  return (paren ? "(" : "") + "NOT " + conditions[0] + (paren ? ")" : "");
} else {
  paren = depth > 0 && conditions.length > 1;
...
```

#### <a name="apidoc.element.jsforce.RecordStream.map"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>map (fn)](#apidoc.element.jsforce.RecordStream.map)
- description and source-code
```javascript
map = function (fn) {
  var mapStream = new RecordStream.Serializable();
  mapStream._transform = function(record, enc, callback) {
    var rec = fn(record) || record; // if not returned record, use same record
    this.push(rec);
    callback();
  };
  return mapStream;
}
```
- example usage
```shell
...

/**
* create and return cache key from namespace and serialized arguments.
* @private
*/
function createCacheKey(namespace, args) {
 args = Array.prototype.slice.apply(args);
 return namespace + '(' + _.map(args, function(a){ return JSON.stringify(a); }).join(',') + ')';
}

/**
* Enable caching for async call fn to intercept the response and store it to cache.
* The original async calll fn is always invoked.
*
* @protected
...
```

#### <a name="apidoc.element.jsforce.RecordStream.recordMapStream"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>recordMapStream (record, noeval)](#apidoc.element.jsforce.RecordStream.recordMapStream)
- description and source-code
```javascript
recordMapStream = function (record, noeval) {
  return RecordStream.map(function(rec) {
    var mapped = { Id: rec.Id };
    for (var prop in record) {
      mapped[prop] = noeval ? record[prop] : evalMapping(record[prop], rec);
    }
    return mapped;
  });

  function evalMapping(value, mapping) {
    if (_.isString(value)) {
      var m = /^\$\{(\w+)\}$/.exec(value);
      if (m) { return mapping[m[1]]; }
      return value.replace(/\$\{(\w+)\}/g, function($0, prop) {
        var v = mapping[prop];
        return _.isNull(v) || _.isUndefined(v) ? "" : String(v);
      });
    } else {
      return value;
    }
  }
}
```
- example usage
```shell
...
  callback = type;
  type = null;
}
type = type || (this._config && this._config.table);
if (!type) {
  throw new Error("SOQL based query needs SObject type information to bulk update.");
}
var updateStream = _.isFunction(mapping) ? RecordStream.map(mapping) : RecordStream.recordMapStream(mapping);
var batch = this._conn.sobject(type).updateBulk();
var deferred = Promise.defer();
var handleError = function(err) {
  if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
  else { deferred.reject(err); }
};
this.on('error', handleError)
...
```

#### <a name="apidoc.element.jsforce.RecordStream.super_"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>super_ (options)](#apidoc.element.jsforce.RecordStream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er, data) {
      done(stream, er, data);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.RecordStream.Parsable"></a>[module jsforce.RecordStream.Parsable](#apidoc.module.jsforce.RecordStream.Parsable)

#### <a name="apidoc.element.jsforce.RecordStream.Parsable.Parsable"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Parsable ()](#apidoc.element.jsforce.RecordStream.Parsable.Parsable)
- description and source-code
```javascript
Parsable = function () {
  Parsable.super_.call(this);
  this._dataStream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Parsable.super_"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.</span>super_ ()](#apidoc.element.jsforce.RecordStream.Parsable.super_)
- description and source-code
```javascript
super_ = function () {
  RecordStream.super_.call(this, { objectMode: true });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.RecordStream.Parsable.prototype"></a>[module jsforce.RecordStream.Parsable.prototype](#apidoc.module.jsforce.RecordStream.Parsable.prototype)

#### <a name="apidoc.element.jsforce.RecordStream.Parsable.prototype.addListener"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.prototype.</span>addListener (ev, fn)](#apidoc.element.jsforce.RecordStream.Parsable.prototype.addListener)
- description and source-code
```javascript
addListener = function (ev, fn) {
  if (ev === 'readable' || ev === 'record') {
    this._dataStream.pipe(this._parserStream);
  }
  return Parsable.super_.prototype.on.call(this, ev, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Parsable.prototype.on"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.prototype.</span>on (ev, fn)](#apidoc.element.jsforce.RecordStream.Parsable.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  if (ev === 'readable' || ev === 'record') {
    this._dataStream.pipe(this._parserStream);
  }
  return Parsable.super_.prototype.on.call(this, ev, fn);
}
```
- example usage
```shell
...
 * @param {String} [options.responseType] - Overriding content mime-type in response
 * @param {Transport} [options.transport] - Transport for http api
 * @param {Object} [options.noContentResponse] - Alternative response when no content returned in response (= HTTP 204)
 */
var HttpApi = function(conn, options) {
  options = options || {};
  this._conn = conn;
  this.on('resume', function(err) { conn.emit('resume', err); });
  this._responseType = options.responseType;
  this._transport = options.transport || conn._transport;
  this._noContentResponse = options.noContentResponse;
};

inherits(HttpApi, events.EventEmitter);
...
```

#### <a name="apidoc.element.jsforce.RecordStream.Parsable.prototype.stream"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.Parsable.prototype.</span>stream (type, options)](#apidoc.element.jsforce.RecordStream.Parsable.prototype.stream)
- description and source-code
```javascript
stream = function (type, options) {
  type = type || 'csv';
  var converter = DataStreamConverters[type];
  if (!converter) {
    throw new Error('Converting [' + type + '] data stream is not supported.');
  }
  if (!this._dataStream) {
    this._dataStream = new PassThrough();
    this._parserStream = converter.parse(options);
    this._parserStream.pipe(this).pipe(new PassThrough({ objectMode: true, highWaterMark: ( 500 * 1000 ) }));
  }
  return this._dataStream;
}
```
- example usage
```shell
...
 * Get blob field as stream
 *
 * @param {String} fieldName - Blob field name
 * @returns {stream.Stream}
 */
RecordReference.prototype.blob = function(fieldName) {
  var url = [ this._conn._baseUrl(), 'sobjects', this.type, this.id, fieldName ].join('/');
  return this._conn.request(url).stream();
};
...
```



# <a name="apidoc.module.jsforce.RecordStream.Serializable"></a>[module jsforce.RecordStream.Serializable](#apidoc.module.jsforce.RecordStream.Serializable)

#### <a name="apidoc.element.jsforce.RecordStream.Serializable.Serializable"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>Serializable ()](#apidoc.element.jsforce.RecordStream.Serializable.Serializable)
- description and source-code
```javascript
Serializable = function () {
  Serializable.super_.call(this);
  this._dataStream = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.Serializable.super_"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.Serializable.</span>super_ ()](#apidoc.element.jsforce.RecordStream.Serializable.super_)
- description and source-code
```javascript
super_ = function () {
  RecordStream.super_.call(this, { objectMode: true });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.RecordStream.Serializable.prototype"></a>[module jsforce.RecordStream.Serializable.prototype](#apidoc.module.jsforce.RecordStream.Serializable.prototype)

#### <a name="apidoc.element.jsforce.RecordStream.Serializable.prototype.stream"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.Serializable.prototype.</span>stream (type, options)](#apidoc.element.jsforce.RecordStream.Serializable.prototype.stream)
- description and source-code
```javascript
stream = function (type, options) {
  type = type || 'csv';
  var converter = DataStreamConverters[type];
  if (!converter) {
    throw new Error('Converting [' + type + '] data stream is not supported.');
  }
  if (!this._dataStream) {
    this._dataStream = new PassThrough();
    this.pipe(converter.serialize(options))
      .pipe(this._dataStream);
  }
  return this._dataStream;
}
```
- example usage
```shell
...
 * Get blob field as stream
 *
 * @param {String} fieldName - Blob field name
 * @returns {stream.Stream}
 */
RecordReference.prototype.blob = function(fieldName) {
  var url = [ this._conn._baseUrl(), 'sobjects', this.type, this.id, fieldName ].join('/');
  return this._conn.request(url).stream();
};
...
```



# <a name="apidoc.module.jsforce.RecordStream.prototype"></a>[module jsforce.RecordStream.prototype](#apidoc.module.jsforce.RecordStream.prototype)

#### <a name="apidoc.element.jsforce.RecordStream.prototype._transform"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.prototype.</span>_transform (record, enc, callback)](#apidoc.element.jsforce.RecordStream.prototype._transform)
- description and source-code
```javascript
_transform = function (record, enc, callback) {
  this.emit('record', record);
  this.push(record);
  callback();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.prototype.filter"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.prototype.</span>filter (fn)](#apidoc.element.jsforce.RecordStream.prototype.filter)
- description and source-code
```javascript
filter = function (fn) {
  return this.pipe(RecordStream.filter(fn));
}
```
- example usage
```shell
...
      op = cond.key === "$or" ? "OR" :
           cond.key === "$and" ? "AND" :
           "NOT";
      return createConditionClause(cond.value, op, d);
    default:
      return createFieldExpression(cond.key, cond.value);
  }
}).filter(function(expr) { return expr; });

var paren;
if (operator === 'NOT') {
  paren = depth > 0;
  return (paren ? "(" : "") + "NOT " + conditions[0] + (paren ? ")" : "");
} else {
  paren = depth > 0 && conditions.length > 1;
...
```

#### <a name="apidoc.element.jsforce.RecordStream.prototype.map"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.prototype.</span>map (fn)](#apidoc.element.jsforce.RecordStream.prototype.map)
- description and source-code
```javascript
map = function (fn) {
  return this.pipe(RecordStream.map(fn));
}
```
- example usage
```shell
...

/**
* create and return cache key from namespace and serialized arguments.
* @private
*/
function createCacheKey(namespace, args) {
 args = Array.prototype.slice.apply(args);
 return namespace + '(' + _.map(args, function(a){ return JSON.stringify(a); }).join(',') + ')';
}

/**
* Enable caching for async call fn to intercept the response and store it to cache.
* The original async calll fn is always invoked.
*
* @protected
...
```



# <a name="apidoc.module.jsforce.RecordStream.super_"></a>[module jsforce.RecordStream.super_](#apidoc.module.jsforce.RecordStream.super_)

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.</span>super_ (options)](#apidoc.element.jsforce.RecordStream.super_.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.RecordStream.super_.prototype"></a>[module jsforce.RecordStream.super_.prototype](#apidoc.module.jsforce.RecordStream.super_.prototype)

#### <a name="apidoc.element.jsforce.RecordStream.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>_read (n)](#apidoc.element.jsforce.RecordStream.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  var ts = this._transformState;

  if (ts.writechunk !== null && ts.writecb && !ts.transforming) {
    ts.transforming = true;
    this._transform(ts.writechunk, ts.writeencoding, ts.afterTransform);
  } else {
    // mark that we need a transform, so that any data that comes in
    // will get processed, now that we've asked for it.
    ts.needTransform = true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.prototype._transform"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  throw new Error('_transform() is not implemented');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  var ts = this._transformState;
  ts.writecb = cb;
  ts.writechunk = chunk;
  ts.writeencoding = encoding;
  if (!ts.transforming) {
    var rs = this._readableState;
    if (ts.needTransform || rs.needReadable || rs.length < rs.highWaterMark) this._read(rs.highWaterMark);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.jsforce.RecordStream.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  this._transformState.needTransform = false;
  return Duplex.prototype.push.call(this, chunk, encoding);
}
```
- example usage
```shell
...
Cache.prototype.makeResponseCacheable = function(fn, scope, options) {
var cache = this;
options = options || {};
return function() {
  var args = Array.prototype.slice.apply(arguments);
  var callback = args.pop();
  if (!_.isFunction(callback)) {
    args.push(callback);
    callback = null;
  }
  var key = _.isString(options.key) ? options.key :
            _.isFunction(options.key) ? options.key.apply(scope, args) :
            createCacheKey(options.namespace, args);
  var entry = cache.get(key);
  entry.fetching = true;
...
```



# <a name="apidoc.module.jsforce.RecordStream.super_.super_.prototype"></a>[module jsforce.RecordStream.super_.super_.prototype](#apidoc.module.jsforce.RecordStream.super_.super_.prototype)

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('_write() is not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>cork ()](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>uncork ()](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.RecordStream.super_.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">jsforce.RecordStream.super_.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.jsforce.RecordStream.super_.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;
  var isBuf = Buffer.isBuffer(chunk);

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (isBuf) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (isBuf || validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, isBuf, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.SfDate"></a>[module jsforce.SfDate](#apidoc.module.jsforce.SfDate)

#### <a name="apidoc.element.jsforce.SfDate.SfDate"></a>[function <span class="apidocSignatureSpan">jsforce.</span>SfDate (literal)](#apidoc.element.jsforce.SfDate.SfDate)
- description and source-code
```javascript
SfDate = function (literal) {
  this._literal = literal;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_DAYS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_DAYS (num)](#apidoc.element.jsforce.SfDate.LAST_N_DAYS)
- description and source-code
```javascript
LAST_N_DAYS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_FISCAL_QUARTERS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_FISCAL_QUARTERS (num)](#apidoc.element.jsforce.SfDate.LAST_N_FISCAL_QUARTERS)
- description and source-code
```javascript
LAST_N_FISCAL_QUARTERS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_FISCAL_YEARS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_FISCAL_YEARS (num)](#apidoc.element.jsforce.SfDate.LAST_N_FISCAL_YEARS)
- description and source-code
```javascript
LAST_N_FISCAL_YEARS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_MONTHS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_MONTHS (num)](#apidoc.element.jsforce.SfDate.LAST_N_MONTHS)
- description and source-code
```javascript
LAST_N_MONTHS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_QUARTERS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_QUARTERS (num)](#apidoc.element.jsforce.SfDate.LAST_N_QUARTERS)
- description and source-code
```javascript
LAST_N_QUARTERS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_WEEKS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_WEEKS (num)](#apidoc.element.jsforce.SfDate.LAST_N_WEEKS)
- description and source-code
```javascript
LAST_N_WEEKS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.LAST_N_YEARS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>LAST_N_YEARS (num)](#apidoc.element.jsforce.SfDate.LAST_N_YEARS)
- description and source-code
```javascript
LAST_N_YEARS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_DAYS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_DAYS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_DAYS)
- description and source-code
```javascript
NEXT_N_DAYS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_FISCAL_QUARTERS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_FISCAL_QUARTERS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_FISCAL_QUARTERS)
- description and source-code
```javascript
NEXT_N_FISCAL_QUARTERS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_FISCAL_YEARS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_FISCAL_YEARS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_FISCAL_YEARS)
- description and source-code
```javascript
NEXT_N_FISCAL_YEARS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_MONTHS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_MONTHS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_MONTHS)
- description and source-code
```javascript
NEXT_N_MONTHS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_QUARTERS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_QUARTERS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_QUARTERS)
- description and source-code
```javascript
NEXT_N_QUARTERS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_WEEKS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_WEEKS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_WEEKS)
- description and source-code
```javascript
NEXT_N_WEEKS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.NEXT_N_YEARS"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>NEXT_N_YEARS (num)](#apidoc.element.jsforce.SfDate.NEXT_N_YEARS)
- description and source-code
```javascript
NEXT_N_YEARS = function (num) { return new SfDate(literal + ":" + num); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.parseDate"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>parseDate (str)](#apidoc.element.jsforce.SfDate.parseDate)
- description and source-code
```javascript
parseDate = function (str) {
  var d = new Date();
  var regexp = /^([\d]{4})-?([\d]{2})-?([\d]{2})(T([\d]{2}):?([\d]{2}):?([\d]{2})(.([\d]{3}))?(Z|([\+\-])([\d]{2}):?([\d]{2})))?$/;
  var m = str.match(regexp);
  if (m) {
    d = new Date(0);
    if (!m[4]) {
      d.setFullYear(parseInt(m[1], 10));
      d.setDate(parseInt(m[3], 10));
      d.setMonth(parseInt(m[2], 10) - 1);
      d.setHours(0);
      d.setMinutes(0);
      d.setSeconds(0);
      d.setMilliseconds(0);
    } else {
      d.setUTCFullYear(parseInt(m[1], 10));
      d.setUTCDate(parseInt(m[3], 10));
      d.setUTCMonth(parseInt(m[2], 10) - 1);
      d.setUTCHours(parseInt(m[5], 10));
      d.setUTCMinutes(parseInt(m[6], 10));
      d.setUTCSeconds(parseInt(m[7], 10));
      d.setUTCMilliseconds(parseInt(m[9] || '0', 10));
      if (m[10] && m[10] !== 'Z') {
        var offset = parseInt(m[12],10) * 60 + parseInt(m[13], 10);
        d.setTime((m[11] === '+' ? -1 : 1) * offset * 60 * 1000 +d.getTime());
      }
    }
    return d;
  } else {
    throw new Error("Invalid date format is specified : " + str);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.toDateLiteral"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>toDateLiteral (date)](#apidoc.element.jsforce.SfDate.toDateLiteral)
- description and source-code
```javascript
toDateLiteral = function (date) {
  if (_.isNumber(date)) {
    date = new Date(date);
  } else if (_.isString(date)) {
    date = SfDate.parseDate(date);
  }
  var yy = date.getFullYear();
  var mm = date.getMonth()+1;
  var dd = date.getDate();
  var dstr = [ yy, zeropad(mm), zeropad(dd) ].join("-");
  return new SfDate(dstr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.toDateTimeLiteral"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.</span>toDateTimeLiteral (date)](#apidoc.element.jsforce.SfDate.toDateTimeLiteral)
- description and source-code
```javascript
toDateTimeLiteral = function (date) {
  if (_.isNumber(date)) {
    date = new Date(date);
  } else if (_.isString(date)) {
    date = SfDate.parseDate(date);
  }
  var yy = date.getUTCFullYear();
  var mm = date.getUTCMonth()+1;
  var dd = date.getUTCDate();
  var hh = date.getUTCHours();
  var mi = date.getUTCMinutes();
  var ss = date.getUTCSeconds();
  var dtstr =
    [ yy, zeropad(mm), zeropad(dd) ].join("-") + "T" +
    [ zeropad(hh), zeropad(mi), zeropad(ss) ].join(":") + "Z";
  return new SfDate(dtstr);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.SfDate.prototype"></a>[module jsforce.SfDate.prototype](#apidoc.module.jsforce.SfDate.prototype)

#### <a name="apidoc.element.jsforce.SfDate.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.prototype.</span>toJSON ()](#apidoc.element.jsforce.SfDate.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () { return this._literal; }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.SfDate.prototype.toString"></a>[function <span class="apidocSignatureSpan">jsforce.SfDate.prototype.</span>toString ()](#apidoc.element.jsforce.SfDate.prototype.toString)
- description and source-code
```javascript
toString = function () { return this._literal; }
```
- example usage
```shell
...
function createValueExpression(value) {
if (isArray(value)) {
  return value.length > 0 ?
         "(" + value.map(createValueExpression).join(", ") + ")" :
         undefined;
}
if (value instanceof SfDate) {
  return value.toString();
}
if (_.isString(value)) {
  return "'" + escapeSOQLString(value) + "'";
}
if (_.isNumber(value)) {
  return (value).toString();
}
...
```



# <a name="apidoc.module.jsforce._required"></a>[module jsforce._required](#apidoc.module.jsforce._required)

#### <a name="apidoc.element.jsforce._required.inherits"></a>[function <span class="apidocSignatureSpan">jsforce._required.</span>inherits (ctor, superCtor)](#apidoc.element.jsforce._required.inherits)
- description and source-code
```javascript
inherits = function (ctor, superCtor) {

  if (ctor === undefined || ctor === null)
    throw new TypeError('The constructor to "inherits" must not be ' +
                        'null or undefined');

  if (superCtor === undefined || superCtor === null)
    throw new TypeError('The super constructor to "inherits" must not ' +
                        'be null or undefined');

  if (superCtor.prototype === undefined)
    throw new TypeError('The super constructor to "inherits" must ' +
                        'have a prototype');

  ctor.super_ = superCtor;
  Object.setPrototypeOf(ctor.prototype, superCtor.prototype);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce._required.multistream"></a>[function <span class="apidocSignatureSpan">jsforce._required.</span>multistream (streams, opts)](#apidoc.element.jsforce._required.multistream)
- description and source-code
```javascript
function MultiStream(streams, opts) {
  var self = this
  if (!(self instanceof MultiStream)) return new MultiStream(streams, opts)
  stream.Readable.call(self, opts)

  self.destroyed = false

  self._drained = false
  self._forwarding = false
  self._current = null

  if (typeof streams === 'function') {
    self._queue = streams
  } else {
    self._queue = streams.map(toStreams2)
    self._queue.forEach(function (stream) {
      if (typeof stream !== 'function') self._attachErrorListener(stream)
    })
  }

  self._next()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce._required.readable-stream"></a>[function <span class="apidocSignatureSpan">jsforce._required.</span>readable-stream (options)](#apidoc.element.jsforce._required.readable-stream)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.cache"></a>[module jsforce.cache](#apidoc.module.jsforce.cache)

#### <a name="apidoc.element.jsforce.cache.cache"></a>[function <span class="apidocSignatureSpan">jsforce.</span>cache ()](#apidoc.element.jsforce.cache.cache)
- description and source-code
```javascript
cache = function () {
  this._entries = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.cache.prototype"></a>[module jsforce.cache.prototype](#apidoc.module.jsforce.cache.prototype)

#### <a name="apidoc.element.jsforce.cache.prototype.clear"></a>[function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>clear (key)](#apidoc.element.jsforce.cache.prototype.clear)
- description and source-code
```javascript
clear = function (key) {
  for (var k in this._entries) {
    if (!key || k.indexOf(key) === 0) {
      this._entries[k].clear();
    }
  }
}
```
- example usage
```shell
...
/**
* clear cache entries prefix matching given key
* @param {String} [key] - Key prefix of cache entry to clear
*/
Cache.prototype.clear = function(key) {
 for (var k in this._entries) {
   if (!key || k.indexOf(key) === 0) {
     this._entries[k].clear();
   }
 }
};

/**
* create and return cache key from namespace and serialized arguments.
* @private
...
```

#### <a name="apidoc.element.jsforce.cache.prototype.get"></a>[function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>get (key)](#apidoc.element.jsforce.cache.prototype.get)
- description and source-code
```javascript
get = function (key) {
  if (key && this._entries[key]) {
    return this._entries[key];
  } else {
    var entry = new CacheEntry();
    this._entries[key] = entry;
    return entry;
  }
}
```
- example usage
```shell
...
if (!_.isFunction(callback)) {
  args.push(callback);
  callback = null;
}
var key = _.isString(options.key) ? options.key :
          _.isFunction(options.key) ? options.key.apply(scope, args) :
          createCacheKey(options.namespace, args);
var entry = cache.get(key);
entry.fetching = true;
if (callback) {
  args.push(function(err, result) {
    entry.set({ error: err, result: result });
    callback(err, result);
  });
}
...
```

#### <a name="apidoc.element.jsforce.cache.prototype.makeCacheable"></a>[function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>makeCacheable (fn, scope, options)](#apidoc.element.jsforce.cache.prototype.makeCacheable)
- description and source-code
```javascript
makeCacheable = function (fn, scope, options) {
  var cache = this;
  options = options || {};
  var $fn = function() {
    var args = Array.prototype.slice.apply(arguments);
    var callback = args.pop();
    if (!_.isFunction(callback)) {
      args.push(callback);
    }
    var key = _.isString(options.key) ? options.key :
              _.isFunction(options.key) ? options.key.apply(scope, args) :
              createCacheKey(options.namespace, args);
    var entry = cache.get(key);
    if (!_.isFunction(callback)) { // if callback is not given in last arg, return cached result (immediate).
      var value = entry.get();
      if (!value) { throw new Error('Function call result is not cached yet.'); }
      if (value.error) { throw value.error; }
      return value.result;
    }
    entry.get(function(value) {
      callback(value.error, value.result);
    });
    if (!entry.fetching) { // only when no other client is calling function
      entry.fetching = true;
      args.push(function(err, result) {
        entry.set({ error: err, result: result });
      });
      fn.apply(scope || this, args);
    }
  };
  $fn.clear = function() {
    var key = _.isString(options.key) ? options.key :
              _.isFunction(options.key) ? options.key.apply(scope, arguments) :
              createCacheKey(options.namespace, arguments);
    cache.clear(key);
  };
  return $fn;
}
```
- example usage
```shell
...
 *
 * @constructor
 */
var SObject = module.exports = function(conn, type) {
this._conn = conn;
this.type = type;
var cacheOptions = { key: "describe." + this.type };
this.describe$ = conn.cache.makeCacheable(this.describe, this, cacheOptions);
this.describe = conn.cache.makeResponseCacheable(this.describe, this, cacheOptions);

cacheOptions = { key: "layouts." + this.type };
this.layouts$ = conn.cache.makeCacheable(this.layouts, this, cacheOptions);
this.layouts = conn.cache.makeResponseCacheable(this.layouts, this, cacheOptions);

cacheOptions = { key: "compactLayouts." + this.type };
...
```

#### <a name="apidoc.element.jsforce.cache.prototype.makeResponseCacheable"></a>[function <span class="apidocSignatureSpan">jsforce.cache.prototype.</span>makeResponseCacheable (fn, scope, options)](#apidoc.element.jsforce.cache.prototype.makeResponseCacheable)
- description and source-code
```javascript
makeResponseCacheable = function (fn, scope, options) {
  var cache = this;
  options = options || {};
  return function() {
    var args = Array.prototype.slice.apply(arguments);
    var callback = args.pop();
    if (!_.isFunction(callback)) {
      args.push(callback);
      callback = null;
    }
    var key = _.isString(options.key) ? options.key :
              _.isFunction(options.key) ? options.key.apply(scope, args) :
              createCacheKey(options.namespace, args);
    var entry = cache.get(key);
    entry.fetching = true;
    if (callback) {
      args.push(function(err, result) {
        entry.set({ error: err, result: result });
        callback(err, result);
      });
    }
    var ret, error;
    try {
      ret = fn.apply(scope || this, args);
    } catch(e) {
      error = e;
    }
    if (ret && _.isFunction(ret.then)) { // if the returned value is promise
      if (!callback) {
        return ret.then(function(result) {
          entry.set({ error: undefined, result: result });
          return result;
        }, function(err) {
          entry.set({ error: err, result: undefined });
          throw err;
        });
      } else {
        return ret;
      }
    } else {
      entry.set({ error: error, result: ret });
      if (error) { throw error; }
      return ret;
    }
  };
}
```
- example usage
```shell
...
 * @constructor
 */
var SObject = module.exports = function(conn, type) {
this._conn = conn;
this.type = type;
var cacheOptions = { key: "describe." + this.type };
this.describe$ = conn.cache.makeCacheable(this.describe, this, cacheOptions);
this.describe = conn.cache.makeResponseCacheable(this.describe, this, cacheOptions);

cacheOptions = { key: "layouts." + this.type };
this.layouts$ = conn.cache.makeCacheable(this.layouts, this, cacheOptions);
this.layouts = conn.cache.makeResponseCacheable(this.layouts, this, cacheOptions);

cacheOptions = { key: "compactLayouts." + this.type };
this.compactLayouts$ = conn.cache.makeCacheable(this.compactLayouts, this, cacheOptions);
...
```



# <a name="apidoc.module.jsforce.csv"></a>[module jsforce.csv](#apidoc.module.jsforce.csv)

#### <a name="apidoc.element.jsforce.csv.parseCSV"></a>[function <span class="apidocSignatureSpan">jsforce.csv.</span>parseCSV (str, options)](#apidoc.element.jsforce.csv.parseCSV)
- description and source-code
```javascript
function parseCSV(str, options) {
  options = _.extend({}, options, { columns: true });
  return csvParseSync(str, options);
}
```
- example usage
```shell
...
  });
  if (ret.error) { throw ret.error; }
  return ret.result;
}

/** @private */
function parseCSV(str) {
  return require('./csv').parseCSV(str);
}

/** @private */
function parseText(str) { return str; }


/**
...
```

#### <a name="apidoc.element.jsforce.csv.parseCSVStream"></a>[function <span class="apidocSignatureSpan">jsforce.csv.</span>parseCSVStream (options)](#apidoc.element.jsforce.csv.parseCSVStream)
- description and source-code
```javascript
function parseCSVStream(options) {
  options = _.extend({}, options, { columns: true });
  return csvParse(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.csv.serializeCSVStream"></a>[function <span class="apidocSignatureSpan">jsforce.csv.</span>serializeCSVStream (options)](#apidoc.element.jsforce.csv.serializeCSVStream)
- description and source-code
```javascript
function serializeCSVStream(options) {
  options = _.extend({}, options, { header: true });
  return csvStringify(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.csv.toCSV"></a>[function <span class="apidocSignatureSpan">jsforce.csv.</span>toCSV (records, options)](#apidoc.element.jsforce.csv.toCSV)
- description and source-code
```javascript
function toCSV(records, options) {
  options = _.extend({}, options, { header: true });
  return csvStringifySync(records, options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.http_api"></a>[module jsforce.http_api](#apidoc.module.jsforce.http_api)

#### <a name="apidoc.element.jsforce.http_api.http_api"></a>[function <span class="apidocSignatureSpan">jsforce.</span>http_api (conn, options)](#apidoc.element.jsforce.http_api.http_api)
- description and source-code
```javascript
http_api = function (conn, options) {
  options = options || {};
  this._conn = conn;
  this.on('resume', function(err) { conn.emit('resume', err); });
  this._responseType = options.responseType;
  this._transport = options.transport || conn._transport;
  this._noContentResponse = options.noContentResponse;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.http_api.SessionRefreshDelegate"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.</span>SessionRefreshDelegate (conn, refreshFn)](#apidoc.element.jsforce.http_api.SessionRefreshDelegate)
- description and source-code
```javascript
SessionRefreshDelegate = function (conn, refreshFn) {
  this._conn = conn;
  this._refreshFn = refreshFn;
  this._refreshing = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.http_api.super_"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.</span>super_ ()](#apidoc.element.jsforce.http_api.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.http_api.prototype"></a>[module jsforce.http_api.prototype](#apidoc.module.jsforce.http_api.prototype)

#### <a name="apidoc.element.jsforce.http_api.prototype.beforeSend"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>beforeSend (request)](#apidoc.element.jsforce.http_api.prototype.beforeSend)
- description and source-code
```javascript
beforeSend = function (request) {
  request.headers = request.headers || {};
  if (this._conn.accessToken) {
    request.headers.Authorization = "Bearer " + this._conn.accessToken;
  }
  if (this._conn.callOptions) {
    var callOptions = [];
    for (var name in this._conn.callOptions) {
      callOptions.push(name + "=" + this._conn.callOptions[name]);
    }
    request.headers["Sforce-Call-Options"] = callOptions.join(', ');
  }
}
```
- example usage
```shell
...

if (refreshDelegate && refreshDelegate._refreshing) {
  refreshDelegate.once('resume', onResume);
  return deferred.promise.thenCall(callback);
}

// hook before sending
self.beforeSend(request);

self.emit('request', request);
logger.debug("<request> method=" + request.method + ", url=" + request.url);
var requestTime = Date.now();

return this._transport.httpRequest(request).then(function(response) {
  var responseTime = Date.now();
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.getError"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getError (response, body)](#apidoc.element.jsforce.http_api.prototype.getError)
- description and source-code
```javascript
getError = function (response, body) {
  var error;
  try {
    error = this.parseError(body || this.parseResponseBody(response));
  } catch(e) {}
  error = _.isObject(error) && _.isString(error.message) ? error : {
    errorCode: 'ERROR_HTTP_' + response.statusCode,
    message : response.body
  };
  var err = new Error(error.message);
  err.name = error.errorCode;
  for (var key in error) { err[key] = error[key]; }
  return err;
}
```
- example usage
```shell
...
  // Refresh token if session has been expired and requires authentication
  // when session refresh delegate is available
  if (self.isSessionExpired(response) && refreshDelegate) {
    refreshDelegate.refresh(requestTime, onResume);
    return deferred.promise;
  }
  if (self.isErrorResponse(response)) {
    var err = self.getError(response);
    throw err;
  }
  return self.getResponseBody(response);
}, function(err) {
  var responseTime = Date.now();
  logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
  logger.error(err);
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.getRefreshDelegate"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getRefreshDelegate ()](#apidoc.element.jsforce.http_api.prototype.getRefreshDelegate)
- description and source-code
```javascript
getRefreshDelegate = function () {
  return this._conn._refreshDelegate;
}
```
- example usage
```shell
...
 * @param {Callback.<Object>} callback - Callback function
 * @returns {Promise.<Object>} -
 */
HttpApi.prototype.request = function(request, callback) {
var self = this;
var conn = this._conn;
var logger = conn._logger;
var refreshDelegate = this.getRefreshDelegate();
// remember previous instance url in case it changes after a refresh
var lastInstanceUrl = conn.instanceUrl;

var deferred = Promise.defer();

var onResume = function(err) {
  if (err) {
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.getResponseBody"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getResponseBody (response)](#apidoc.element.jsforce.http_api.prototype.getResponseBody)
- description and source-code
```javascript
getResponseBody = function (response) {
  if (response.statusCode === 204) { // No Content
    return this._noContentResponse;
  }
  var body = this.parseResponseBody(response);
  var err;
  if (this.hasErrorInResponseBody(body)) {
    err = this.getError(response, body);
    throw err;
  }
  if (response.statusCode === 300) { // Multiple Choices
    err = new Error('Multiple records found');
    err.name = "MULTIPLE_CHOICES";
    err.content = body;
    throw err;
  }
  return body;
}
```
- example usage
```shell
...
    refreshDelegate.refresh(requestTime, onResume);
    return deferred.promise;
  }
  if (self.isErrorResponse(response)) {
    var err = self.getError(response);
    throw err;
  }
  return self.getResponseBody(response);
}, function(err) {
  var responseTime = Date.now();
  logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
  logger.error(err);
  throw err;
})
.thenCall(callback);
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.getResponseContentType"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>getResponseContentType (response)](#apidoc.element.jsforce.http_api.prototype.getResponseContentType)
- description and source-code
```javascript
getResponseContentType = function (response) {
  return this._responseType || response.headers && response.headers["content-type"];
}
```
- example usage
```shell
...
return this._responseType || response.headers && response.headers["content-type"];
};

/**
 *
 */
HttpApi.prototype.parseResponseBody = function(response) {
var contentType = this.getResponseContentType(response);
var parseBody = /^(text|application)\/xml(;|$)/.test(contentType) ? parseXML :
       /^application\/json(;|$)/.test(contentType) ? parseJSON :
       /^text\/csv(;|$)/.test(contentType) ? parseCSV :
       parseText;
try {
  return parseBody(response.body);
} catch(e) {
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.hasErrorInResponseBody"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>hasErrorInResponseBody (body)](#apidoc.element.jsforce.http_api.prototype.hasErrorInResponseBody)
- description and source-code
```javascript
hasErrorInResponseBody = function (body) {
  return false;
}
```
- example usage
```shell
...
 */
HttpApi.prototype.getResponseBody = function(response) {
if (response.statusCode === 204) { // No Content
  return this._noContentResponse;
}
var body = this.parseResponseBody(response);
var err;
if (this.hasErrorInResponseBody(body)) {
  err = this.getError(response, body);
  throw err;
}
if (response.statusCode === 300) { // Multiple Choices
  err = new Error('Multiple records found');
  err.name = "MULTIPLE_CHOICES";
  err.content = body;
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.isErrorResponse"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>isErrorResponse (response)](#apidoc.element.jsforce.http_api.prototype.isErrorResponse)
- description and source-code
```javascript
isErrorResponse = function (response) {
  return response.statusCode >= 400;
}
```
- example usage
```shell
...
  self.emit('response', response);
  // Refresh token if session has been expired and requires authentication
  // when session refresh delegate is available
  if (self.isSessionExpired(response) && refreshDelegate) {
    refreshDelegate.refresh(requestTime, onResume);
    return deferred.promise;
  }
  if (self.isErrorResponse(response)) {
    var err = self.getError(response);
    throw err;
  }
  return self.getResponseBody(response);
}, function(err) {
  var responseTime = Date.now();
  logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.isSessionExpired"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>isSessionExpired (response)](#apidoc.element.jsforce.http_api.prototype.isSessionExpired)
- description and source-code
```javascript
isSessionExpired = function (response) {
  return response.statusCode === 401;
}
```
- example usage
```shell
...
var responseTime = Date.now();
logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
logger.debug("<response> status=" + response.statusCode + ", url=" + request.url);

self.emit('response', response);
// Refresh token if session has been expired and requires authentication
// when session refresh delegate is available
if (self.isSessionExpired(response) && refreshDelegate) {
  refreshDelegate.refresh(requestTime, onResume);
  return deferred.promise;
}
if (self.isErrorResponse(response)) {
  var err = self.getError(response);
  throw err;
}
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.parseError"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>parseError (body)](#apidoc.element.jsforce.http_api.prototype.parseError)
- description and source-code
```javascript
parseError = function (body) {
  var errors = body;
  return _.isArray(errors) ? errors[0] : errors;
}
```
- example usage
```shell
...
/**
 * Get error message in response
 * @protected
 */
HttpApi.prototype.getError = function(response, body) {
var error;
try {
  error = this.parseError(body || this.parseResponseBody(response));
} catch(e) {}
error = _.isObject(error) && _.isString(error.message) ? error : {
  errorCode: 'ERROR_HTTP_' + response.statusCode,
  message : response.body
};
var err = new Error(error.message);
err.name = error.errorCode;
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.parseResponseBody"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>parseResponseBody (response)](#apidoc.element.jsforce.http_api.prototype.parseResponseBody)
- description and source-code
```javascript
parseResponseBody = function (response) {
  var contentType = this.getResponseContentType(response);
  var parseBody = /^(text|application)\/xml(;|$)/.test(contentType) ? parseXML :
         /^application\/json(;|$)/.test(contentType) ? parseJSON :
         /^text\/csv(;|$)/.test(contentType) ? parseCSV :
         parseText;
  try {
    return parseBody(response.body);
  } catch(e) {
    return response.body;
  }
}
```
- example usage
```shell
...
 * Get response body
 * @protected
 */
HttpApi.prototype.getResponseBody = function(response) {
if (response.statusCode === 204) { // No Content
  return this._noContentResponse;
}
var body = this.parseResponseBody(response);
var err;
if (this.hasErrorInResponseBody(body)) {
  err = this.getError(response, body);
  throw err;
}
if (response.statusCode === 300) { // Multiple Choices
  err = new Error('Multiple records found');
...
```

#### <a name="apidoc.element.jsforce.http_api.prototype.request"></a>[function <span class="apidocSignatureSpan">jsforce.http_api.prototype.</span>request (request, callback)](#apidoc.element.jsforce.http_api.prototype.request)
- description and source-code
```javascript
request = function (request, callback) {
  var self = this;
  var conn = this._conn;
  var logger = conn._logger;
  var refreshDelegate = this.getRefreshDelegate();
  // remember previous instance url in case it changes after a refresh
  var lastInstanceUrl = conn.instanceUrl;

  var deferred = Promise.defer();

  var onResume = function(err) {
    if (err) {
      deferred.reject(err);
      return;
    }
    // check to see if the token refresh has changed the instance url
    if(lastInstanceUrl !== conn.instanceUrl){
      // if the instance url has changed
      // then replace the current request urls instance url fragment
      // with the updated instance url
      request.url = request.url.replace(lastInstanceUrl,conn.instanceUrl);
    }

    self.request(request).then(function(response) {
      deferred.resolve(response);
    }, function(err) {
      deferred.reject(err);
    });
  };

  if (refreshDelegate && refreshDelegate._refreshing) {
    refreshDelegate.once('resume', onResume);
    return deferred.promise.thenCall(callback);
  }

  // hook before sending
  self.beforeSend(request);

  self.emit('request', request);
  logger.debug("<request> method=" + request.method + ", url=" + request.url);
  var requestTime = Date.now();

  return this._transport.httpRequest(request).then(function(response) {
    var responseTime = Date.now();
    logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
    logger.debug("<response> status=" + response.statusCode + ", url=" + request.url);

    self.emit('response', response);
    // Refresh token if session has been expired and requires authentication
    // when session refresh delegate is available
    if (self.isSessionExpired(response) && refreshDelegate) {
      refreshDelegate.refresh(requestTime, onResume);
      return deferred.promise;
    }
    if (self.isErrorResponse(response)) {
      var err = self.getError(response);
      throw err;
    }
    return self.getResponseBody(response);
  }, function(err) {
    var responseTime = Date.now();
    logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
    logger.error(err);
    throw err;
  })
  .thenCall(callback);
}
```
- example usage
```shell
...
  if(lastInstanceUrl !== conn.instanceUrl){
    // if the instance url has changed
    // then replace the current request urls instance url fragment
    // with the updated instance url
    request.url = request.url.replace(lastInstanceUrl,conn.instanceUrl);
  }

  self.request(request).then(function(response) {
    deferred.resolve(response);
  }, function(err) {
    deferred.reject(err);
  });
};

if (refreshDelegate && refreshDelegate._refreshing) {
...
```



# <a name="apidoc.module.jsforce.logger"></a>[module jsforce.logger](#apidoc.module.jsforce.logger)

#### <a name="apidoc.element.jsforce.logger.logger"></a>[function <span class="apidocSignatureSpan">jsforce.</span>logger (logLevel)](#apidoc.element.jsforce.logger.logger)
- description and source-code
```javascript
logger = function (logLevel) {
  if (typeof logLevel === 'string') {
    logLevel = LogLevels[logLevel];
  }
  if (!logLevel) {
    logLevel = LogLevels.INFO;
  }
  this._logLevel = logLevel;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.logger.prototype"></a>[module jsforce.logger.prototype](#apidoc.module.jsforce.logger.prototype)

#### <a name="apidoc.element.jsforce.logger.prototype.debug"></a>[function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>debug (message)](#apidoc.element.jsforce.logger.prototype.debug)
- description and source-code
```javascript
debug = function (message) { this.log(level, message); }
```
- example usage
```shell
...
  return deferred.promise.thenCall(callback);
}

// hook before sending
self.beforeSend(request);

self.emit('request', request);
logger.debug("<request> method=" + request.method + ", url=" + request.url);
var requestTime = Date.now();

return this._transport.httpRequest(request).then(function(response) {
  var responseTime = Date.now();
  logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
  logger.debug("<response> status=" + response.statusCode + ", url=" + request.url);
...
```

#### <a name="apidoc.element.jsforce.logger.prototype.error"></a>[function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>error (message)](#apidoc.element.jsforce.logger.prototype.error)
- description and source-code
```javascript
error = function (message) { this.log(level, message); }
```
- example usage
```shell
...
     var err = self.getError(response);
     throw err;
   }
   return self.getResponseBody(response);
 }, function(err) {
   var responseTime = Date.now();
   logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
   logger.error(err);
   throw err;
 })
 .thenCall(callback);
};

/**
* @protected
...
```

#### <a name="apidoc.element.jsforce.logger.prototype.fatal"></a>[function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>fatal (message)](#apidoc.element.jsforce.logger.prototype.fatal)
- description and source-code
```javascript
fatal = function (message) { this.log(level, message); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.logger.prototype.info"></a>[function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>info (message)](#apidoc.element.jsforce.logger.prototype.info)
- description and source-code
```javascript
info = function (message) { this.log(level, message); }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.logger.prototype.log"></a>[function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>log (level, message)](#apidoc.element.jsforce.logger.prototype.log)
- description and source-code
```javascript
log = function (level, message) {
  if (this._logLevel <= level) {
    if (level < LogLevels.ERROR) {
      console.log(message);
    } else {
      console.error(message);
    }
  }
}
```
- example usage
```shell
...
 *
 * @param {String} level - Logging target level
 * @param {String} message - Message to log
 */
Logger.prototype.log = function(level, message) {
  if (this._logLevel <= level) {
    if (level < LogLevels.ERROR) {
      console.log(message);
    } else {
      console.error(message);
    }
  }
};

for (var level in LogLevels) {
...
```

#### <a name="apidoc.element.jsforce.logger.prototype.warn"></a>[function <span class="apidocSignatureSpan">jsforce.logger.prototype.</span>warn (message)](#apidoc.element.jsforce.logger.prototype.warn)
- description and source-code
```javascript
warn = function (message) { this.log(level, message); }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.query"></a>[module jsforce.query](#apidoc.module.jsforce.query)

#### <a name="apidoc.element.jsforce.query.query"></a>[function <span class="apidocSignatureSpan">jsforce.</span>query (conn, config, options)](#apidoc.element.jsforce.query.query)
- description and source-code
```javascript
query = function (conn, config, options) {
  Query.super_.call(this, { objectMode: true });

  this._conn = conn;
  if (_.isString(config)) { // if query config is string, it is given in SOQL.
    this._soql = config;
  } else if (config.locator && config.locator.indexOf("/") >= 0) { // if locator given in url for next records
    this._locator = config.locator.split("/").pop();
  } else {
    this._config = config;
    this.select(config.fields);
    if (config.includes) {
      this.include(config.includes);
    }
  }
  this._options = _.defaults({
    maxFetch: 10000,
    autoFetch: false,
    scanAll: false,
    responseTarget: ResponseTargets.QueryResult
  }, options || {});
  this._executed = false;
  this._finished = false;
  this._chaining = false;

  this._deferred = Promise.defer();

  var self = this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.super_"></a>[function <span class="apidocSignatureSpan">jsforce.query.</span>super_ (options)](#apidoc.element.jsforce.query.super_)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.query.prototype"></a>[module jsforce.query.prototype](#apidoc.module.jsforce.query.prototype)

#### <a name="apidoc.element.jsforce.query.prototype._execute"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>_execute (options)](#apidoc.element.jsforce.query.prototype._execute)
- description and source-code
```javascript
_execute = function (options) {
  var self = this;
  var logger = this._conn._logger;
  var responseTarget = options.responseTarget;
  var autoFetch = options.autoFetch;
  var maxFetch = options.maxFetch;
  var scanAll = options.scanAll;

  return Promise.resolve(
    self._locator ?
    self._conn._baseUrl() + "/query/" + self._locator :
    self.toSOQL().then(function(soql) {
      self.totalFetched = 0;
      logger.debug("SOQL = " + soql);
      return self._conn._baseUrl() + "/" + (scanAll ? "queryAll" : "query") + "?q=" + encodeURIComponent(soql);
    })
  ).then(function(url) {
    return self._conn.request({
      method: 'GET',
      url: url,
      headers: options.headers
    });
  }).then(function(data) {
    self.emit("fetch");
    self.totalSize = data.totalSize;
    var res;
    switch(responseTarget) {
      case ResponseTargets.SingleRecord:
        res = data.records && data.records.length > 0 ? data.records[0] : null;
        break;
      case ResponseTargets.Records:
        res = data.records;
        break;
      case ResponseTargets.Count:
        res = data.totalSize;
        break;
      default:
        res = data;
    }
    // only fire response event when it should be notified per fetch
    if (responseTarget !== ResponseTargets.Records) {
      self.emit("response", res, self);
    }

    // streaming record instances
    for (var i=0, l=data.records.length; i<l; i++) {
      if (self.totalFetched >= maxFetch) {
        self._finished = true;
        break;
      }
      var record = data.records[i];
      self.push(record);
      self.emit('record', record, self.totalFetched++, self);
    }
    if (data.nextRecordsUrl) {
      self._locator = data.nextRecordsUrl.split('/').pop();
    }
    self._finished = self._finished || data.done || !autoFetch;
    if (self._finished) {
      self.push(null);
    } else {
      self._execute(options);
    }
    return res;
  });
}
```
- example usage
```shell
...
});

// flag to prevent re-execution
this._executed = true;

// start actual query
logger.debug('>>> Query start >>>');
this._execute(options).then(function() {
  logger.debug('*** Query finished ***');
}).fail(function(err) {
  logger.debug('--- Query error ---');
  self.emit('error', err);
});

// return Query instance for chaining
...
```

#### <a name="apidoc.element.jsforce.query.prototype._expandFields"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>_expandFields ()](#apidoc.element.jsforce.query.prototype._expandFields)
- description and source-code
```javascript
_expandFields = function () {
  if (this._soql) {
    return Promise.reject(new Error("Cannot expand fields for the query which has already built SOQL."));
  }
  var self = this;
  var logger = self._conn._logger;
  var conn = this._conn;
  var table = this._config.table;
  var fields = this._config.fields || [];

  logger.debug('_expandFields: table = ' + table + ', fields = ' + fields.join(', '));

  return Promise.all([
    Promise.resolve(self._parent ? findRelationTable(table) : table)
      .then(function(table) {
        return Promise.all(
          _.map(fields, function(field) { return expandAsteriskField(table, field); })
        ).then(function(expandedFields) {
          self._config.fields = _.flatten(expandedFields);
        });
      }),
    Promise.all(
      _.map(self._children || [], function(childQuery) {
        return childQuery._expandFields();
      })
    )
  ]);

  function findRelationTable(rname) {
    var ptable = self._parent._config.table;
    logger.debug('finding table for relation "' + rname + '" in "' + ptable + '"...');
    return describeCache(ptable).then(function(sobject) {
      var upperRname = rname.toUpperCase();
      var childRelation = _.find(sobject.childRelationships, function(cr) {
        return (cr.relationshipName || '').toUpperCase() === upperRname;
      });
      return childRelation ? childRelation.childSObject :
        Promise.reject(new Error("No child relationship found: " + rname ));
    });
  }

  function describeCache(table) {
    logger.debug('describe cache: '+table);
    var deferred = Promise.defer();
    conn.describe$(table, function(err, sobject) {
      logger.debug('... done.');
      if (err) { deferred.reject(err); }
      else { deferred.resolve(sobject); }
    });
    return deferred.promise;
  }

  function expandAsteriskField(table, field) {
    logger.debug('expanding field "'+ field + '" in "' + table + '"...');
    var fpath = field.split('.');
    return fpath[fpath.length - 1] === '*' ?
      describeCache(table).then(function(sobject) {
        logger.debug('table '+table+'has been described');
        if (fpath.length > 1) {
          var rname = fpath.shift();
          var rfield = _.find(sobject.fields, function(f) {
            return f.relationshipName &&
                   f.relationshipName.toUpperCase() === rname.toUpperCase();
          });
          if (rfield) {
            var rtable = rfield.referenceTo.length === 1 ? rfield.referenceTo[0] : 'Name';
            return expandAsteriskField(rtable, fpath.join('.')).then(function(fpaths) {
              return _.map(fpaths, function(fpath) { return rname + '.' + fpath; });
            });
          } else {
            return [];
          }
        } else {
          return _.map(sobject.fields, function(f) { return f.name; });
        }
      }) :
      Promise.resolve([ field ]);
  }
}
```
- example usage
```shell
...
        _.map(fields, function(field) { return expandAsteriskField(table, field); })
      ).then(function(expandedFields) {
        self._config.fields = _.flatten(expandedFields);
      });
    }),
  Promise.all(
    _.map(self._children || [], function(childQuery) {
      return childQuery._expandFields();
    })
  )
]);

function findRelationTable(rname) {
  var ptable = self._parent._config.table;
  logger.debug('finding table for relation "' + rname + '" in "' + ptable + '"...');
...
```

#### <a name="apidoc.element.jsforce.query.prototype._read"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>_read (size)](#apidoc.element.jsforce.query.prototype._read)
- description and source-code
```javascript
_read = function (size) {
  if (!this._finished && !this._executed) {
    this.execute({ autoFetch: true });
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.addListener"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>addListener (e, fn)](#apidoc.element.jsforce.query.prototype.addListener)
- description and source-code
```javascript
addListener = function (e, fn) {
  if (e === 'record') {
    var self = this;
    this.on('readable', function() {
      while(self.read() !== null) {} // discard buffered records
    });
  }
  return Query.super_.prototype.on.call(this, e, fn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.autoFetch"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>autoFetch (autoFetch)](#apidoc.element.jsforce.query.prototype.autoFetch)
- description and source-code
```javascript
autoFetch = function (autoFetch) {
  this._options.autoFetch = autoFetch;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.del"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>del (type, callback)](#apidoc.element.jsforce.query.prototype.del)
- description and source-code
```javascript
del = function (type, callback) {
  if (typeof type === 'function') {
    callback = type;
    type = null;
  }
  type = type || (this._config && this._config.table);
  if (!type) {
    throw new Error("SOQL based query needs SObject type information to bulk delete.");
  }
  var batch = this._conn.sobject(type).deleteBulk();
  var deferred = Promise.defer();
  var handleError = function(err) {
    if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
    else { deferred.reject(err); }
  };
  this.on('error', handleError)
    .pipe(batch)
    .on('response', function(res) { deferred.resolve(res); })
    .on('error', handleError);
  return deferred.promise.thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.delete"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>delete (type, callback)](#apidoc.element.jsforce.query.prototype.delete)
- description and source-code
```javascript
delete = function (type, callback) {
  if (typeof type === 'function') {
    callback = type;
    type = null;
  }
  type = type || (this._config && this._config.table);
  if (!type) {
    throw new Error("SOQL based query needs SObject type information to bulk delete.");
  }
  var batch = this._conn.sobject(type).deleteBulk();
  var deferred = Promise.defer();
  var handleError = function(err) {
    if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
    else { deferred.reject(err); }
  };
  this.on('error', handleError)
    .pipe(batch)
    .on('response', function(res) { deferred.resolve(res); })
    .on('error', handleError);
  return deferred.promise.thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.destroy"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>destroy (type, callback)](#apidoc.element.jsforce.query.prototype.destroy)
- description and source-code
```javascript
destroy = function (type, callback) {
  if (typeof type === 'function') {
    callback = type;
    type = null;
  }
  type = type || (this._config && this._config.table);
  if (!type) {
    throw new Error("SOQL based query needs SObject type information to bulk delete.");
  }
  var batch = this._conn.sobject(type).deleteBulk();
  var deferred = Promise.defer();
  var handleError = function(err) {
    if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
    else { deferred.reject(err); }
  };
  this.on('error', handleError)
    .pipe(batch)
    .on('response', function(res) { deferred.resolve(res); })
    .on('error', handleError);
  return deferred.promise.thenCall(callback);
}
```
- example usage
```shell
...
* @returns {Promise.<RecordResult>}
*/
RecordReference.prototype.destroy = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.destroy(this.type, this.id, options, callback);
};

/**
* Get blob field as stream
*
* @param {String} fieldName - Blob field name
* @returns {stream.Stream}
...
```

#### <a name="apidoc.element.jsforce.query.prototype.exec"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>exec (options, callback)](#apidoc.element.jsforce.query.prototype.exec)
- description and source-code
```javascript
exec = function (options, callback) {
  var self = this;
  var logger = this._conn._logger;
  var deferred = this._deferred;

  if (this._executed) {
    deferred.reject(new Error("re-executing already executed query"));
    return this;
  }

  if (this._finished) {
    deferred.reject(new Error("executing already closed query"));
    return this;
  }

  if (typeof options === "function") {
    callback = options;
    options = {};
  }
  options = options || {};
  options = {
    headers: options.headers || self._options.headers,
    responseTarget: options.responseTarget || self._options.responseTarget,
    autoFetch: options.autoFetch || self._options.autoFetch,
    maxFetch: options.maxFetch || self._options.maxFetch,
    scanAll: options.scanAll || self._options.scanAll
  };

  // callback and promise resolution;
  var promiseCallback = function(err, res) {
    if (_.isFunction(callback)) {
      try {
        res = callback(err, res);
        err = null;
      } catch(e) {
        err = e;
      }
    }
    if (err) {
      deferred.reject(err);
    } else {
      deferred.resolve(res);
    }
  };
  this.once('response', function(res) {
    promiseCallback(null, res);
  });
  this.once('error', function(err) {
    promiseCallback(err);
  });

  // collect fetched records in array
  // only when response target is Records and
  // either callback or chaining promises are available to this query.
  this.once('fetch', function() {
    if (options.responseTarget === ResponseTargets.Records && (self._chaining || callback)) {
      logger.debug('--- collecting all fetched records ---');
      var records = [];
      var onRecord = function(record) {
        records.push(record);
      };
      self.on('record', onRecord);
      self.once('end', function() {
        self.removeListener('record', onRecord);
        self.emit('response', records, self);
      });
    }
  });

  // flag to prevent re-execution
  this._executed = true;

  // start actual query
  logger.debug('>>> Query start >>>');
  this._execute(options).then(function() {
    logger.debug('*** Query finished ***');
  }).fail(function(err) {
    logger.debug('--- Query error ---');
    self.emit('error', err);
  });

  // return Query instance for chaining
  return this;
}
```
- example usage
```shell
...
}

/**
 * Normarize Salesforce API host name
 * @private
 */
function normalizeApiHost(apiHost) {
  var m = /(\w+)\.(visual\.force|salesforce)\.com$/.exec(apiHost);
  if (m) {
    apiHost = m[1] + ".salesforce.com";
  }
  return apiHost;
}

/**
...
```

#### <a name="apidoc.element.jsforce.query.prototype.execute"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>execute (options, callback)](#apidoc.element.jsforce.query.prototype.execute)
- description and source-code
```javascript
execute = function (options, callback) {
  var self = this;
  var logger = this._conn._logger;
  var deferred = this._deferred;

  if (this._executed) {
    deferred.reject(new Error("re-executing already executed query"));
    return this;
  }

  if (this._finished) {
    deferred.reject(new Error("executing already closed query"));
    return this;
  }

  if (typeof options === "function") {
    callback = options;
    options = {};
  }
  options = options || {};
  options = {
    headers: options.headers || self._options.headers,
    responseTarget: options.responseTarget || self._options.responseTarget,
    autoFetch: options.autoFetch || self._options.autoFetch,
    maxFetch: options.maxFetch || self._options.maxFetch,
    scanAll: options.scanAll || self._options.scanAll
  };

  // callback and promise resolution;
  var promiseCallback = function(err, res) {
    if (_.isFunction(callback)) {
      try {
        res = callback(err, res);
        err = null;
      } catch(e) {
        err = e;
      }
    }
    if (err) {
      deferred.reject(err);
    } else {
      deferred.resolve(res);
    }
  };
  this.once('response', function(res) {
    promiseCallback(null, res);
  });
  this.once('error', function(err) {
    promiseCallback(err);
  });

  // collect fetched records in array
  // only when response target is Records and
  // either callback or chaining promises are available to this query.
  this.once('fetch', function() {
    if (options.responseTarget === ResponseTargets.Records && (self._chaining || callback)) {
      logger.debug('--- collecting all fetched records ---');
      var records = [];
      var onRecord = function(record) {
        records.push(record);
      };
      self.on('record', onRecord);
      self.once('end', function() {
        self.removeListener('record', onRecord);
        self.emit('response', records, self);
      });
    }
  });

  // flag to prevent re-execution
  this._executed = true;

  // start actual query
  logger.debug('>>> Query start >>>');
  this._execute(options).then(function() {
    logger.debug('*** Query finished ***');
  }).fail(function(err) {
    logger.debug('--- Query error ---');
    self.emit('error', err);
  });

  // return Query instance for chaining
  return this;
}
```
- example usage
```shell
...
 * Readable stream implementation
 *
 * @override
 * @private
 */
Query.prototype._read = function(size) {
if (!this._finished && !this._executed) {
  this.execute({ autoFetch: true });
}
};

/** @override **/
Query.prototype.on = function(e, fn) {
if (e === 'record') {
  var self = this;
...
```

#### <a name="apidoc.element.jsforce.query.prototype.explain"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>explain (callback)](#apidoc.element.jsforce.query.prototype.explain)
- description and source-code
```javascript
explain = function (callback) {
  var self = this;
  var logger = this._conn._logger;
  return self.toSOQL().then(function(soql) {
    logger.debug("SOQL = " + soql);
    var url = "/query/?explain=" + encodeURIComponent(soql);
    return self._conn.request(url);
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.filter"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>filter (fn)](#apidoc.element.jsforce.query.prototype.filter)
- description and source-code
```javascript
filter = function (fn) {
  return this.pipe(RecordStream.map(fn));
}
```
- example usage
```shell
...
      op = cond.key === "$or" ? "OR" :
           cond.key === "$and" ? "AND" :
           "NOT";
      return createConditionClause(cond.value, op, d);
    default:
      return createFieldExpression(cond.key, cond.value);
  }
}).filter(function(expr) { return expr; });

var paren;
if (operator === 'NOT') {
  paren = depth > 0;
  return (paren ? "(" : "") + "NOT " + conditions[0] + (paren ? ")" : "");
} else {
  paren = depth > 0 && conditions.length > 1;
...
```

#### <a name="apidoc.element.jsforce.query.prototype.include"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>include (childRelName, conditions, fields, options)](#apidoc.element.jsforce.query.prototype.include)
- description and source-code
```javascript
include = function (childRelName, conditions, fields, options) {
  if (this._soql) {
    throw Error("Cannot include child relationship into the query which has already built SOQL.");
  }
  if (_.isObject(childRelName)) {
    var includes = childRelName;
    for (var crname in includes) {
      var config = includes[crname];
      this.include(crname, config.conditions, config.fields, config);
    }
    return;
  }
  var childConfig = {
    table: childRelName,
    conditions: conditions,
    fields: fields,
    limit: options && options.limit,
    offset: options && (options.offset || options.skip),
    sort: options && options.sort
  };
  if (!_.isArray(this._config.includes)) this._config.includes = [];
  this._config.includes.push(childConfig);
  var childQuery = new SubQuery(this._conn, this, childConfig);
  this._children = this._children || [];
  this._children.push(childQuery);
  return childQuery;
}
```
- example usage
```shell
...
  this._soql = config;
} else if (config.locator && config.locator.indexOf("/") >= 0) { // if locator given in url for next records
  this._locator = config.locator.split("/").pop();
} else {
  this._config = config;
  this.select(config.fields);
  if (config.includes) {
    this.include(config.includes);
  }
}
this._options = _.defaults({
  maxFetch: 10000,
  autoFetch: false,
  scanAll: false,
  responseTarget: ResponseTargets.QueryResult
...
```

#### <a name="apidoc.element.jsforce.query.prototype.limit"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>limit (limit)](#apidoc.element.jsforce.query.prototype.limit)
- description and source-code
```javascript
limit = function (limit) {
  if (this._soql) {
    throw Error("Cannot set limit for the query which has already built SOQL.");
  }
  this._config.limit = limit;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.map"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>map (fn)](#apidoc.element.jsforce.query.prototype.map)
- description and source-code
```javascript
map = function (fn) {
  return this.pipe(RecordStream.map(fn));
}
```
- example usage
```shell
...

/**
* create and return cache key from namespace and serialized arguments.
* @private
*/
function createCacheKey(namespace, args) {
 args = Array.prototype.slice.apply(args);
 return namespace + '(' + _.map(args, function(a){ return JSON.stringify(a); }).join(',') + ')';
}

/**
* Enable caching for async call fn to intercept the response and store it to cache.
* The original async calll fn is always invoked.
*
* @protected
...
```

#### <a name="apidoc.element.jsforce.query.prototype.maxFetch"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>maxFetch (maxFetch)](#apidoc.element.jsforce.query.prototype.maxFetch)
- description and source-code
```javascript
maxFetch = function (maxFetch) {
  this._options.maxFetch = maxFetch;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.offset"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>offset (offset)](#apidoc.element.jsforce.query.prototype.offset)
- description and source-code
```javascript
offset = function (offset) {
  if (this._soql) {
    throw Error("Cannot set skip/offset for the query which has already built SOQL.");
  }
  this._config.offset = offset;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.on"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>on (e, fn)](#apidoc.element.jsforce.query.prototype.on)
- description and source-code
```javascript
on = function (e, fn) {
  if (e === 'record') {
    var self = this;
    this.on('readable', function() {
      while(self.read() !== null) {} // discard buffered records
    });
  }
  return Query.super_.prototype.on.call(this, e, fn);
}
```
- example usage
```shell
...
 * @param {String} [options.responseType] - Overriding content mime-type in response
 * @param {Transport} [options.transport] - Transport for http api
 * @param {Object} [options.noContentResponse] - Alternative response when no content returned in response (= HTTP 204)
 */
var HttpApi = function(conn, options) {
  options = options || {};
  this._conn = conn;
  this.on('resume', function(err) { conn.emit('resume', err); });
  this._responseType = options.responseType;
  this._transport = options.transport || conn._transport;
  this._noContentResponse = options.noContentResponse;
};

inherits(HttpApi, events.EventEmitter);
...
```

#### <a name="apidoc.element.jsforce.query.prototype.orderby"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>orderby (sort, dir)](#apidoc.element.jsforce.query.prototype.orderby)
- description and source-code
```javascript
orderby = function (sort, dir) {
  if (this._soql) {
    throw Error("Cannot set sort for the query which has already built SOQL.");
  }
  if (_.isString(sort) && _.isString(dir)) {
    sort = [ [ sort, dir ] ];
  }
  this._config.sort = sort;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.run"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>run (options, callback)](#apidoc.element.jsforce.query.prototype.run)
- description and source-code
```javascript
run = function (options, callback) {
  var self = this;
  var logger = this._conn._logger;
  var deferred = this._deferred;

  if (this._executed) {
    deferred.reject(new Error("re-executing already executed query"));
    return this;
  }

  if (this._finished) {
    deferred.reject(new Error("executing already closed query"));
    return this;
  }

  if (typeof options === "function") {
    callback = options;
    options = {};
  }
  options = options || {};
  options = {
    headers: options.headers || self._options.headers,
    responseTarget: options.responseTarget || self._options.responseTarget,
    autoFetch: options.autoFetch || self._options.autoFetch,
    maxFetch: options.maxFetch || self._options.maxFetch,
    scanAll: options.scanAll || self._options.scanAll
  };

  // callback and promise resolution;
  var promiseCallback = function(err, res) {
    if (_.isFunction(callback)) {
      try {
        res = callback(err, res);
        err = null;
      } catch(e) {
        err = e;
      }
    }
    if (err) {
      deferred.reject(err);
    } else {
      deferred.resolve(res);
    }
  };
  this.once('response', function(res) {
    promiseCallback(null, res);
  });
  this.once('error', function(err) {
    promiseCallback(err);
  });

  // collect fetched records in array
  // only when response target is Records and
  // either callback or chaining promises are available to this query.
  this.once('fetch', function() {
    if (options.responseTarget === ResponseTargets.Records && (self._chaining || callback)) {
      logger.debug('--- collecting all fetched records ---');
      var records = [];
      var onRecord = function(record) {
        records.push(record);
      };
      self.on('record', onRecord);
      self.once('end', function() {
        self.removeListener('record', onRecord);
        self.emit('response', records, self);
      });
    }
  });

  // flag to prevent re-execution
  this._executed = true;

  // start actual query
  logger.debug('>>> Query start >>>');
  this._execute(options).then(function() {
    logger.debug('*** Query finished ***');
  }).fail(function(err) {
    logger.debug('--- Query error ---');
    self.emit('error', err);
  });

  // return Query instance for chaining
  return this;
}
```
- example usage
```shell
...
   table: this.type,
   conditions: conditions,
   limit: options.limit,
   offset: options.offset || options.skip
 };
 var query = new Query(this._conn, config, options);
 query.setResponseTarget(Query.ResponseTargets.Records);
 if (callback) { query.run(callback); }
 return query;
};

/**
* Fetch one record which matches given conditions
*
* @param {Object|String} [conditions] - Conditions in JSON object (MongoDB-like), or raw SOQL WHERE clause string.
...
```

#### <a name="apidoc.element.jsforce.query.prototype.scanAll"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>scanAll (scanAll)](#apidoc.element.jsforce.query.prototype.scanAll)
- description and source-code
```javascript
scanAll = function (scanAll) {
  this._options.scanAll = scanAll;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.select"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>select (fields)](#apidoc.element.jsforce.query.prototype.select)
- description and source-code
```javascript
select = function (fields) {
  if (this._soql) {
    throw Error("Cannot set select fields for the query which has already built SOQL.");
  }
  fields = fields || '*';
  if (_.isString(fields)) {
    fields = fields.split(/\s*,\s*/);
  } else if (_.isObject(fields) && !_.isArray(fields)) {
    var _fields =  [];
    for (var k in fields) {
      if (fields[k]) { _fields.push(k); }
    }
    fields = _fields;
  }
  this._config.fields = fields;
  return this;
}
```
- example usage
```shell
...
this._conn = conn;
if (_.isString(config)) { // if query config is string, it is given in SOQL.
  this._soql = config;
} else if (config.locator && config.locator.indexOf("/") >= 0) { // if locator given in url for next records
  this._locator = config.locator.split("/").pop();
} else {
  this._config = config;
  this.select(config.fields);
  if (config.includes) {
    this.include(config.includes);
  }
}
this._options = _.defaults({
  maxFetch: 10000,
  autoFetch: false,
...
```

#### <a name="apidoc.element.jsforce.query.prototype.setResponseTarget"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>setResponseTarget (responseTarget)](#apidoc.element.jsforce.query.prototype.setResponseTarget)
- description and source-code
```javascript
setResponseTarget = function (responseTarget) {
  if (responseTarget in ResponseTargets) {
    this._options.responseTarget = responseTarget;
  }
  return this;
}
```
- example usage
```shell
...
   includes: options.includes,
   table: this.type,
   conditions: conditions,
   limit: options.limit,
   offset: options.offset || options.skip
 };
 var query = new Query(this._conn, config, options);
 query.setResponseTarget(Query.ResponseTargets.Records);
 if (callback) { query.run(callback); }
 return query;
};

/**
* Fetch one record which matches given conditions
*
...
```

#### <a name="apidoc.element.jsforce.query.prototype.skip"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>skip (offset)](#apidoc.element.jsforce.query.prototype.skip)
- description and source-code
```javascript
skip = function (offset) {
  if (this._soql) {
    throw Error("Cannot set skip/offset for the query which has already built SOQL.");
  }
  this._config.offset = offset;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.sort"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>sort (sort, dir)](#apidoc.element.jsforce.query.prototype.sort)
- description and source-code
```javascript
sort = function (sort, dir) {
  if (this._soql) {
    throw Error("Cannot set sort for the query which has already built SOQL.");
  }
  if (_.isString(sort) && _.isString(dir)) {
    sort = [ [ sort, dir ] ];
  }
  this._config.sort = sort;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.query.prototype.stream"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>stream (type, options)](#apidoc.element.jsforce.query.prototype.stream)
- description and source-code
```javascript
stream = function (type, options) {
  type = type || 'csv';
  var converter = DataStreamConverters[type];
  if (!converter) {
    throw new Error('Converting [' + type + '] data stream is not supported.');
  }
  if (!this._dataStream) {
    this._dataStream = new PassThrough();
    this.pipe(converter.serialize(options))
      .pipe(this._dataStream);
  }
  return this._dataStream;
}
```
- example usage
```shell
...
 * Get blob field as stream
 *
 * @param {String} fieldName - Blob field name
 * @returns {stream.Stream}
 */
RecordReference.prototype.blob = function(fieldName) {
  var url = [ this._conn._baseUrl(), 'sobjects', this.type, this.id, fieldName ].join('/');
  return this._conn.request(url).stream();
};
...
```

#### <a name="apidoc.element.jsforce.query.prototype.then"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>then (onResolved, onReject)](#apidoc.element.jsforce.query.prototype.then)
- description and source-code
```javascript
then = function (onResolved, onReject) {
  this._chaining = true;
  if (!this._finished && !this._executed) { this.execute(); }
  return this._deferred.promise.then.apply(this._deferred.promise, arguments);
}
```
- example usage
```shell
...
try {
  ret = fn.apply(scope || this, args);
} catch(e) {
  error = e;
}
if (ret && _.isFunction(ret.then)) { // if the returned value is promise
  if (!callback) {
    return ret.then(function(result) {
      entry.set({ error: undefined, result: result });
      return result;
    }, function(err) {
      entry.set({ error: err, result: undefined });
      throw err;
    });
  } else {
...
```

#### <a name="apidoc.element.jsforce.query.prototype.thenCall"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>thenCall (callback)](#apidoc.element.jsforce.query.prototype.thenCall)
- description and source-code
```javascript
thenCall = function (callback) {
  if (_.isFunction(callback)) {
    this.then(function(res) {
      process.nextTick(function() {
        callback(null, res);
      });
    }, function(err) {
      process.nextTick(function() {
        callback(err);
      });
    });
  }
  return this;
}
```
- example usage
```shell
...
  }, function(err) {
    deferred.reject(err);
  });
};

if (refreshDelegate && refreshDelegate._refreshing) {
  refreshDelegate.once('resume', onResume);
  return deferred.promise.thenCall(callback);
}

// hook before sending
self.beforeSend(request);

self.emit('request', request);
logger.debug("<request> method=" + request.method + ", url=" + request.url);
...
```

#### <a name="apidoc.element.jsforce.query.prototype.toSOQL"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>toSOQL (callback)](#apidoc.element.jsforce.query.prototype.toSOQL)
- description and source-code
```javascript
toSOQL = function (callback) {
  var self = this;
  return Promise.resolve(self._soql ||
    self._expandFields().then(function() { return SOQLBuilder.createSOQL(self._config); })
  ).thenCall(callback);
}
```
- example usage
```shell
...
var autoFetch = options.autoFetch;
var maxFetch = options.maxFetch;
var scanAll = options.scanAll;

return Promise.resolve(
  self._locator ?
  self._conn._baseUrl() + "/query/" + self._locator :
  self.toSOQL().then(function(soql) {
    self.totalFetched = 0;
    logger.debug("SOQL = " + soql);
    return self._conn._baseUrl() + "/" + (scanAll ? "queryAll" : "query") + "?q=" + encodeURIComponent(soql);
  })
).then(function(url) {
  return self._conn.request({
    method: 'GET',
...
```

#### <a name="apidoc.element.jsforce.query.prototype.update"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>update (mapping, type, callback)](#apidoc.element.jsforce.query.prototype.update)
- description and source-code
```javascript
update = function (mapping, type, callback) {
  if (typeof type === 'function') {
    callback = type;
    type = null;
  }
  type = type || (this._config && this._config.table);
  if (!type) {
    throw new Error("SOQL based query needs SObject type information to bulk update.");
  }
  var updateStream = _.isFunction(mapping) ? RecordStream.map(mapping) : RecordStream.recordMapStream(mapping);
  var batch = this._conn.sobject(type).updateBulk();
  var deferred = Promise.defer();
  var handleError = function(err) {
    if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
    else { deferred.reject(err); }
  };
  this.on('error', handleError)
    .pipe(updateStream)
    .on('error', handleError)
    .pipe(batch)
    .on('response', function(res) { deferred.resolve(res); })
    .on('error', handleError);
  return deferred.promise.thenCall(callback);
}
```
- example usage
```shell
...
RecordReference.prototype.update = function(record, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 record = _.clone(record);
 record.Id = this.id;
 return this._conn.update(this.type, record, options, callback);
};

/**
* Synonym of Record#destroy()
*
* @method RecordReference#delete
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.query.prototype.where"></a>[function <span class="apidocSignatureSpan">jsforce.query.prototype.</span>where (conditions)](#apidoc.element.jsforce.query.prototype.where)
- description and source-code
```javascript
where = function (conditions) {
  if (this._soql) {
    throw Error("Cannot set where conditions for the query which has already built SOQL.");
  }
  this._config.conditions = conditions;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.quick_action"></a>[module jsforce.quick_action](#apidoc.module.jsforce.quick_action)

#### <a name="apidoc.element.jsforce.quick_action.quick_action"></a>[function <span class="apidocSignatureSpan">jsforce.</span>quick_action (conn, path)](#apidoc.element.jsforce.quick_action.quick_action)
- description and source-code
```javascript
quick_action = function (conn, path) {
  this._conn = conn;
  this._path = path;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.quick_action.prototype"></a>[module jsforce.quick_action.prototype](#apidoc.module.jsforce.quick_action.prototype)

#### <a name="apidoc.element.jsforce.quick_action.prototype.defaultValues"></a>[function <span class="apidocSignatureSpan">jsforce.quick_action.prototype.</span>defaultValues (contextId, callback)](#apidoc.element.jsforce.quick_action.prototype.defaultValues)
- description and source-code
```javascript
defaultValues = function (contextId, callback) {
  if (typeof contextId === 'function') {
    callback = contextId;
    contextId = null;
  }
  var url = this._path + "/defaultValues";
  if (contextId) {
    url += "/" + contextId;
  }
  return this._conn.request(url).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.quick_action.prototype.describe"></a>[function <span class="apidocSignatureSpan">jsforce.quick_action.prototype.</span>describe (callback)](#apidoc.element.jsforce.quick_action.prototype.describe)
- description and source-code
```javascript
describe = function (callback) {
  var url = this._path + "/describe";
  return this._conn.request(url).thenCall(callback);
}
```
- example usage
```shell
...
/**
* Describe SObject metadata
*
* @param {Callback.<DescribeSObjectResult>} [callback] - Callback function
* @returns {Promise.<DescribeSObjectResult>}
*/
SObject.prototype.describe = function(callback) {
 return this._conn.describe(this.type, callback);
};

/**
* Get record representation instance by given id
*
* @param {String} id - A record ID
* @returns {RecordReference}
...
```

#### <a name="apidoc.element.jsforce.quick_action.prototype.execute"></a>[function <span class="apidocSignatureSpan">jsforce.quick_action.prototype.</span>execute (contextId, record, callback)](#apidoc.element.jsforce.quick_action.prototype.execute)
- description and source-code
```javascript
execute = function (contextId, record, callback) {
  var body = {
    contextId: contextId,
    record: record
  };
  return this._conn.requestPost(this._path, body).thenCall(callback);
}
```
- example usage
```shell
...
 * Readable stream implementation
 *
 * @override
 * @private
 */
Query.prototype._read = function(size) {
if (!this._finished && !this._executed) {
  this.execute({ autoFetch: true });
}
};

/** @override **/
Query.prototype.on = function(e, fn) {
if (e === 'record') {
  var self = this;
...
```



# <a name="apidoc.module.jsforce.record"></a>[module jsforce.record](#apidoc.module.jsforce.record)

#### <a name="apidoc.element.jsforce.record.record"></a>[function <span class="apidocSignatureSpan">jsforce.</span>record (conn, type, id)](#apidoc.element.jsforce.record.record)
- description and source-code
```javascript
record = function (conn, type, id) {
  this._conn = conn;
  this.type = type;
  this.id = id;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.record.prototype"></a>[module jsforce.record.prototype](#apidoc.module.jsforce.record.prototype)

#### <a name="apidoc.element.jsforce.record.prototype.blob"></a>[function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>blob (fieldName)](#apidoc.element.jsforce.record.prototype.blob)
- description and source-code
```javascript
blob = function (fieldName) {
  var url = [ this._conn._baseUrl(), 'sobjects', this.type, this.id, fieldName ].join('/');
  return this._conn.request(url).stream();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.record.prototype.del"></a>[function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>del (options, callback)](#apidoc.element.jsforce.record.prototype.del)
- description and source-code
```javascript
del = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.destroy(this.type, this.id, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.record.prototype.delete"></a>[function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>delete (options, callback)](#apidoc.element.jsforce.record.prototype.delete)
- description and source-code
```javascript
delete = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.destroy(this.type, this.id, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.record.prototype.destroy"></a>[function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>destroy (options, callback)](#apidoc.element.jsforce.record.prototype.destroy)
- description and source-code
```javascript
destroy = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.destroy(this.type, this.id, options, callback);
}
```
- example usage
```shell
...
* @returns {Promise.<RecordResult>}
*/
RecordReference.prototype.destroy = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.destroy(this.type, this.id, options, callback);
};

/**
* Get blob field as stream
*
* @param {String} fieldName - Blob field name
* @returns {stream.Stream}
...
```

#### <a name="apidoc.element.jsforce.record.prototype.retrieve"></a>[function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>retrieve (options, callback)](#apidoc.element.jsforce.record.prototype.retrieve)
- description and source-code
```javascript
retrieve = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.retrieve(this.type, this.id, options, callback);
}
```
- example usage
```shell
...
* @returns {Promise.<Record>}
*/
RecordReference.prototype.retrieve = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.retrieve(this.type, this.id, options, callback);
};

/**
* Update record field information
*
* @param {Record} record - A Record which includes fields to update
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.record.prototype.update"></a>[function <span class="apidocSignatureSpan">jsforce.record.prototype.</span>update (record, options, callback)](#apidoc.element.jsforce.record.prototype.update)
- description and source-code
```javascript
update = function (record, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  record = _.clone(record);
  record.Id = this.id;
  return this._conn.update(this.type, record, options, callback);
}
```
- example usage
```shell
...
RecordReference.prototype.update = function(record, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 record = _.clone(record);
 record.Id = this.id;
 return this._conn.update(this.type, record, options, callback);
};

/**
* Synonym of Record#destroy()
*
* @method RecordReference#delete
* @param {Object} [options] - Options for rest api.
...
```



# <a name="apidoc.module.jsforce.soap"></a>[module jsforce.soap](#apidoc.module.jsforce.soap)

#### <a name="apidoc.element.jsforce.soap.soap"></a>[function <span class="apidocSignatureSpan">jsforce.</span>soap (conn, options)](#apidoc.element.jsforce.soap.soap)
- description and source-code
```javascript
soap = function (conn, options) {
  SOAP.super_.apply(this, arguments);
  this._endpointUrl = options.endpointUrl;
  this._xmlns = options.xmlns || 'urn:partner.soap.sforce.com';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.soap.super_"></a>[function <span class="apidocSignatureSpan">jsforce.soap.</span>super_ (conn, options)](#apidoc.element.jsforce.soap.super_)
- description and source-code
```javascript
super_ = function (conn, options) {
  options = options || {};
  this._conn = conn;
  this.on('resume', function(err) { conn.emit('resume', err); });
  this._responseType = options.responseType;
  this._transport = options.transport || conn._transport;
  this._noContentResponse = options.noContentResponse;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.soap.prototype"></a>[module jsforce.soap.prototype](#apidoc.module.jsforce.soap.prototype)

#### <a name="apidoc.element.jsforce.soap.prototype._createEnvelope"></a>[function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>_createEnvelope (message)](#apidoc.element.jsforce.soap.prototype._createEnvelope)
- description and source-code
```javascript
_createEnvelope = function (message) {
  var header = {};
  var conn = this._conn;
  if (conn.accessToken) {
    header.SessionHeader = { sessionId: this._conn.accessToken };
  }
  if (conn.callOptions) {
    header.CallOptions = conn.callOptions;
  }
  return [
    '<?xml version="1.0" encoding="UTF-8"?>',
    '<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"',
    ' xmlns:xsd="http://www.w3.org/2001/XMLSchema"',
    ' xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">',
    '<soapenv:Header xmlns="' + this._xmlns + '">',
    toXML(header),
    '</soapenv:Header>',
    '<soapenv:Body xmlns="' + this._xmlns + '">',
    toXML(message),
    '</soapenv:Body>',
    '</soapenv:Envelope>'
  ].join('');
}
```
- example usage
```shell
...
      }
    }
  }
}

/** @override **/
SOAP.prototype.beforeSend = function(request) {
  request.body = this._createEnvelope(request.message);
};

/** @override **/
SOAP.prototype.isSessionExpired = function(response) {
  return response.statusCode === 500 &&
    /<faultcode>[a-zA-Z]+:INVALID_SESSION_ID<\/faultcode>/.test(response.body);
};
...
```

#### <a name="apidoc.element.jsforce.soap.prototype.beforeSend"></a>[function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>beforeSend (request)](#apidoc.element.jsforce.soap.prototype.beforeSend)
- description and source-code
```javascript
beforeSend = function (request) {
  request.body = this._createEnvelope(request.message);
}
```
- example usage
```shell
...

if (refreshDelegate && refreshDelegate._refreshing) {
  refreshDelegate.once('resume', onResume);
  return deferred.promise.thenCall(callback);
}

// hook before sending
self.beforeSend(request);

self.emit('request', request);
logger.debug("<request> method=" + request.method + ", url=" + request.url);
var requestTime = Date.now();

return this._transport.httpRequest(request).then(function(response) {
  var responseTime = Date.now();
...
```

#### <a name="apidoc.element.jsforce.soap.prototype.getResponseBody"></a>[function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>getResponseBody (response)](#apidoc.element.jsforce.soap.prototype.getResponseBody)
- description and source-code
```javascript
getResponseBody = function (response) {
  var body = SOAP.super_.prototype.getResponseBody.call(this, response);
  return lookupValue(body, [ /:Envelope$/, /:Body$/, /.+/ ]);
}
```
- example usage
```shell
...
    refreshDelegate.refresh(requestTime, onResume);
    return deferred.promise;
  }
  if (self.isErrorResponse(response)) {
    var err = self.getError(response);
    throw err;
  }
  return self.getResponseBody(response);
}, function(err) {
  var responseTime = Date.now();
  logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
  logger.error(err);
  throw err;
})
.thenCall(callback);
...
```

#### <a name="apidoc.element.jsforce.soap.prototype.invoke"></a>[function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>invoke (method, args, schema, callback)](#apidoc.element.jsforce.soap.prototype.invoke)
- description and source-code
```javascript
invoke = function (method, args, schema, callback) {
  if (typeof schema === 'function') {
    callback = schema;
    schema = null;
  }
  var message = {};
  message[method] = args;
  return this.request({
    method: 'POST',
    url: this._endpointUrl,
    headers: {
      'Content-Type': 'text/xml',
      'SOAPAction': '""'
    },
    message: message
  }).then(function(res) {
    return schema ? convertType(res, schema) : res;
  }).thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.soap.prototype.isSessionExpired"></a>[function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>isSessionExpired (response)](#apidoc.element.jsforce.soap.prototype.isSessionExpired)
- description and source-code
```javascript
isSessionExpired = function (response) {
  return response.statusCode === 500 &&
    /<faultcode>[a-zA-Z]+:INVALID_SESSION_ID<\/faultcode>/.test(response.body);
}
```
- example usage
```shell
...
var responseTime = Date.now();
logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
logger.debug("<response> status=" + response.statusCode + ", url=" + request.url);

self.emit('response', response);
// Refresh token if session has been expired and requires authentication
// when session refresh delegate is available
if (self.isSessionExpired(response) && refreshDelegate) {
  refreshDelegate.refresh(requestTime, onResume);
  return deferred.promise;
}
if (self.isErrorResponse(response)) {
  var err = self.getError(response);
  throw err;
}
...
```

#### <a name="apidoc.element.jsforce.soap.prototype.parseError"></a>[function <span class="apidocSignatureSpan">jsforce.soap.prototype.</span>parseError (body)](#apidoc.element.jsforce.soap.prototype.parseError)
- description and source-code
```javascript
parseError = function (body) {
  var error = lookupValue(body, [ /:Envelope$/, /:Body$/, /:Fault$/ ]);
  return {
    errorCode: error.faultcode,
    message: error.faultstring
  };
}
```
- example usage
```shell
...
/**
 * Get error message in response
 * @protected
 */
HttpApi.prototype.getError = function(response, body) {
var error;
try {
  error = this.parseError(body || this.parseResponseBody(response));
} catch(e) {}
error = _.isObject(error) && _.isString(error.message) ? error : {
  errorCode: 'ERROR_HTTP_' + response.statusCode,
  message : response.body
};
var err = new Error(error.message);
err.name = error.errorCode;
...
```



# <a name="apidoc.module.jsforce.sobject"></a>[module jsforce.sobject](#apidoc.module.jsforce.sobject)

#### <a name="apidoc.element.jsforce.sobject.sobject"></a>[function <span class="apidocSignatureSpan">jsforce.</span>sobject (conn, type)](#apidoc.element.jsforce.sobject.sobject)
- description and source-code
```javascript
sobject = function (conn, type) {
  this._conn = conn;
  this.type = type;
  var cacheOptions = { key: "describe." + this.type };
  this.describe$ = conn.cache.makeCacheable(this.describe, this, cacheOptions);
  this.describe = conn.cache.makeResponseCacheable(this.describe, this, cacheOptions);

  cacheOptions = { key: "layouts." + this.type };
  this.layouts$ = conn.cache.makeCacheable(this.layouts, this, cacheOptions);
  this.layouts = conn.cache.makeResponseCacheable(this.layouts, this, cacheOptions);

  cacheOptions = { key: "compactLayouts." + this.type };
  this.compactLayouts$ = conn.cache.makeCacheable(this.compactLayouts, this, cacheOptions);
  this.compactLayouts = conn.cache.makeResponseCacheable(this.compactLayouts, this, cacheOptions);

  cacheOptions = { key: "approvalLayouts." + this.type };
  this.approvalLayouts$ = conn.cache.makeCacheable(this.approvalLayouts, this, cacheOptions);
  this.approvalLayouts = conn.cache.makeResponseCacheable(this.approvalLayouts, this, cacheOptions);
}
```
- example usage
```shell
...
  callback = type;
  type = null;
}
type = type || (this._config && this._config.table);
if (!type) {
  throw new Error("SOQL based query needs SObject type information to bulk delete.");
}
var batch = this._conn.sobject(type).deleteBulk();
var deferred = Promise.defer();
var handleError = function(err) {
  if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
  else { deferred.reject(err); }
};
this.on('error', handleError)
  .pipe(batch)
...
```



# <a name="apidoc.module.jsforce.sobject.prototype"></a>[module jsforce.sobject.prototype](#apidoc.module.jsforce.sobject.prototype)

#### <a name="apidoc.element.jsforce.sobject.prototype.approvalLayouts"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>approvalLayouts (callback)](#apidoc.element.jsforce.sobject.prototype.approvalLayouts)
- description and source-code
```javascript
approvalLayouts = function (callback) {
  var url = "/sobjects/" + this.type + "/describe/approvalLayouts";
  return this._conn.request(url, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.bulkload"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>bulkload (operation, options, input, callback)](#apidoc.element.jsforce.sobject.prototype.bulkload)
- description and source-code
```javascript
bulkload = function (operation, options, input, callback) {
  return this._conn.bulk.load(this.type, operation, options, input, callback);
}
```
- example usage
```shell
...
* @method SObject#createBulk
* @param {Array.<Record>|stream.Stream|String} [input] - Input source for bulk insert. Accepts array of records, CSv string, and
 CSV data input stream.
* @param {Callback.<Array.<RecordResult>>} [callback] - Callback function
* @returns {Bulk~Batch}
*/
SObject.prototype.insertBulk =
SObject.prototype.createBulk = function(input, callback) {
 return this.bulkload("insert", input, callback);
};

/**
* Bulkly update records by input data using bulk API
*
* @param {Array.<Record>|stream.Stream|String} [input] - Input source for bulk update Accepts array of records, CSv string, and
CSV data input stream.
* @param {Callback.<Array.<RecordResult>>} [callback] - Callback function
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.compactLayouts"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>compactLayouts (callback)](#apidoc.element.jsforce.sobject.prototype.compactLayouts)
- description and source-code
```javascript
compactLayouts = function (callback) {
  var url = "/sobjects/" + this.type + "/describe/compactLayouts";
  return this._conn.request(url, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.count"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>count (conditions, callback)](#apidoc.element.jsforce.sobject.prototype.count)
- description and source-code
```javascript
count = function (conditions, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
  }
  var query = this.find(conditions, { "count()" : true });
  query.setResponseTarget("Count");
  if (callback) { query.run(callback); }
  return query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.create"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>create (records, options, callback)](#apidoc.element.jsforce.sobject.prototype.create)
- description and source-code
```javascript
create = function (records, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.create(this.type, records, options, callback);
}
```
- example usage
```shell
...
*/
SObject.prototype.insert =
SObject.prototype.create = function(records, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.create(this.type, records, options, callback);
};

/**
* Retrieve specified records
*
* @param {String|Array.<String>} ids - A record ID or array of record IDs
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.createBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>createBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.createBulk)
- description and source-code
```javascript
createBulk = function (input, callback) {
  return this.bulkload("insert", input, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.del"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>del (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.del)
- description and source-code
```javascript
del = function (ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.destroy(this.type, ids, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.delete"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>delete (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.delete)
- description and source-code
```javascript
delete = function (ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.destroy(this.type, ids, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.deleteBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>deleteBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.deleteBulk)
- description and source-code
```javascript
deleteBulk = function (input, callback) {
  return this.bulkload("delete", input, callback);
}
```
- example usage
```shell
...
  callback = type;
  type = null;
}
type = type || (this._config && this._config.table);
if (!type) {
  throw new Error("SOQL based query needs SObject type information to bulk delete.");
}
var batch = this._conn.sobject(type).deleteBulk();
var deferred = Promise.defer();
var handleError = function(err) {
  if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
  else { deferred.reject(err); }
};
this.on('error', handleError)
  .pipe(batch)
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.deleteHardBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>deleteHardBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.deleteHardBulk)
- description and source-code
```javascript
deleteHardBulk = function (input, callback) {
  return this.bulkload("hardDelete", input, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.deleted"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>deleted (start, end, callback)](#apidoc.element.jsforce.sobject.prototype.deleted)
- description and source-code
```javascript
deleted = function (start, end, callback) {
  return this._conn.deleted(this.type, start, end, callback);
}
```
- example usage
```shell
...
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
* @param {Callback.<DeletedRecordsInfo>} [callback] - Callback function
* @returns {Promise.<DeletedRecordsInfo>}
*/
SObject.prototype.deleted = function (start, end, callback) {
 return this._conn.deleted(this.type, start, end, callback);
};

/**
* @typedef {Object} LayoutInfo
* @prop {Array.<Object>} layouts - Array of layouts
* @prop {Array.<Object>} recordTypeMappings - Array of record type mappings
*/
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.describe"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>describe (callback)](#apidoc.element.jsforce.sobject.prototype.describe)
- description and source-code
```javascript
describe = function (callback) {
  return this._conn.describe(this.type, callback);
}
```
- example usage
```shell
...
/**
* Describe SObject metadata
*
* @param {Callback.<DescribeSObjectResult>} [callback] - Callback function
* @returns {Promise.<DescribeSObjectResult>}
*/
SObject.prototype.describe = function(callback) {
 return this._conn.describe(this.type, callback);
};

/**
* Get record representation instance by given id
*
* @param {String} id - A record ID
* @returns {RecordReference}
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.destroy"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>destroy (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.destroy)
- description and source-code
```javascript
destroy = function (ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.destroy(this.type, ids, options, callback);
}
```
- example usage
```shell
...
* @returns {Promise.<RecordResult>}
*/
RecordReference.prototype.destroy = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.destroy(this.type, this.id, options, callback);
};

/**
* Get blob field as stream
*
* @param {String} fieldName - Blob field name
* @returns {stream.Stream}
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.destroyBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>destroyBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.destroyBulk)
- description and source-code
```javascript
destroyBulk = function (input, callback) {
  return this.bulkload("delete", input, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.destroyHardBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>destroyHardBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.destroyHardBulk)
- description and source-code
```javascript
destroyHardBulk = function (input, callback) {
  return this.bulkload("hardDelete", input, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.find"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>find (conditions, fields, options, callback)](#apidoc.element.jsforce.sobject.prototype.find)
- description and source-code
```javascript
find = function (conditions, fields, options, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
    fields = null;
    options = null;
  } else if (typeof fields === 'function') {
    callback = fields;
    fields = null;
    options = null;
  } else if (typeof options === 'function') {
    callback = options;
    options = null;
  }
  options = options || {};
  var config = {
    fields: fields,
    includes: options.includes,
    table: this.type,
    conditions: conditions,
    limit: options.limit,
    offset: options.offset || options.skip
  };
  var query = new Query(this._conn, config, options);
  query.setResponseTarget(Query.ResponseTargets.Records);
  if (callback) { query.run(callback); }
  return query;
}
```
- example usage
```shell
...
]);

function findRelationTable(rname) {
  var ptable = self._parent._config.table;
  logger.debug('finding table for relation "' + rname + '" in "' + ptable + '"...');
  return describeCache(ptable).then(function(sobject) {
    var upperRname = rname.toUpperCase();
    var childRelation = _.find(sobject.childRelationships, function(cr) {
      return (cr.relationshipName || '').toUpperCase() === upperRname;
    });
    return childRelation ? childRelation.childSObject :
      Promise.reject(new Error("No child relationship found: " + rname ));
  });
}
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.findOne"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>findOne (conditions, fields, options, callback)](#apidoc.element.jsforce.sobject.prototype.findOne)
- description and source-code
```javascript
findOne = function (conditions, fields, options, callback) {
  if (typeof conditions === 'function') {
    callback = conditions;
    conditions = {};
    fields = null;
    options = null;
  } else if (typeof fields === 'function') {
    callback = fields;
    fields = null;
    options = null;
  } else if (typeof options === 'function') {
    callback = options;
    options = null;
  }
  options = _.extend(options || {}, { limit: 1 });
  var query = this.find(conditions, fields, options);
  query.setResponseTarget(Query.ResponseTargets.SingleRecord);
  if (callback) { query.run(callback); }
  return query;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.insert"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>insert (records, options, callback)](#apidoc.element.jsforce.sobject.prototype.insert)
- description and source-code
```javascript
insert = function (records, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.create(this.type, records, options, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.insertBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>insertBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.insertBulk)
- description and source-code
```javascript
insertBulk = function (input, callback) {
  return this.bulkload("insert", input, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.layouts"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>layouts (layoutName, callback)](#apidoc.element.jsforce.sobject.prototype.layouts)
- description and source-code
```javascript
layouts = function (layoutName, callback) {
  if (typeof layoutName === 'function') {
    callback = layoutName;
    layoutName = null;
  }
  var url = "/sobjects/" + this.type + "/describe/" + (layoutName ? "namedLayouts/"+layoutName : "layouts");
  return this._conn.request(url, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.listview"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>listview (id)](#apidoc.element.jsforce.sobject.prototype.listview)
- description and source-code
```javascript
listview = function (id) {
  return new ListView(this._conn, this.type, id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.listviews"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>listviews (callback)](#apidoc.element.jsforce.sobject.prototype.listviews)
- description and source-code
```javascript
listviews = function (callback) {
  var url = this._conn._baseUrl() + '/sobjects/' + this.type + '/listviews';
  return this._conn.request(url, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.quickAction"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>quickAction (actionName)](#apidoc.element.jsforce.sobject.prototype.quickAction)
- description and source-code
```javascript
quickAction = function (actionName) {
  return new QuickAction(this._conn, "/sobjects/" + this.type + "/quickActions/" + actionName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.quickActions"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>quickActions (callback)](#apidoc.element.jsforce.sobject.prototype.quickActions)
- description and source-code
```javascript
quickActions = function (callback) {
  return this._conn.request("/sobjects/" + this.type + "/quickActions").thenCall(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.recent"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>recent (callback)](#apidoc.element.jsforce.sobject.prototype.recent)
- description and source-code
```javascript
recent = function (callback) {
  return this._conn.recent(this.type, callback);
}
```
- example usage
```shell
...
/**
* Retrieve recently accessed records
*
* @param {Callback.<Array.<RecordResult>>} [callback] - Callback function
* @returns {Promise.<Array.<RecordResult>>}
*/
SObject.prototype.recent = function (callback) {
 return this._conn.recent(this.type, callback);
};

/**
* Retrieve the updated records
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.record"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>record (id)](#apidoc.element.jsforce.sobject.prototype.record)
- description and source-code
```javascript
record = function (id) {
  return new Record(this._conn, this.type, id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.sobject.prototype.retrieve"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>retrieve (ids, options, callback)](#apidoc.element.jsforce.sobject.prototype.retrieve)
- description and source-code
```javascript
retrieve = function (ids, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.retrieve(this.type, ids, options, callback);
}
```
- example usage
```shell
...
* @returns {Promise.<Record>}
*/
RecordReference.prototype.retrieve = function(options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.retrieve(this.type, this.id, options, callback);
};

/**
* Update record field information
*
* @param {Record} record - A Record which includes fields to update
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.select"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>select (fields, callback)](#apidoc.element.jsforce.sobject.prototype.select)
- description and source-code
```javascript
select = function (fields, callback) {
  return this.find(null, fields, null, callback);
}
```
- example usage
```shell
...
this._conn = conn;
if (_.isString(config)) { // if query config is string, it is given in SOQL.
  this._soql = config;
} else if (config.locator && config.locator.indexOf("/") >= 0) { // if locator given in url for next records
  this._locator = config.locator.split("/").pop();
} else {
  this._config = config;
  this.select(config.fields);
  if (config.includes) {
    this.include(config.includes);
  }
}
this._options = _.defaults({
  maxFetch: 10000,
  autoFetch: false,
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.update"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>update (records, options, callback)](#apidoc.element.jsforce.sobject.prototype.update)
- description and source-code
```javascript
update = function (records, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.update(this.type, records, options, callback);
}
```
- example usage
```shell
...
RecordReference.prototype.update = function(record, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 record = _.clone(record);
 record.Id = this.id;
 return this._conn.update(this.type, record, options, callback);
};

/**
* Synonym of Record#destroy()
*
* @method RecordReference#delete
* @param {Object} [options] - Options for rest api.
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.updateBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>updateBulk (input, callback)](#apidoc.element.jsforce.sobject.prototype.updateBulk)
- description and source-code
```javascript
updateBulk = function (input, callback) {
  return this.bulkload("update", input, callback);
}
```
- example usage
```shell
...
  type = null;
}
type = type || (this._config && this._config.table);
if (!type) {
  throw new Error("SOQL based query needs SObject type information to bulk update.");
}
var updateStream = _.isFunction(mapping) ? RecordStream.map(mapping) : RecordStream.recordMapStream(mapping);
var batch = this._conn.sobject(type).updateBulk();
var deferred = Promise.defer();
var handleError = function(err) {
  if (err.name === 'ClientInputError') { deferred.resolve([]); } // if batch input receives no records
  else { deferred.reject(err); }
};
this.on('error', handleError)
  .pipe(updateStream)
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.updated"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>updated (start, end, callback)](#apidoc.element.jsforce.sobject.prototype.updated)
- description and source-code
```javascript
updated = function (start, end, callback) {
  return this._conn.updated(this.type, start, end, callback);
}
```
- example usage
```shell
...
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
* @param {Callback.<UpdatedRecordsInfo>} [callback] - Callback function
* @returns {Promise.<UpdatedRecordsInfo>}
*/
SObject.prototype.updated = function (start, end, callback) {
 return this._conn.updated(this.type, start, end, callback);
};

/**
* Retrieve the deleted records
*
* @param {String|Date} start - start date or string representing the start of the interval
* @param {String|Date} end - start date or string representing the end of the interval, must be > start
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.upsert"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>upsert (records, extIdField, options, callback)](#apidoc.element.jsforce.sobject.prototype.upsert)
- description and source-code
```javascript
upsert = function (records, extIdField, options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  return this._conn.upsert(this.type, records, extIdField, options, callback);
}
```
- example usage
```shell
...
* @returns {Promise.<RecordResult|Array.<RecordResult>>}
*/
SObject.prototype.upsert = function(records, extIdField, options, callback) {
 if (typeof options === 'function') {
   callback = options;
   options = {};
 }
 return this._conn.upsert(this.type, records, extIdField, options, callback);
};

/**
* Synonym of SObject#destroy()
*
* @method SObject#delete
* @param {String|Array.<String>} ids - A ID or array of IDs to delete
...
```

#### <a name="apidoc.element.jsforce.sobject.prototype.upsertBulk"></a>[function <span class="apidocSignatureSpan">jsforce.sobject.prototype.</span>upsertBulk (input, extIdField, callback)](#apidoc.element.jsforce.sobject.prototype.upsertBulk)
- description and source-code
```javascript
upsertBulk = function (input, extIdField, callback) {
  return this.bulkload("upsert", { extIdField: extIdField }, input, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.soql_builder"></a>[module jsforce.soql_builder](#apidoc.module.jsforce.soql_builder)

#### <a name="apidoc.element.jsforce.soql_builder.createSOQL"></a>[function <span class="apidocSignatureSpan">jsforce.soql_builder.</span>createSOQL (query)](#apidoc.element.jsforce.soql_builder.createSOQL)
- description and source-code
```javascript
function createSOQL(query) {
  var soql = [
    "SELECT ",
    createFieldsClause(query.fields, query.includes),
    " FROM ",
    query.table
  ].join("");
  var cond = createConditionClause(query.conditions);
  if (cond) {
    soql += " WHERE " + cond;
  }
  var orderby = createOrderByClause(query.sort);
  if (orderby) {
    soql += " ORDER BY " + orderby;
  }
  if (query.limit) {
    soql += " LIMIT " + query.limit;
  }
  if (query.offset) {
    soql += " OFFSET " + query.offset;
  }
  return soql;
}
```
- example usage
```shell
...
*
* @param {Callback.<String>} [callback] - Callback function
* @returns {Promise.<String>}
*/
Query.prototype.toSOQL = function(callback) {
 var self = this;
 return Promise.resolve(self._soql ||
   self._expandFields().then(function() { return SOQLBuilder.createSOQL(self._config); })
 ).thenCall(callback);
};

/**
* Create data stream of queried records.
* Automatically resume query if paused.
*
...
```



# <a name="apidoc.module.jsforce.transport"></a>[module jsforce.transport](#apidoc.module.jsforce.transport)

#### <a name="apidoc.element.jsforce.transport.transport"></a>[function <span class="apidocSignatureSpan">jsforce.</span>transport ()](#apidoc.element.jsforce.transport.transport)
- description and source-code
```javascript
transport = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.transport.CanvasTransport"></a>[function <span class="apidocSignatureSpan">jsforce.transport.</span>CanvasTransport (signedRequest)](#apidoc.element.jsforce.transport.CanvasTransport)
- description and source-code
```javascript
CanvasTransport = function (signedRequest) {
  this._signedRequest = signedRequest;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.transport.JsonpTransport"></a>[function <span class="apidocSignatureSpan">jsforce.transport.</span>JsonpTransport (jsonpParam)](#apidoc.element.jsforce.transport.JsonpTransport)
- description and source-code
```javascript
JsonpTransport = function (jsonpParam) {
  this._jsonpParam = jsonpParam;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jsforce.transport.ProxyTransport"></a>[function <span class="apidocSignatureSpan">jsforce.transport.</span>ProxyTransport (proxyUrl)](#apidoc.element.jsforce.transport.ProxyTransport)
- description and source-code
```javascript
ProxyTransport = function (proxyUrl) {
  this._proxyUrl = proxyUrl;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jsforce.transport.prototype"></a>[module jsforce.transport.prototype](#apidoc.module.jsforce.transport.prototype)

#### <a name="apidoc.element.jsforce.transport.prototype._getHttpRequestModule"></a>[function <span class="apidocSignatureSpan">jsforce.transport.prototype.</span>_getHttpRequestModule ()](#apidoc.element.jsforce.transport.prototype._getHttpRequestModule)
- description and source-code
```javascript
_getHttpRequestModule = function () {
  return request;
}
```
- example usage
```shell
...
 * @param {Object} params - HTTP request
 * @param {Callback.<Object>} [callback] - Calback Function
 * @returns {Promise.<Object>}
 */
Transport.prototype.httpRequest = function(params, callback) {
var deferred = Promise.defer();
var req;
var httpRequest = this._getHttpRequestModule();
var createRequest = function() {
  if (!req) {
    req = httpRequest(params, function(err, response) {
      if (err) {
        deferred.reject(err);
      } else {
        deferred.resolve(response);
...
```

#### <a name="apidoc.element.jsforce.transport.prototype.httpRequest"></a>[function <span class="apidocSignatureSpan">jsforce.transport.prototype.</span>httpRequest (params, callback)](#apidoc.element.jsforce.transport.prototype.httpRequest)
- description and source-code
```javascript
httpRequest = function (params, callback) {
  var deferred = Promise.defer();
  var req;
  var httpRequest = this._getHttpRequestModule();
  var createRequest = function() {
    if (!req) {
      req = httpRequest(params, function(err, response) {
        if (err) {
          deferred.reject(err);
        } else {
          deferred.resolve(response);
        }
      });
    }
    return req;
  };
  return streamify(deferred.promise, createRequest).thenCall(callback);
}
```
- example usage
```shell
...
  // hook before sending
  self.beforeSend(request);

  self.emit('request', request);
  logger.debug("<request> method=" + request.method + ", url=" + request.url);
  var requestTime = Date.now();

  return this._transport.httpRequest(request).then(function(response) {
var responseTime = Date.now();
logger.debug("elappsed time : " + (responseTime - requestTime) + "msec");
logger.debug("<response> status=" + response.statusCode + ", url=" + request.url);

self.emit('response', response);
// Refresh token if session has been expired and requires authentication
// when session refresh delegate is available
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
