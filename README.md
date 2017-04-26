# npmdoc-browser-perf

#### basic api documentation for  [browser-perf (v1.4.11)](https://github.com/axemclion/browser-perf#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-browser-perf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-browser-perf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-browser-perf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-browser-perf)

#### Measure browser rendering performance metrics

[![NPM](https://nodei.co/npm/browser-perf.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/browser-perf)

- [https://npmdoc.github.io/node-npmdoc-browser-perf/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-browser-perf/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-browser-perf/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-browser-perf/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-browser-perf/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-browser-perf/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Parashuram"
    },
    "bin": {
        "browser-perf": "lib/cli.js"
    },
    "bugs": {
        "url": "https://github.com/axemclion/browser-perf/issues"
    },
    "dependencies": {
        "JSONStream": "^1.0.6",
        "byline": "^4.2.1",
        "cli-table": "~0.3.1",
        "commander": "^2.9.0",
        "debug": "^2.2.0",
        "event-stream": "^3.3.2",
        "glob": "^6.0.2",
        "jsmin": "~1.0.1",
        "q": "^1.4.1",
        "request": "^2.65.0",
        "wd": "^0.4.0"
    },
    "description": "Measure browser rendering performance metrics",
    "devDependencies": {
        "chai": "~3.4.0",
        "chai-as-promised": "^5.1.0",
        "mocha": "^2.3.3",
        "sinon": "^1.17.2"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "3d73394331438aa0dbf3455a98ab2306a035b2aa",
        "tarball": "https://registry.npmjs.org/browser-perf/-/browser-perf-1.4.11.tgz"
    },
    "gitHead": "db8aecd284725cb99c9e868c2d9bcde53f9b445a",
    "homepage": "https://github.com/axemclion/browser-perf#readme",
    "keywords": [
        "browser-perf",
        "rendering",
        "telemetry",
        "chromium",
        "performance",
        "high performance web sites",
        "metrics",
        "monitoring",
        "web development",
        "webperf"
    ],
    "license": "BSD-2-Clause",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "axemclion"
        }
    ],
    "name": "browser-perf",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/axemclion/browser-perf.git"
    },
    "scripts": {
        "test": "mocha --recursive --require=./test/test.helper.js ./test"
    },
    "version": "1.4.11"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
