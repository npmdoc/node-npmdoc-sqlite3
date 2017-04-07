# api documentation for  [sqlite3 (v3.1.8)](http://github.com/mapbox/node-sqlite3)  [![npm package](https://img.shields.io/npm/v/npmdoc-sqlite3.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-sqlite3) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-sqlite3.svg)](https://travis-ci.org/npmdoc/node-npmdoc-sqlite3)
#### Asynchronous, non-blocking SQLite3 bindings

[![NPM](https://nodei.co/npm/sqlite3.png?downloads=true)](https://www.npmjs.com/package/sqlite3)

[![apidoc](https://npmdoc.github.io/node-npmdoc-sqlite3/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-sqlite3_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-sqlite3/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-sqlite3/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-sqlite3/build/screenCapture.npmPackageDependencyTree.svg)



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
            "name": "Konstantin Käfer",
            "email": "mail@kkaefer.com"
        },
        {
            "name": "Dane Springmeyer",
            "email": "dane@mapbox.com"
        },
        {
            "name": "Will White",
            "email": "will@mapbox.com"
        },
        {
            "name": "Orlando Vazquez",
            "email": "ovazquez@gmail.com"
        },
        {
            "name": "Artem Kustikov",
            "email": "kustikoff@gmail.com"
        },
        {
            "name": "Eric Fredricksen",
            "email": "efredricksen@gmail.com"
        },
        {
            "name": "John Wright",
            "email": "mrjjwright@gmail.com"
        },
        {
            "name": "Ryan Dahl",
            "email": "ry@tinyclouds.org"
        },
        {
            "name": "Tom MacWright",
            "email": "tom@mapbox.com"
        },
        {
            "name": "Carter Thaxton",
            "email": "carter.thaxton@gmail.com"
        },
        {
            "name": "Audrius Kažukauskas",
            "email": "audrius@neutrino.lt"
        },
        {
            "name": "Johannes Schauer",
            "email": "josch@pyneo.org"
        },
        {
            "name": "Nathan Rajlich",
            "email": "nathan@tootallnate.net"
        },
        {
            "name": "AJ ONeal",
            "email": "coolaj86@gmail.com"
        },
        {
            "name": "Mithgol"
        },
        {
            "name": "Ben Noordhuis",
            "email": "ben@strongloop.com"
        }
    ],
    "dependencies": {
        "nan": "~2.4.0",
        "node-pre-gyp": "~0.6.31"
    },
    "description": "Asynchronous, non-blocking SQLite3 bindings",
    "devDependencies": {
        "aws-sdk": "2.x",
        "eslint": "3.5.0",
        "mocha": "3.x"
    },
    "directories": {},
    "dist": {
        "shasum": "4cbcf965d8b901d1b1015cbc7fc415aae157dfaa",
        "tarball": "https://registry.npmjs.org/sqlite3/-/sqlite3-3.1.8.tgz"
    },
    "gitHead": "4800c6377ef15f467290d77776302b486e71ada3",
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
            "name": "kkaefer",
            "email": "kkaefer@gmail.com"
        },
        {
            "name": "yhahn",
            "email": "young@developmentseed.org"
        },
        {
            "name": "tmcw",
            "email": "macwright@gmail.com"
        },
        {
            "name": "springmeyer",
            "email": "dane@dbsgeo.com"
        }
    ],
    "name": "sqlite3",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mapbox/node-sqlite3.git"
    },
    "scripts": {
        "install": "node-pre-gyp install --fallback-to-build",
        "prepublish": "npm ls",
        "pretest": "node test/support/createdb.js",
        "test": "mocha -R spec --timeout 480000"
    },
    "version": "3.1.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module sqlite3](#apidoc.module.sqlite3)
