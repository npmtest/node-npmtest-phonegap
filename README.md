# npmtest-phonegap

#### basic test coverage for  [phonegap (v6.5.0)](http://github.com/phonegap/phonegap-cli)  [![npm package](https://img.shields.io/npm/v/npmtest-phonegap.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-phonegap) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-phonegap.svg)](https://travis-ci.org/npmtest/node-npmtest-phonegap)

#### PhoneGap command-line interface and node.js library.

[![NPM](https://nodei.co/npm/phonegap.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/phonegap)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-phonegap/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-phonegap/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-phonegap/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-phonegap/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-phonegap/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-phonegap/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-phonegap/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-phonegap/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-phonegap/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-phonegap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-phonegap/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-phonegap/build/test-report.html](https://npmtest.github.io/node-npmtest-phonegap/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-phonegap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-phonegap/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-phonegap/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-phonegap/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-phonegap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-phonegap/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-phonegap/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-phonegap/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "phonegap",
    "description": "PhoneGap command-line interface and node.js library.",
    "version": "6.5.0",
    "license": "Apache-2.0",
    "homepage": "http://github.com/phonegap/phonegap-cli",
    "repository": {
        "type": "git",
        "url": "git://github.com/phonegap/phonegap-cli.git"
    },
    "keywords": [
        "cli",
        "cordova",
        "phonegap",
        "phonegap build",
        "phonegap/build"
    ],
    "preferGlobal": true,
    "main": "./lib/main.js",
    "bin": {
        "phonegap": "./bin/phonegap.js"
    },
    "scripts": {
        "test": "node node_modules/jasmine-node/bin/jasmine-node --color spec; node_modules/eslint/bin/eslint.js ./ --ignore-path .gitignore",
        "cover": "istanbul cover --print detail -x **/spec/** node_modules/jasmine-node/bin/jasmine-node -- --color spec"
    },
    "engineStrict": true,
    "engines": {
        "node": ">=4.0.0"
    },
    "dependencies": {
        "archiver": "^1.0.0",
        "colors": "0.6.0-1",
        "connect-phonegap": "0.24.5",
        "cordova": "6.5.0",
        "insight": "0.8.2",
        "configstore": "1.4.0",
        "os-name": "2.0.1",
        "minimist": "0.1.0",
        "opener": "1.4.1",
        "opn": "^4.0.2",
        "phonegap-build": "0.10.0",
        "pluralize": "0.0.4",
        "prompt": "0.2.11",
        "qrcode-terminal": "0.9.4",
        "request": "2.81.0",
        "semver": "1.1.0",
        "shelljs": "0.1.4",
        "update-notifier": "^0.6.0"
    },
    "devDependencies": {
        "chdir": "0.0.x",
        "eslint": "^3.12.2",
        "jasmine-node": "1.14.5",
        "istanbul": "0.4.5"
    },
    "optionalDependencies": {},
    "contributors": [
        {
            "name": "Michael Brooks",
            "url": "http://michaelbrooks.ca/"
        },
        {
            "name": "Lorin Beer",
            "url": "http://www.ensufire.com/"
        },
        {
            "name": "Jesse MacFadyen",
            "url": "http://risingj.com"
        },
        {
            "name": "Ryan Stewart"
        },
        {
            "name": "Herm Wong"
        },
        {
            "name": "Suraj Pindoria"
        },
        {
            "name": "Tommy-Carlos Williams"
        }
    ],
    "templates": {
        "blank": {
            "description": "A blank and empty PhoneGap app.",
            "npm": "phonegap-template-blank"
        },
        "csdk-image-editor": {
            "description": "A template for using the Creative Cloud Image Editor.",
            "npm": "phonegap-template-csdk-image-editor"
        },
        "hello-world": {
            "description": "Default hello world app for PhoneGap.",
            "npm": "phonegap-template-hello-world"
        },
        "framework7": {
            "description": "Starter PhoneGap project for Framework7.",
            "npm": "phonegap-template-framework7"
        },
        "push": {
            "description": "An example app for getting started with push notifications",
            "npm": "phonegap-template-push"
        },
        "react-hot-loader": {
            "description": "Starter PhoneGap project using React.js, Babel, Webpack and Hot Reloading.",
            "npm": "phonegap-template-react-hot-loader"
        },
        "star-track": {
            "description": "An example app using Framework7 and the Spotify API.",
            "npm": "phonegap-app-star-track"
        },
        "webvr": {
            "description": "A WebVR and Google Cardboard demo ported from borismus/webvr-boilerplate.",
            "npm": "phonegap-template-webvr"
        },
        "wikitude-augmented-reality": {
            "description": "Augmented Reality demo app powered by the Wikitude plugin",
            "npm": "phonegap-app-augmented-reality"
        }
    },
    "gitHead": "26e04aca43a9b2ebccc80d4591afd4d7509dd810",
    "bugs": {
        "url": "https://github.com/phonegap/phonegap-cli/issues"
    },
    "dist": {
        "shasum": "8a101db223f7c13f80bd0d30873674b39f2f7a0c",
        "tarball": "https://registry.npmjs.org/phonegap/-/phonegap-6.5.0.tgz"
    },
    "maintainers": [
        {
            "name": "devgeeks"
        },
        {
            "name": "filmaj"
        },
        {
            "name": "hermwong"
        },
        {
            "name": "macdonst"
        },
        {
            "name": "mwbrooks"
        },
        {
            "name": "stevegill"
        },
        {
            "name": "surajpindoria"
        },
        {
            "name": "timkim"
        }
    ],
    "directories": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
