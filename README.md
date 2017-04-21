# npmtest-deepcopy

#### basic test coverage for  deepcopy (v0.6.3)  [![npm package](https://img.shields.io/npm/v/npmtest-deepcopy.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-deepcopy) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-deepcopy.svg)](https://travis-ci.org/npmtest/node-npmtest-deepcopy)

#### deep copy for any data

[![NPM](https://nodei.co/npm/deepcopy.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/deepcopy)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-deepcopy/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-deepcopy/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-deepcopy/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-deepcopy/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-deepcopy/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-deepcopy/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-deepcopy/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-deepcopy/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-deepcopy/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-deepcopy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-deepcopy/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-deepcopy/build/test-report.html](https://npmtest.github.io/node-npmtest-deepcopy/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-deepcopy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-deepcopy/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-deepcopy/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-deepcopy/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-deepcopy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-deepcopy/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-deepcopy/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-deepcopy/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "deepcopy",
    "version": "0.6.3",
    "author": "sasa+1 <sasaplus1@gmail.com>",
    "contributors": [
        "kjirou <kjirou.web@gmail.com>"
    ],
    "description": "deep copy for any data",
    "main": "./index.js",
    "license": "MIT",
    "readmeFilename": "README.md",
    "repository": {
        "type": "git",
        "url": "git://github.com/sasaplus1/deepcopy.js.git"
    },
    "scripts": {
        "babel": "babel --out-dir ./lib ./src",
        "build": "npm run clean && npm run babel && npm run compile && npm run minify",
        "clean": "npm run rimraf -- ./build ./lib",
        "compile": "npm run webpack -- --output-filename ./build/deepcopy.js",
        "develop": " parallelshell 'npm run babel -- -w' 'npm run compile -- -w' 'npm run minify -- -w'",
        "eslint": "eslint",
        "karma": "karma",
        "lint": "npm run eslint -- --ext .js .",
        "minify": "npm run webpack -- --optimize-minimize --output-filename ./build/deepcopy.min.js",
        "mocha": "mocha",
        "posttest": "npm run karma -- start --single-run --browsers Chrome,Firefox,Safari",
        "prepublish": "npm run build",
        "rimraf": "rimraf",
        "test": "npm run mocha",
        "travis": "npm run mocha",
        "webpack": "webpack --colors --display-error-details --progress"
    },
    "devDependencies": {
        "babel": "^6.5.2",
        "babel-cli": "^6.6.5",
        "babel-core": "^6.7.2",
        "babel-eslint": "^6.0.4",
        "babel-loader": "^6.2.4",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-check-es2015-constants": "^6.7.2",
        "babel-plugin-espower": "^2.1.2",
        "babel-plugin-transform-es2015-arrow-functions": "^6.5.2",
        "babel-plugin-transform-es2015-block-scoping": "^6.7.1",
        "babel-plugin-transform-es2015-computed-properties": "^6.6.5",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.7.0",
        "babel-plugin-transform-es2015-parameters": "^6.7.0",
        "babel-plugin-transform-es2015-template-literals": "^6.6.5",
        "babel-plugin-transform-es3-member-expression-literals": "^6.5.0",
        "babel-plugin-transform-es3-property-literals": "^6.5.0",
        "babel-plugin-transform-strict-mode": "^6.6.5",
        "babel-plugin-transform-undefined-to-void": "^6.5.0",
        "coffee-script": "^1.10.0",
        "eslint": "^2.4.0",
        "eslint-config-sasaplus1": "sasaplus1-prototype/eslint-config-sasaplus1.git",
        "espower-babel": "4.0.3",
        "karma": "^0.13.15",
        "karma-chrome-launcher": "^1.0.1",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.0.1",
        "karma-safari-launcher": "^1.0.0",
        "karma-webpack": "^1.7.0",
        "mocha": "^2.3.4",
        "parallelshell": "^2.0.0",
        "power-assert": "^1.3.1",
        "rimraf": "^2.4.4",
        "webpack": "^1.12.9"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