1.  [function <span class="apidocSignatureSpan">sqlite3.</span>Database ()](#apidoc.element.sqlite3.Database)
1.  [function <span class="apidocSignatureSpan">sqlite3.</span>Statement ()](#apidoc.element.sqlite3.Statement)
1.  [function <span class="apidocSignatureSpan">sqlite3.</span>verbose ()](#apidoc.element.sqlite3.verbose)
1.  number <span class="apidocSignatureSpan">sqlite3.</span>ABORT
1.  number <span class="apidocSignatureSpan">sqlite3.</span>AUTH
1.  number <span class="apidocSignatureSpan">sqlite3.</span>BUSY
1.  number <span class="apidocSignatureSpan">sqlite3.</span>CANTOPEN
1.  number <span class="apidocSignatureSpan">sqlite3.</span>CONSTRAINT
1.  number <span class="apidocSignatureSpan">sqlite3.</span>CORRUPT
1.  number <span class="apidocSignatureSpan">sqlite3.</span>EMPTY
1.  number <span class="apidocSignatureSpan">sqlite3.</span>ERROR
1.  number <span class="apidocSignatureSpan">sqlite3.</span>FORMAT
1.  number <span class="apidocSignatureSpan">sqlite3.</span>FULL
1.  number <span class="apidocSignatureSpan">sqlite3.</span>INTERNAL
1.  number <span class="apidocSignatureSpan">sqlite3.</span>INTERRUPT
1.  number <span class="apidocSignatureSpan">sqlite3.</span>IOERR
1.  number <span class="apidocSignatureSpan">sqlite3.</span>LOCKED
1.  number <span class="apidocSignatureSpan">sqlite3.</span>MISMATCH
1.  number <span class="apidocSignatureSpan">sqlite3.</span>MISUSE
1.  number <span class="apidocSignatureSpan">sqlite3.</span>NOLFS
1.  number <span class="apidocSignatureSpan">sqlite3.</span>NOMEM
1.  number <span class="apidocSignatureSpan">sqlite3.</span>NOTADB
1.  number <span class="apidocSignatureSpan">sqlite3.</span>NOTFOUND
1.  number <span class="apidocSignatureSpan">sqlite3.</span>OK
1.  number <span class="apidocSignatureSpan">sqlite3.</span>OPEN_CREATE
1.  number <span class="apidocSignatureSpan">sqlite3.</span>OPEN_READONLY
1.  number <span class="apidocSignatureSpan">sqlite3.</span>OPEN_READWRITE
1.  number <span class="apidocSignatureSpan">sqlite3.</span>PERM
1.  number <span class="apidocSignatureSpan">sqlite3.</span>PROTOCOL
1.  number <span class="apidocSignatureSpan">sqlite3.</span>RANGE
1.  number <span class="apidocSignatureSpan">sqlite3.</span>READONLY
1.  number <span class="apidocSignatureSpan">sqlite3.</span>SCHEMA
1.  number <span class="apidocSignatureSpan">sqlite3.</span>TOOBIG
1.  number <span class="apidocSignatureSpan">sqlite3.</span>VERSION_NUMBER
1.  object <span class="apidocSignatureSpan">sqlite3.</span>Database.prototype
1.  object <span class="apidocSignatureSpan">sqlite3.</span>Statement.prototype
1.  object <span class="apidocSignatureSpan">sqlite3.</span>cached
1.  object <span class="apidocSignatureSpan">sqlite3.</span>trace
1.  string <span class="apidocSignatureSpan">sqlite3.</span>SOURCE_ID
1.  string <span class="apidocSignatureSpan">sqlite3.</span>VERSION

#### [module sqlite3.Database](#apidoc.module.sqlite3.Database)
1.  [function <span class="apidocSignatureSpan">sqlite3.</span>Database ()](#apidoc.element.sqlite3.Database.Database)

#### [module sqlite3.Database.prototype](#apidoc.module.sqlite3.Database.prototype)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>addListener (type)](#apidoc.element.sqlite3.Database.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>all (sql)](#apidoc.element.sqlite3.Database.prototype.all)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>close ()](#apidoc.element.sqlite3.Database.prototype.close)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>configure ()](#apidoc.element.sqlite3.Database.prototype.configure)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>each (sql)](#apidoc.element.sqlite3.Database.prototype.each)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>emit (type)](#apidoc.element.sqlite3.Database.prototype.emit)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>eventNames ()](#apidoc.element.sqlite3.Database.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>exec ()](#apidoc.element.sqlite3.Database.prototype.exec)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>get (sql)](#apidoc.element.sqlite3.Database.prototype.get)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>getMaxListeners ()](#apidoc.element.sqlite3.Database.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>interrupt ()](#apidoc.element.sqlite3.Database.prototype.interrupt)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>listenerCount (type)](#apidoc.element.sqlite3.Database.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>listeners (type)](#apidoc.element.sqlite3.Database.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>loadExtension ()](#apidoc.element.sqlite3.Database.prototype.loadExtension)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>map (sql)](#apidoc.element.sqlite3.Database.prototype.map)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>on (type)](#apidoc.element.sqlite3.Database.prototype.on)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>once (type, listener)](#apidoc.element.sqlite3.Database.prototype.once)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>parallelize ()](#apidoc.element.sqlite3.Database.prototype.parallelize)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>prepare (sql)](#apidoc.element.sqlite3.Database.prototype.prepare)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>prependListener (type, listener)](#apidoc.element.sqlite3.Database.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.sqlite3.Database.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>removeAllListeners (type)](#apidoc.element.sqlite3.Database.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>removeListener (type)](#apidoc.element.sqlite3.Database.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>run (sql)](#apidoc.element.sqlite3.Database.prototype.run)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>serialize ()](#apidoc.element.sqlite3.Database.prototype.serialize)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>setMaxListeners (n)](#apidoc.element.sqlite3.Database.prototype.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>wait ()](#apidoc.element.sqlite3.Database.prototype.wait)
1.  undefined <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>domain

#### [module sqlite3.Statement](#apidoc.module.sqlite3.Statement)
1.  [function <span class="apidocSignatureSpan">sqlite3.</span>Statement ()](#apidoc.element.sqlite3.Statement.Statement)

#### [module sqlite3.Statement.prototype](#apidoc.module.sqlite3.Statement.prototype)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>addListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>all ()](#apidoc.element.sqlite3.Statement.prototype.all)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>bind ()](#apidoc.element.sqlite3.Statement.prototype.bind)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>each ()](#apidoc.element.sqlite3.Statement.prototype.each)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>emit (type)](#apidoc.element.sqlite3.Statement.prototype.emit)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>eventNames ()](#apidoc.element.sqlite3.Statement.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>finalize ()](#apidoc.element.sqlite3.Statement.prototype.finalize)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>get ()](#apidoc.element.sqlite3.Statement.prototype.get)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>getMaxListeners ()](#apidoc.element.sqlite3.Statement.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>listenerCount (type)](#apidoc.element.sqlite3.Statement.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>listeners (type)](#apidoc.element.sqlite3.Statement.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>map ()](#apidoc.element.sqlite3.Statement.prototype.map)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>on (type, listener)](#apidoc.element.sqlite3.Statement.prototype.on)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>once (type, listener)](#apidoc.element.sqlite3.Statement.prototype.once)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>prependListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>removeAllListeners (type)](#apidoc.element.sqlite3.Statement.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>removeListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>reset ()](#apidoc.element.sqlite3.Statement.prototype.reset)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>run ()](#apidoc.element.sqlite3.Statement.prototype.run)
1.  [function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>setMaxListeners (n)](#apidoc.element.sqlite3.Statement.prototype.setMaxListeners)
1.  undefined <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>domain

#### [module sqlite3.cached](#apidoc.module.sqlite3.cached)
1.  [function <span class="apidocSignatureSpan">sqlite3.cached.</span>Database (file, a, b)](#apidoc.element.sqlite3.cached.Database)
1.  object <span class="apidocSignatureSpan">sqlite3.cached.</span>objects

#### [module sqlite3.trace](#apidoc.module.sqlite3.trace)
1.  [function <span class="apidocSignatureSpan">sqlite3.trace.</span>extendTrace (object, property, pos)](#apidoc.element.sqlite3.trace.extendTrace)



# <a name="apidoc.module.sqlite3"></a>[module sqlite3](#apidoc.module.sqlite3)

#### <a name="apidoc.element.sqlite3.Database"></a>[function <span class="apidocSignatureSpan">sqlite3.</span>Database ()](#apidoc.element.sqlite3.Database)
- description and source-code
```javascript
function Database() { [native code] }
```
- example usage
```shell
...

# Usage

**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
...
```

#### <a name="apidoc.element.sqlite3.Statement"></a>[function <span class="apidocSignatureSpan">sqlite3.</span>Statement ()](#apidoc.element.sqlite3.Statement)
- description and source-code
```javascript
function Statement() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.verbose"></a>[function <span class="apidocSignatureSpan">sqlite3.</span>verbose ()](#apidoc.element.sqlite3.verbose)
- description and source-code
```javascript
verbose = function () {
    if (!isVerbose) {
        var trace = require('./trace');
        [
            'prepare',
            'get',
            'run',
            'all',
            'each',
            'map',
            'close',
            'exec'
        ].forEach(function (name) {
            trace.extendTrace(Database.prototype, name);
        });
        [
            'bind',
            'get',
            'run',
            'all',
            'each',
            'map',
            'reset',
            'finalize',
        ].forEach(function (name) {
            trace.extendTrace(Statement.prototype, name);
        });
        isVerbose = true;
    }

    return this;
}
```
- example usage
```shell
...
SQLite's [SQLCipher extension](https://github.com/sqlcipher/sqlcipher) is also supported. [(See below.)](#building-for-sqlcipher
)

# Usage

**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
...
```



# <a name="apidoc.module.sqlite3.Database"></a>[module sqlite3.Database](#apidoc.module.sqlite3.Database)

#### <a name="apidoc.element.sqlite3.Database.Database"></a>[function <span class="apidocSignatureSpan">sqlite3.</span>Database ()](#apidoc.element.sqlite3.Database.Database)
- description and source-code
```javascript
function Database() { [native code] }
```
- example usage
```shell
...

# Usage

**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
...
```



# <a name="apidoc.module.sqlite3.Database.prototype"></a>[module sqlite3.Database.prototype](#apidoc.module.sqlite3.Database.prototype)

#### <a name="apidoc.element.sqlite3.Database.prototype.addListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>addListener (type)](#apidoc.element.sqlite3.Database.prototype.addListener)
- description and source-code
```javascript
addListener = function (type) {
    var val = EventEmitter.prototype.addListener.apply(this, arguments);
    if (supportedEvents.indexOf(type) >= 0) {
        this.configure(type, true);
    }
    return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.all"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>all (sql)](#apidoc.element.sqlite3.Database.prototype.all)
- description and source-code
```javascript
all = function (sql) {
    var errBack;
    var args = Array.prototype.slice.call(arguments, 1);
    if (typeof args[args.length - 1] === 'function') {
        var callback = args[args.length - 1];
        errBack = function(err) {
            if (err) {
                callback(err);
            }
        };
    }
    var statement = new Statement(this, sql, errBack);
    return fn.call(this, statement, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.close"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>close ()](#apidoc.element.sqlite3.Database.prototype.close)
- description and source-code
```javascript
function close() { [native code] }
```
- example usage
```shell
...
 stmt.finalize();

 db.each("SELECT rowid AS id, info FROM lorem", function(err, row) {
     console.log(row.id + ": " + row.info);
 });
});

db.close();
'''

# Features

- Straightforward query and parameter binding interface
- Full Buffer/Blob support
- Extensive [debugging support](https://github.com/mapbox/node-sqlite3/wiki/Debugging)
...
```

#### <a name="apidoc.element.sqlite3.Database.prototype.configure"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>configure ()](#apidoc.element.sqlite3.Database.prototype.configure)
- description and source-code
```javascript
function configure() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.each"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>each (sql)](#apidoc.element.sqlite3.Database.prototype.each)
- description and source-code
```javascript
each = function (sql) {
    var errBack;
    var args = Array.prototype.slice.call(arguments, 1);
    if (typeof args[args.length - 1] === 'function') {
        var callback = args[args.length - 1];
        errBack = function(err) {
            if (err) {
                callback(err);
            }
        };
    }
    var statement = new Statement(this, sql, errBack);
    return fn.call(this, statement, args);
}
```
- example usage
```shell
...

  var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
  for (var i = 0; i < 10; i++) {
      stmt.run("Ipsum " + i);
  }
  stmt.finalize();

  db.each("SELECT rowid AS id, info FROM lorem", function(err, row) {
      console.log(row.id + ": " + row.info);
  });
});

db.close();
'''
...
```

#### <a name="apidoc.element.sqlite3.Database.prototype.emit"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>emit (type)](#apidoc.element.sqlite3.Database.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>eventNames ()](#apidoc.element.sqlite3.Database.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.exec"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>exec ()](#apidoc.element.sqlite3.Database.prototype.exec)
- description and source-code
```javascript
function exec() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.get"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>get (sql)](#apidoc.element.sqlite3.Database.prototype.get)
- description and source-code
```javascript
get = function (sql) {
    var errBack;
    var args = Array.prototype.slice.call(arguments, 1);
    if (typeof args[args.length - 1] === 'function') {
        var callback = args[args.length - 1];
        errBack = function(err) {
            if (err) {
                callback(err);
            }
        };
    }
    var statement = new Statement(this, sql, errBack);
    return fn.call(this, statement, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>getMaxListeners ()](#apidoc.element.sqlite3.Database.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.interrupt"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>interrupt ()](#apidoc.element.sqlite3.Database.prototype.interrupt)
- description and source-code
```javascript
function interrupt() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>listenerCount (type)](#apidoc.element.sqlite3.Database.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.listeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>listeners (type)](#apidoc.element.sqlite3.Database.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.loadExtension"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>loadExtension ()](#apidoc.element.sqlite3.Database.prototype.loadExtension)
- description and source-code
```javascript
function loadExtension() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.map"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>map (sql)](#apidoc.element.sqlite3.Database.prototype.map)
- description and source-code
```javascript
map = function (sql) {
    var errBack;
    var args = Array.prototype.slice.call(arguments, 1);
    if (typeof args[args.length - 1] === 'function') {
        var callback = args[args.length - 1];
        errBack = function(err) {
            if (err) {
                callback(err);
            }
        };
    }
    var statement = new Statement(this, sql, errBack);
    return fn.call(this, statement, args);
}
```
- example usage
```shell
...
var util = require('util');

function extendTrace(object, property, pos) {
    var old = object[property];
    object[property] = function() {
var error = new Error();
var name = object.constructor.name + '#' + property + '(' +
    Array.prototype.slice.call(arguments).map(function(el) {
        return util.inspect(el, false, 0);
    }).join(', ') + ')';

if (typeof pos === 'undefined') pos = -1;
if (pos < 0) pos += arguments.length;
var cb = arguments[pos];
if (typeof arguments[pos] === 'function') {
...
```

#### <a name="apidoc.element.sqlite3.Database.prototype.on"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>on (type)](#apidoc.element.sqlite3.Database.prototype.on)
- description and source-code
```javascript
on = function (type) {
    var val = EventEmitter.prototype.addListener.apply(this, arguments);
    if (supportedEvents.indexOf(type) >= 0) {
        this.configure(type, true);
    }
    return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.once"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>once (type, listener)](#apidoc.element.sqlite3.Database.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.parallelize"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>parallelize ()](#apidoc.element.sqlite3.Database.prototype.parallelize)
- description and source-code
```javascript
function parallelize() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.prepare"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>prepare (sql)](#apidoc.element.sqlite3.Database.prototype.prepare)
- description and source-code
```javascript
prepare = function (sql) {
    var errBack;
    var args = Array.prototype.slice.call(arguments, 1);
    if (typeof args[args.length - 1] === 'function') {
        var callback = args[args.length - 1];
        errBack = function(err) {
            if (err) {
                callback(err);
            }
        };
    }
    var statement = new Statement(this, sql, errBack);
    return fn.call(this, statement, args);
}
```
- example usage
```shell
...
''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
}
stmt.finalize();

db.each("SELECT rowid AS id, info FROM lorem", function(err, row) {
    console.log(row.id + ": " + row.info);
...
```

#### <a name="apidoc.element.sqlite3.Database.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>prependListener (type, listener)](#apidoc.element.sqlite3.Database.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.sqlite3.Database.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>removeAllListeners (type)](#apidoc.element.sqlite3.Database.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function (type) {
    var val = EventEmitter.prototype.removeAllListeners.apply(this, arguments);
    if (supportedEvents.indexOf(type) >= 0) {
        this.configure(type, false);
    }
    return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>removeListener (type)](#apidoc.element.sqlite3.Database.prototype.removeListener)
- description and source-code
```javascript
removeListener = function (type) {
    var val = EventEmitter.prototype.removeListener.apply(this, arguments);
    if (supportedEvents.indexOf(type) >= 0 && !this._events[type]) {
        this.configure(type, false);
    }
    return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.run"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>run (sql)](#apidoc.element.sqlite3.Database.prototype.run)
- description and source-code
```javascript
run = function (sql) {
    var errBack;
    var args = Array.prototype.slice.call(arguments, 1);
    if (typeof args[args.length - 1] === 'function') {
        var callback = args[args.length - 1];
        errBack = function(err) {
            if (err) {
                callback(err);
            }
        };
    }
    var statement = new Statement(this, sql, errBack);
    return fn.call(this, statement, args);
}
```
- example usage
```shell
...
**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
}
stmt.finalize();
...
```

#### <a name="apidoc.element.sqlite3.Database.prototype.serialize"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>serialize ()](#apidoc.element.sqlite3.Database.prototype.serialize)
- description and source-code
```javascript
function serialize() { [native code] }
```
- example usage
```shell
...

**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
}
stmt.finalize();
...
```

#### <a name="apidoc.element.sqlite3.Database.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>setMaxListeners (n)](#apidoc.element.sqlite3.Database.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Database.prototype.wait"></a>[function <span class="apidocSignatureSpan">sqlite3.Database.prototype.</span>wait ()](#apidoc.element.sqlite3.Database.prototype.wait)
- description and source-code
```javascript
function wait() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sqlite3.Statement"></a>[module sqlite3.Statement](#apidoc.module.sqlite3.Statement)

#### <a name="apidoc.element.sqlite3.Statement.Statement"></a>[function <span class="apidocSignatureSpan">sqlite3.</span>Statement ()](#apidoc.element.sqlite3.Statement.Statement)
- description and source-code
```javascript
function Statement() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sqlite3.Statement.prototype"></a>[module sqlite3.Statement.prototype](#apidoc.module.sqlite3.Statement.prototype)

#### <a name="apidoc.element.sqlite3.Statement.prototype.addListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>addListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.all"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>all ()](#apidoc.element.sqlite3.Statement.prototype.all)
- description and source-code
```javascript
function all() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.bind"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>bind ()](#apidoc.element.sqlite3.Statement.prototype.bind)
- description and source-code
```javascript
function bind() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.each"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>each ()](#apidoc.element.sqlite3.Statement.prototype.each)
- description and source-code
```javascript
function each() { [native code] }
```
- example usage
```shell
...

  var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
  for (var i = 0; i < 10; i++) {
      stmt.run("Ipsum " + i);
  }
  stmt.finalize();

  db.each("SELECT rowid AS id, info FROM lorem", function(err, row) {
      console.log(row.id + ": " + row.info);
  });
});

db.close();
'''
...
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.emit"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>emit (type)](#apidoc.element.sqlite3.Statement.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>eventNames ()](#apidoc.element.sqlite3.Statement.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.finalize"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>finalize ()](#apidoc.element.sqlite3.Statement.prototype.finalize)
- description and source-code
```javascript
function finalize() { [native code] }
```
- example usage
```shell
...
db.serialize(function() {
  db.run("CREATE TABLE lorem (info TEXT)");

  var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
  for (var i = 0; i < 10; i++) {
      stmt.run("Ipsum " + i);
  }
  stmt.finalize();

  db.each("SELECT rowid AS id, info FROM lorem", function(err, row) {
      console.log(row.id + ": " + row.info);
  });
});

db.close();
...
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.get"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>get ()](#apidoc.element.sqlite3.Statement.prototype.get)
- description and source-code
```javascript
function get() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>getMaxListeners ()](#apidoc.element.sqlite3.Statement.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>listenerCount (type)](#apidoc.element.sqlite3.Statement.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.listeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>listeners (type)](#apidoc.element.sqlite3.Statement.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.map"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>map ()](#apidoc.element.sqlite3.Statement.prototype.map)
- description and source-code
```javascript
map = function () {
    var params = Array.prototype.slice.call(arguments);
    var callback = params.pop();
    params.push(function(err, rows) {
        if (err) return callback(err);
        var result = {};
        if (rows.length) {
            var keys = Object.keys(rows[0]), key = keys[0];
            if (keys.length > 2) {
                // Value is an object
                for (var i = 0; i < rows.length; i++) {
                    result[rows[i][key]] = rows[i];
                }
            } else {
                var value = keys[1];
                // Value is a plain value
                for (i = 0; i < rows.length; i++) {
                    result[rows[i][key]] = rows[i][value];
                }
            }
        }
        callback(err, result);
    });
    return this.all.apply(this, params);
}
```
- example usage
```shell
...
var util = require('util');

function extendTrace(object, property, pos) {
    var old = object[property];
    object[property] = function() {
var error = new Error();
var name = object.constructor.name + '#' + property + '(' +
    Array.prototype.slice.call(arguments).map(function(el) {
        return util.inspect(el, false, 0);
    }).join(', ') + ')';

if (typeof pos === 'undefined') pos = -1;
if (pos < 0) pos += arguments.length;
var cb = arguments[pos];
if (typeof arguments[pos] === 'function') {
...
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.on"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>on (type, listener)](#apidoc.element.sqlite3.Statement.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.once"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>once (type, listener)](#apidoc.element.sqlite3.Statement.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>prependListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>removeAllListeners (type)](#apidoc.element.sqlite3.Statement.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>removeListener (type, listener)](#apidoc.element.sqlite3.Statement.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.reset"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>reset ()](#apidoc.element.sqlite3.Statement.prototype.reset)
- description and source-code
```javascript
function reset() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.run"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>run ()](#apidoc.element.sqlite3.Statement.prototype.run)
- description and source-code
```javascript
function run() { [native code] }
```
- example usage
```shell
...
**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
}
stmt.finalize();
...
```

#### <a name="apidoc.element.sqlite3.Statement.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">sqlite3.Statement.prototype.</span>setMaxListeners (n)](#apidoc.element.sqlite3.Statement.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.sqlite3.cached"></a>[module sqlite3.cached](#apidoc.module.sqlite3.cached)

#### <a name="apidoc.element.sqlite3.cached.Database"></a>[function <span class="apidocSignatureSpan">sqlite3.cached.</span>Database (file, a, b)](#apidoc.element.sqlite3.cached.Database)
- description and source-code
```javascript
Database = function (file, a, b) {
    if (file === '' || file === ':memory:') {
        // Don't cache special databases.
        return new Database(file, a, b);
    }

    var db;
    file = path.resolve(file);
    function cb() { callback.call(db, null); }

    if (!sqlite3.cached.objects[file]) {
        db = sqlite3.cached.objects[file] = new Database(file, a, b);
    }
    else {
        // Make sure the callback is called.
        db = sqlite3.cached.objects[file];
        var callback = (typeof a === 'number') ? b : a;
        if (typeof callback === 'function') {
            if (db.open) process.nextTick(cb);
            else db.once('open', cb);
        }
    }

    return db;
}
```
- example usage
```shell
...

# Usage

**Note:** the module must be [installed](#installing) before use.

''' js
var sqlite3 = require('sqlite3').verbose();
var db = new sqlite3.Database(':memory:');

db.serialize(function() {
db.run("CREATE TABLE lorem (info TEXT)");

var stmt = db.prepare("INSERT INTO lorem VALUES (?)");
for (var i = 0; i < 10; i++) {
    stmt.run("Ipsum " + i);
...
```



# <a name="apidoc.module.sqlite3.trace"></a>[module sqlite3.trace](#apidoc.module.sqlite3.trace)

#### <a name="apidoc.element.sqlite3.trace.extendTrace"></a>[function <span class="apidocSignatureSpan">sqlite3.trace.</span>extendTrace (object, property, pos)](#apidoc.element.sqlite3.trace.extendTrace)
- description and source-code
```javascript
function extendTrace(object, property, pos) {
    var old = object[property];
    object[property] = function() {
        var error = new Error();
        var name = object.constructor.name + '#' + property + '(' +
            Array.prototype.slice.call(arguments).map(function(el) {
                return util.inspect(el, false, 0);
            }).join(', ') + ')';

        if (typeof pos === 'undefined') pos = -1;
        if (pos < 0) pos += arguments.length;
        var cb = arguments[pos];
        if (typeof arguments[pos] === 'function') {
            arguments[pos] = function replacement() {
                try {
                    return cb.apply(this, arguments);
                } catch (err) {
                    if (err && err.stack && !err.__augmented) {
                        err.stack = filter(err).join('\n');
                        err.stack += '\n--> in ' + name;
                        err.stack += '\n' + filter(error).slice(1).join('\n');
                        err.__augmented = true;
                    }
                    throw err;
                }
            };
        }
        return old.apply(this, arguments);
    };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
