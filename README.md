# npmtest-ios-deploy

#### basic test coverage for  ios-deploy (v1.9.1)  [![npm package](https://img.shields.io/npm/v/npmtest-ios-deploy.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-ios-deploy) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-ios-deploy.svg)](https://travis-ci.org/npmtest/node-npmtest-ios-deploy)

#### launch iOS apps iOS devices from the command line (Xcode 7)

[![NPM](https://nodei.co/npm/ios-deploy.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ios-deploy)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-ios-deploy/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-ios-deploy/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-ios-deploy/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-ios-deploy/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-ios-deploy/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-ios-deploy/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-ios-deploy/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-ios-deploy/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-ios-deploy/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-ios-deploy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-ios-deploy/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-ios-deploy/build/test-report.html](https://npmtest.github.io/node-npmtest-ios-deploy/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-ios-deploy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-ios-deploy/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-ios-deploy/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ios-deploy/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ios-deploy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ios-deploy/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-ios-deploy/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-ios-deploy/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "ios-deploy",
    "version": "1.9.1",
    "os": [
        "darwin"
    ],
    "description": "launch iOS apps iOS devices from the command line (Xcode 7)",
    "main": "ios-deploy",
    "scripts": {
        "preinstall": "./src/scripts/check_reqs.js && xcodebuild",
        "test": "npm run pycompile && npm run jshint && xcodebuild -target ios-deploy-lib && xcodebuild test -scheme ios-deploy-tests",
        "jshint": "node node_modules/jshint/bin/jshint src/scripts/*.js",
        "pycompile": "python -m py_compile src/scripts/*.py"
    },
    "bin": "./build/Release/ios-deploy",
    "repository": {
        "type": "git",
        "url": "https://github.com/phonegap/ios-deploy"
    },
    "devDependencies": {
        "jshint": "2.5.8"
    },
    "keywords": [
        "ios-deploy",
        "deploy to iOS device"
    ],
    "bugs": {
        "url": "https://github.com/phonegap/ios-deploy/issues"
    },
    "author": "Greg Hughes",
    "license": "GPLv3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
