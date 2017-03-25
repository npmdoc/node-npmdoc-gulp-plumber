# api documentation for  [gulp-plumber (v1.1.0)](https://github.com/floatdrop/gulp-plumber)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-plumber.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-plumber)
#### Prevent pipe breaking caused by errors from gulp plugins

[![NPM](https://nodei.co/npm/gulp-plumber.png?downloads=true)](https://www.npmjs.com/package/gulp-plumber)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-plumber/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp_plumber_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-plumber/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-gulp-plumber/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Vsevolod Strukchinsky",
        "email": "floatdrop@gmail.com",
        "url": "https://github.com/floatdrop"
    },
    "bugs": {
        "url": "https://github.com/floatdrop/gulp-plumber/issues"
    },
    "dependencies": {
        "gulp-util": "^3",
        "through2": "^2"
    },
    "description": "Prevent pipe breaking caused by errors from gulp plugins",
    "devDependencies": {
        "coveralls": "^2.11.6",
        "event-stream": "^3.3.2",
        "gulp": "^3.9.1",
        "istanbul": "^0.4.2",
        "mocha": "^2.4.5",
        "mocha-lcov-reporter": "^1.0.0",
        "should": "^8.2.2",
        "through": "^2.3.8",
        "xo": "^0.12.1"
    },
    "directories": {},
    "dist": {
        "shasum": "f12176c2d0422f60306c242fff6a01a394faba09",
        "tarball": "https://registry.npmjs.org/gulp-plumber/-/gulp-plumber-1.1.0.tgz"
    },
    "engines": {
        "node": ">=0.10",
        "npm": ">=1.2.10"
    },
    "gitHead": "982ec116283b5b5907448ac932a96be31c7d872f",
    "homepage": "https://github.com/floatdrop/gulp-plumber",
    "keywords": [
        "gulpplugin"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "floatdrop",
            "email": "floatdrop@gmail.com"
        }
    ],
    "name": "gulp-plumber",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/floatdrop/gulp-plumber.git"
    },
    "scripts": {
        "test": "xo && mocha -R spec"
    },
    "version": "1.1.0",
    "xo": {
        "ignore": [
            "test/**"
        ]
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-plumber](#apidoc.module.gulp-plumber)
1.  [function <span class="apidocSignatureSpan">gulp-plumber.</span>stop ()](#apidoc.element.gulp-plumber.stop)



# <a name="apidoc.module.gulp-plumber"></a>[module gulp-plumber](#apidoc.module.gulp-plumber)

#### <a name="apidoc.element.gulp-plumber.stop"></a>[function <span class="apidocSignatureSpan">gulp-plumber.</span>stop ()](#apidoc.element.gulp-plumber.stop)
- description and source-code
```javascript
stop = function () {
	var through = through2.obj();
	through._unplumbed = true;
	return through;
}
```
- example usage
```shell
...
Default: 'true'

Handle errors in underlying streams and output them to console.
 * 'function' passed - it will be attached to stream 'on('error')'.
 * 'false' passed - error handler will not be attached.
 * 'undefined' - default error handler will be attached.

### plumber.stop()

This method will return default behaviour for pipeline after it was piped.

'''javascript
var plumber = require('gulp-plumber');

gulp.src('./src/*.scss')
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
