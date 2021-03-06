# npmdoc-aqb

#### basic api documentation for  [aqb (v2.1.0)](https://github.com/arangodb/aqbjs)  [![npm package](https://img.shields.io/npm/v/npmdoc-aqb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-aqb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-aqb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-aqb)

#### ArangoDB AQL query builder.

[![NPM](https://nodei.co/npm/aqb.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/aqb)

- [https://npmdoc.github.io/node-npmdoc-aqb/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-aqb/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-aqb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-aqb/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-aqb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-aqb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Alan Plum"
    },
    "bugs": {
        "url": "https://github.com/arangodb/aqbjs/issues"
    },
    "dependencies": {},
    "description": "ArangoDB AQL query builder.",
    "devDependencies": {
        "browserify": "^7.0.2",
        "coveralls": "^2.11.2",
        "dekeywordify": "^0.2.1",
        "eslint": "^1.3.1",
        "expect.js": "^0.3.1",
        "istanbul": "^0.3.5",
        "mocha": "^2.1.0",
        "uglify-js": "^2.4.15"
    },
    "directories": {},
    "dist": {
        "shasum": "cc3de1656fbc7e43e8c06ade4d40262b069fafbd",
        "tarball": "https://registry.npmjs.org/aqb/-/aqb-2.1.0.tgz"
    },
    "files": [
        "*.js",
        "package.json",
        "README.md",
        "LICENSE"
    ],
    "gitHead": "2bd6cb05200c15c25769b496f2de126bee83e5c9",
    "homepage": "https://github.com/arangodb/aqbjs",
    "keywords": [
        "arangodb",
        "aql",
        "nosql",
        "query"
    ],
    "license": "APACHE-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "pluma"
        },
        {
            "name": "jsteemann"
        }
    ],
    "name": "aqb",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/arangodb/aqbjs.git"
    },
    "scripts": {
        "bundle": "browserify -t dekeywordify -u console -s aqb ./index.js > dist/aqb.js",
        "cover": "npm run lint && istanbul cover --report lcov _mocha -- -t 30000 -R spec",
        "coveralls": "npm run cover && cat ./coverage/lcov.info | coveralls ; rm -rf ./coverage",
        "dist": "npm run bundle && npm run minify",
        "lint": "eslint index.js *.js test",
        "minify": "uglifyjs dist/aqb.js > dist/aqb.min.js",
        "prepublish": "npm run lint",
        "test": "npm run lint && npm run test-only",
        "test-only": "mocha -t 30000 --growl -R spec test test/**"
    },
    "version": "2.1.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
