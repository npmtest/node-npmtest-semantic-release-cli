# test coverage for  [semantic-release-cli (v3.0.3)](https://github.com/semantic-release/cli)  [![npm package](https://img.shields.io/npm/v/npmtest-semantic-release-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-semantic-release-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-semantic-release-cli.svg)](https://travis-ci.org/npmtest/node-npmtest-semantic-release-cli)
#### setup automated semver compliant package publishing

[![NPM](https://nodei.co/npm/semantic-release-cli.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/semantic-release-cli)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-semantic-release-cli/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-semantic-release-cli/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-semantic-release-cli/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-semantic-release-cli/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-semantic-release-cli/build/test-report.html](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-semantic-release-cli/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-semantic-release-cli/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-semantic-release-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-semantic-release-cli/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-semantic-release-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christoph Witzko",
        "url": "http://christophwitzko.com"
    },
    "babel": {
        "presets": [
            "es2015-node4"
        ],
        "plugins": [
            "transform-async-to-generator"
        ]
    },
    "bin": {
        "semantic-release-cli": "./bin/semantic-release.js"
    },
    "bugs": {
        "url": "https://github.com/semantic-release/cli/issues"
    },
    "dependencies": {
        "base32": "0.0.6",
        "bluebird": "^3.4.6",
        "github-url-from-git": "^1.4.0",
        "ini": "^1.3.4",
        "inquirer": "^1.2.2",
        "js-yaml": "^3.3.1",
        "keytar": "^3.0.0",
        "lodash": "^4.16.4",
        "nopt": "^4.0.0",
        "npm": "^4.0.3",
        "npm-registry-client": "^7.3.0",
        "npmlog": "^4.0.0",
        "parse-github-repo-url": "^1.0.0",
        "request": "^2.58.0",
        "request-promise": "^4.1.1",
        "travis-ci": "^2.1.1",
        "update-notifier": "^1.0.2",
        "user-home": "^2.0.0",
        "validator": "^6.1.0"
    },
    "description": "setup automated semver compliant package publishing",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-plugin-transform-async-to-generator": "^6.16.0",
        "babel-preset-es2015-node4": "^2.1.0",
        "mkdirp": "^0.5.1",
        "nyc": "^10.0.0",
        "rimraf": "^2.4.2",
        "semantic-release": "^6.3.2",
        "standard": "^8.5.0",
        "tap": "^9.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a120f41a8c3710a9364aac19172e4b26ebea4533",
        "tarball": "https://registry.npmjs.org/semantic-release-cli/-/semantic-release-cli-3.0.3.tgz"
    },
    "engines": {
        "node": ">=4",
        "npm": ">=3"
    },
    "gitHead": "1638a48abe19bae669c5b60a0fabb45836fe2dcc",
    "homepage": "https://github.com/semantic-release/cli",
    "keywords": [
        "author",
        "automation",
        "changelog",
        "module",
        "package",
        "publish",
        "release",
        "semver",
        "version"
    ],
    "license": "MIT",
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "semantic-release-bot"
        }
    ],
    "name": "semantic-release-cli",
    "optionalDependencies": {
        "keytar": "^3.0.0"
    },
    "preferGlobal": true,
    "readmeFilename": "README.md",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/semantic-release/cli.git"
    },
    "scripts": {
        "build": "rimraf dist && mkdirp dist && babel src --out-dir dist",
        "coverage": "nyc report",
        "coverage:upload": "npm run coverage -- --reporter=lcovonly && coveralls < coverage/lcov.info",
        "prepublish": "npm run build",
        "semantic-release": "semantic-release pre && npm publish && semantic-release post",
        "test": "npm run test:style && npm run test:unit",
        "test:style": "standard",
        "test:unit": "nyc tap --no-cov test/specs/*.js"
    },
    "version": "3.0.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
