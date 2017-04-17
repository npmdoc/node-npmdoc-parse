# api documentation for  [parse (v1.9.2)](https://www.parse.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-parse.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-parse) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-parse.svg)](https://travis-ci.org/npmdoc/node-npmdoc-parse)
#### The Parse JavaScript SDK

[![NPM](https://nodei.co/npm/parse.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/parse)

- [https://npmdoc.github.io/node-npmdoc-parse/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-parse/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-parse/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-parse/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-parse/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-parse/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "browser": {
        "react-native": false
    },
    "bugs": {
        "url": "https://github.com/ParsePlatform/Parse-SDK-JS/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.11.6",
        "ws": "^1.0.1",
        "xmlhttprequest": "^1.7.0"
    },
    "description": "The Parse JavaScript SDK",
    "devDependencies": {
        "babel-jest": "^15.0.0",
        "babel-plugin-flow-comments": "^1.0.9",
        "babel-plugin-inline-package-json": "~2.0.0",
        "babel-plugin-minify-dead-code-elimination": "0.0.2",
        "babel-plugin-transform-inline-environment-variables": "^6.8.0",
        "babel-plugin-transform-runtime": "^6.15.0",
        "babel-preset-es2015": "^6.14.0",
        "babel-preset-react": "^6.11.1",
        "babel-preset-stage-2": "^6.13.0",
        "browserify": "^11.0.1",
        "codecov.io": "^0.1.6",
        "gulp": "^3.9.0",
        "gulp-babel": "^6.1.2",
        "gulp-derequire": "^2.1.0",
        "gulp-insert": "^0.5.0",
        "gulp-rename": "^1.2.2",
        "gulp-replace": "^0.5.4",
        "gulp-uglify": "^1.4.0",
        "jasmine-reporters": "~1.0.0",
        "jest-cli": "^15.1.1",
        "vinyl-source-stream": "^1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "e41d7cb6efd464eea30c34ec0651548f66c5b8e4",
        "tarball": "https://registry.npmjs.org/parse/-/parse-1.9.2.tgz"
    },
    "files": [
        "index.js",
        "node.js",
        "react-native.js",
        "dist/",
        "lib/",
        "LICENSE",
        "PATENTS",
        "README.md"
    ],
    "gitHead": "b01f2df856121dd557bc7e936e4ca32a4682b269",
    "homepage": "https://www.parse.com",
    "jest": {
        "automock": true,
        "collectCoverage": true,
        "testPathDirs": [
            "src/"
        ],
        "testPathIgnorePatterns": [
            "/node_modules/",
            "/test_helpers/"
        ],
        "scriptPreprocessor": "babel-jest.js",
        "setupTestFrameworkScriptFile": "setup-jest.js"
    },
    "keywords": [
        "cloud",
        "mobile",
        "api"
    ],
    "license": "BSD-3-Clause",
    "maintainers": [
        {
            "name": "andrewimm"
        },
        {
            "name": "grantland"
        },
        {
            "name": "lacker"
        },
        {
            "name": "nlutsenko"
        },
        {
            "name": "peterdotjs"
        },
        {
            "name": "wangmengyan95"
        }
    ],
    "name": "parse",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ParsePlatform/Parse-SDK-JS.git"
    },
    "scripts": {
        "build": "./build_releases.sh",
        "release": "./build_releases.sh && npm publish",
        "test": "PARSE_BUILD=node jest"
    },
    "version": "1.9.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
