# npmdoc-sqlite3

#### basic api documentation for  [sqlite3 (4.0.0)](http://github.com/mapbox/node-sqlite3)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sqlite3.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sqlite3)

#### Asynchronous, non-blocking SQLite3 bindings

[![NPM](https://nodei.co/npm/sqlite3.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/sqlite3)

- [https://npmdoc.github.io/node-npmdoc-sqlite3/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-sqlite3/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sqlite3/build/screenshot.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sqlite3/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sqlite3/build/screenshot.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sqlite3/build/screenshot.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "MapBox",
        "url": "https://mapbox.com/"
    },
    "binary": {
        "module_name": "node_sqlite3",
        "module_path": "./lib/binding/{node_abi}-{platform}-{arch}",
        "host": "https://mapbox-node-binary.s3.amazonaws.com",
        "remote_path": "./{name}/v{version}/{toolset}/",
        "package_name": "{node_abi}-{platform}-{arch}.tar.gz"
    },
    "bugs": {
        "url": "https://github.com/mapbox/node-sqlite3/issues"
    },
    "bundleDependencies": [
        "node-pre-gyp"
    ],
    "contributors": [
        {
            "name": "Konstantin Käfer"
        },
        {
            "name": "Dane Springmeyer"
        },
        {
            "name": "Will White"
        },
        {
            "name": "Orlando Vazquez"
        },
        {
            "name": "Artem Kustikov"
        },
        {
            "name": "Eric Fredricksen"
        },
        {
            "name": "John Wright"
        },
        {
            "name": "Ryan Dahl"
        },
        {
            "name": "Tom MacWright"
        },
        {
            "name": "Carter Thaxton"
        },
        {
            "name": "Audrius Kažukauskas"
        },
        {
            "name": "Johannes Schauer"
        },
        {
            "name": "Nathan Rajlich"
        },
        {
            "name": "AJ ONeal"
        },
        {
            "name": "Mithgol"
        },
        {
            "name": "Ben Noordhuis"
        }
    ],
    "dependencies": {
        "nan": "~2.9.2",
        "node-pre-gyp": "~0.9.0"
    },
    "description": "Asynchronous, non-blocking SQLite3 bindings",
    "devDependencies": {
        "aws-sdk": "2.x",
        "eslint": "3.5.0",
        "mocha": "3.x"
    },
    "directories": {},
    "dist": {
        "integrity": "sha512-6OlcAQNGaRSBLK1CuaRbKwlMFBb9DEhzmZyQP+fltNRF6XcIMpVIfXCBEcXPe1d4v9LnhkQUYkknDbA5JReqJg==",
        "shasum": "cc0e093ab51873f50d9dfc4126fcbef15d486570",
        "tarball": "https://registry.npmjs.org/sqlite3/-/sqlite3-4.0.0.tgz",
        "fileCount": 563,
        "unpackedSize": 4502461
    },
    "gitHead": "d02f5c3b496aab1e10ba1f981b0a7f7a276894e7",
    "homepage": "http://github.com/mapbox/node-sqlite3",
    "keywords": [
        "sql",
        "sqlite",
        "sqlite3",
        "database"
    ],
    "license": "BSD-3-Clause",
    "main": "./lib/sqlite3",
    "maintainers": [
        {
            "name": "kkaefer"
        },
        {
            "name": "springmeyer"
        },
        {
            "name": "tmcw"
        },
        {
            "name": "yhahn"
        }
    ],
    "name": "sqlite3",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/mapbox/node-sqlite3.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build",
        "prepublishOnly": "npm ls",
        "pretest": "node test/support/createdb.js",
        "test": "mocha -R spec --timeout 480000"
    },
    "version": "4.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
