# api documentation for  [superstatic (v4.0.3)](https://github.com/firebase/superstatic#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-superstatic.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-superstatic) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-superstatic.svg)](https://travis-ci.org/npmdoc/node-npmdoc-superstatic)
#### A static file server for fancy apps

[![NPM](https://nodei.co/npm/superstatic.png?downloads=true)](https://www.npmjs.com/package/superstatic)

[![apidoc](https://npmdoc.github.io/node-npmdoc-superstatic/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-superstatic_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-superstatic/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-superstatic/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-superstatic/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Firebase",
        "url": "https://www.firebase.com/"
    },
    "bin": {
        "superstatic": "bin/server"
    },
    "bugs": {
        "url": "https://github.com/firebase/superstatic/issues"
    },
    "dependencies": {
        "as-array": "^2.0.0",
        "async": "^1.5.2",
        "basic-auth-connect": "^1.0.0",
        "chalk": "^1.0.0",
        "char-spinner": "^1.0.1",
        "compare-semver": "^1.0.0",
        "compression": "^1.2.2",
        "connect": "^3.3.3",
        "connect-query": "^0.2.0",
        "destroy": "^1.0.3",
        "fast-url-parser": "^1.1.3",
        "fs-extra": "^0.30.0",
        "glob": "^7.0.3",
        "glob-slasher": "^1.0.1",
        "home-dir": "^1.0.0",
        "is-url": "^1.2.1",
        "join-path": "^1.0.0",
        "lodash": "^4.11.2",
        "mime-types": "^2.0.4",
        "minimatch": "^3.0.2",
        "morgan": "^1.5.0",
        "nash": "^2.0.0",
        "on-finished": "^2.2.0",
        "on-headers": "^1.0.0",
        "path-to-regexp": "^1.2.1",
        "router": "^1.0.0",
        "rsvp": "^3.1.0",
        "string-length": "^1.0.0",
        "try-require": "^1.0.0",
        "update-notifier": "^1.0.1"
    },
    "description": "A static file server for fancy apps",
    "devDependencies": {
        "chai": "^3.0.0",
        "chai-as-promised": "^5.1.0",
        "concat-stream": "^1.5.1",
        "eslint": "^2.9.0",
        "istanbul": "^0.4.0",
        "mocha": "^2.0.1",
        "nsp": "^2.4.0",
        "request": "^2.51.0",
        "sinon": "^1.17.2",
        "sinon-chai": "^2.8.0",
        "std-mocks": "^1.0.0",
        "supertest": "^1.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "a8ca3770a98489711917f3bd16f719ea92d4e686",
        "tarball": "https://registry.npmjs.org/superstatic/-/superstatic-4.0.3.tgz"
    },
    "gitHead": "572e2ad99b5322810b9d9c16b00983942ce189f4",
    "homepage": "https://github.com/firebase/superstatic#readme",
    "keywords": [
        "static",
        "server",
        "firebase",
        "hosting",
        "pushstate",
        "html5",
        "router",
        "file",
        "directory",
        "hash",
        "hashbang"
    ],
    "license": "MIT",
    "main": "./lib",
    "maintainers": [
        {
            "name": "scottcorgan",
            "email": "scottcorgan@gmail.com"
        },
        {
            "name": "mbleigh",
            "email": "michael@intridea.com"
        }
    ],
    "name": "superstatic",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/firebase/superstatic.git"
    },
    "scripts": {
        "audit": "npm shrinkwrap --dev && nsp check || true && rm npm-shrinkwrap.json",
        "coverage": "istanbul cover --print detail ./node_modules/.bin/_mocha -- test/unit/** test/integration/**",
        "lint": "eslint .",
        "outdated": "npm outdated --depth 0",
        "test": "npm run lint && npm run coverage",
        "test-integration": "mocha test/integration/**",
        "test-unit": "mocha test/unit/**",
        "watch": "mocha -w test/unit/** test/integration/**"
    },
    "version": "4.0.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module superstatic](#apidoc.module.superstatic)
1.  [function <span class="apidocSignatureSpan">superstatic.</span>responder (req, res, options)](#apidoc.element.superstatic.responder)
1.  [function <span class="apidocSignatureSpan">superstatic.</span>server (spec)](#apidoc.element.superstatic.server)
1.  object <span class="apidocSignatureSpan">superstatic.</span>responder.prototype
1.  object <span class="apidocSignatureSpan">superstatic.</span>stacks

#### [module superstatic.responder](#apidoc.module.superstatic.responder)
1.  [function <span class="apidocSignatureSpan">superstatic.</span>responder (req, res, options)](#apidoc.element.superstatic.responder.responder)

#### [module superstatic.responder.prototype](#apidoc.module.superstatic.responder.prototype)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>_handle (item)](#apidoc.element.superstatic.responder.prototype._handle)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handle (item, next)](#apidoc.element.superstatic.responder.prototype.handle)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleData (data)](#apidoc.element.superstatic.responder.prototype.handleData)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleError (err)](#apidoc.element.superstatic.responder.prototype.handleError)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleFile (file)](#apidoc.element.superstatic.responder.prototype.handleFile)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleFileStream (file, result)](#apidoc.element.superstatic.responder.prototype.handleFileStream)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleNotModified ()](#apidoc.element.superstatic.responder.prototype.handleNotModified)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleRedirect (redirect)](#apidoc.element.superstatic.responder.prototype.handleRedirect)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleStack (stack)](#apidoc.element.superstatic.responder.prototype.handleStack)
1.  [function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>isNotModified (stats)](#apidoc.element.superstatic.responder.prototype.isNotModified)



# <a name="apidoc.module.superstatic"></a>[module superstatic](#apidoc.module.superstatic)

#### <a name="apidoc.element.superstatic.responder"></a>[function <span class="apidocSignatureSpan">superstatic.</span>responder (req, res, options)](#apidoc.element.superstatic.responder)
- description and source-code
```javascript
responder = function (req, res, options) {
  this.req = req;
  this.res = res;
  this.provider = options.provider;
  this.config = options.config || {};
  this.gzip = options.gzip;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superstatic.server"></a>[function <span class="apidocSignatureSpan">superstatic.</span>server (spec)](#apidoc.element.superstatic.server)
- description and source-code
```javascript
server = function (spec) {
  spec = _.assign({fallthrough: false}, spec);

  var app = connect();
  var listen = app.listen.bind(app);

  // Override method because port and host are given
  // in the spec object
  app.listen = function(done) {
    var server = {};

    app.use(superstatic(spec));

    // Start server
    server = listen(spec.port, spec.hostname || spec.host, done);

    return server;
  };

  // Console output for network requests
  if (spec.debug) {
    app.use(networkLogger('combined'));
  }

  return app;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superstatic.responder"></a>[module superstatic.responder](#apidoc.module.superstatic.responder)

#### <a name="apidoc.element.superstatic.responder.responder"></a>[function <span class="apidocSignatureSpan">superstatic.</span>responder (req, res, options)](#apidoc.element.superstatic.responder.responder)
- description and source-code
```javascript
responder = function (req, res, options) {
  this.req = req;
  this.res = res;
  this.provider = options.provider;
  this.config = options.config || {};
  this.gzip = options.gzip;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.superstatic.responder.prototype"></a>[module superstatic.responder.prototype](#apidoc.module.superstatic.responder.prototype)

#### <a name="apidoc.element.superstatic.responder.prototype._handle"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>_handle (item)](#apidoc.element.superstatic.responder.prototype._handle)
- description and source-code
```javascript
_handle = function (item) {
  if (_.isArray(item)) {
    return this.handleStack(item);
  } else if (_.isString(item)) {
    return this.handleFile({file: item});
  } else if (_.isObject(item)) {
    if (item.file) {
      return this.handleFile(item);
    } else if (item.redirect) {
      return this.handleRedirect(item);
    } else if (item.data) {
      return this.handleData(item);
    }
  }

  return RSVP.reject(new Error(JSON.stringify(item) + ' is not a recognized responder directive'));
}
```
- example usage
```shell
...
}

return false;
};

Responder.prototype.handle = function(item, next) {
var self = this;
return this._handle(item).then(function(responded) {
  if (!responded && next) {
    next();
  }
  return responded;
}).catch(function(err) {
  return self.handleError(err);
});
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handle"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handle (item, next)](#apidoc.element.superstatic.responder.prototype.handle)
- description and source-code
```javascript
handle = function (item, next) {
  var self = this;
  return this._handle(item).then(function(responded) {
    if (!responded && next) {
      next();
    }
    return responded;
  }).catch(function(err) {
    return self.handleError(err);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleData"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleData (data)](#apidoc.element.superstatic.responder.prototype.handleData)
- description and source-code
```javascript
handleData = function (data) {
  this.res.statusCode = data.status || 200;
  this.res.setHeader('Content-Type', data.contentType || 'text/html; charset=utf-8');
  this.res.end(data.data);
  return RSVP.resolve(true);
}
```
- example usage
```shell
...
    return this.handleFile({file: item});
  } else if (_.isObject(item)) {
    if (item.file) {
      return this.handleFile(item);
    } else if (item.redirect) {
      return this.handleRedirect(item);
    } else if (item.data) {
      return this.handleData(item);
    }
  }

  return RSVP.reject(new Error(JSON.stringify(item) + ' is not a recognized responder directive'));
};

Responder.prototype.handleError = function(err) {
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleError"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleError (err)](#apidoc.element.superstatic.responder.prototype.handleError)
- description and source-code
```javascript
handleError = function (err) {
  this.res.statusCode = 500;
  console.log(err.stack);
  this.res.end('Unexpected error occurred.');
}
```
- example usage
```shell
...
var self = this;
return this._handle(item).then(function(responded) {
  if (!responded && next) {
    next();
  }
  return responded;
}).catch(function(err) {
  return self.handleError(err);
});
};

Responder.prototype._handle = function(item) {
if (_.isArray(item)) {
  return this.handleStack(item);
} else if (_.isString(item)) {
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleFile"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleFile (file)](#apidoc.element.superstatic.responder.prototype.handleFile)
- description and source-code
```javascript
handleFile = function (file) {
  var self = this;
  return this.provider(this.req, file.file).then(function(result) {
    if (!result) {
      return false;
    }

    if (self.isNotModified(result)) {
      return self.handleNotModified(result);
    }

    return self.handleFileStream(file, result);
  });
}
```
- example usage
```shell
...
});
};

Responder.prototype._handle = function(item) {
if (_.isArray(item)) {
  return this.handleStack(item);
} else if (_.isString(item)) {
  return this.handleFile({file: item});
} else if (_.isObject(item)) {
  if (item.file) {
    return this.handleFile(item);
  } else if (item.redirect) {
    return this.handleRedirect(item);
  } else if (item.data) {
    return this.handleData(item);
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleFileStream"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleFileStream (file, result)](#apidoc.element.superstatic.responder.prototype.handleFileStream)
- description and source-code
```javascript
handleFileStream = function (file, result) {
  var self = this;

  this.streamedFile = file;
  this.res.statusCode = file.status || 200;
  if (this.res.statusCode === 200 && file.file === this.config.errorPage) {
    this.res.statusCode = 404;
  }
  this.res.setHeader('Content-Type', result.contentType || mime.contentType(path.extname(file.file)));
  if (result.size) { this.res.setHeader('Content-Length', result.size); }
  if (result.etag) { this.res.setHeader('ETag', result.etag); }
  if (result.modified) {
    this.res.setHeader('Last-Modified', new Date(result.modified).toUTCString());
  }
  if (this.gzip) {
    compress(this.req, this.res, function() {
      result.stream.pipe(self.res);
    });
  } else {
    result.stream.pipe(self.res);
  }

  return awaitFinished(this.res).then(function() {
    destroy(result.stream);
    return true;
  });
}
```
- example usage
```shell
...
    return false;
  }

  if (self.isNotModified(result)) {
    return self.handleNotModified(result);
  }

  return self.handleFileStream(file, result);
});
};

Responder.prototype.handleFileStream = function(file, result) {
var self = this;

this.streamedFile = file;
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleNotModified"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleNotModified ()](#apidoc.element.superstatic.responder.prototype.handleNotModified)
- description and source-code
```javascript
handleNotModified = function () {
  this.res.statusCode = 304;
  this.res.removeHeader('Content-Type');
  this.res.removeHeader('Content-Length');
  this.res.removeHeader('Transfer-Encoding');
  this.res.end();
}
```
- example usage
```shell
...
  var self = this;
  return this.provider(this.req, file.file).then(function(result) {
    if (!result) {
      return false;
    }

    if (self.isNotModified(result)) {
      return self.handleNotModified(result);
    }

    return self.handleFileStream(file, result);
  });
};

Responder.prototype.handleFileStream = function(file, result) {
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleRedirect"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleRedirect (redirect)](#apidoc.element.superstatic.responder.prototype.handleRedirect)
- description and source-code
```javascript
handleRedirect = function (redirect) {
  this.res.statusCode = redirect.status || 301;
  this.res.setHeader('Location', redirect.redirect);
  this.res.setHeader('Content-Type', 'text/html; charset=utf-8');
  this.res.end('Redirecting to ' + redirect.redirect);
  return RSVP.resolve(true);
}
```
- example usage
```shell
...
    return this.handleStack(item);
  } else if (_.isString(item)) {
    return this.handleFile({file: item});
  } else if (_.isObject(item)) {
    if (item.file) {
      return this.handleFile(item);
    } else if (item.redirect) {
      return this.handleRedirect(item);
    } else if (item.data) {
      return this.handleData(item);
    }
  }

  return RSVP.reject(new Error(JSON.stringify(item) + ' is not a recognized responder directive'));
};
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.handleStack"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>handleStack (stack)](#apidoc.element.superstatic.responder.prototype.handleStack)
- description and source-code
```javascript
handleStack = function (stack) {
  var self = this;
  if (stack.length) {
    return this._handle(stack.shift()).then(function(responded) {
      return responded ? true : self.handleStack(stack);
    });
  }

  return RSVP.resolve(false);
}
```
- example usage
```shell
...
}).catch(function(err) {
  return self.handleError(err);
});
};

Responder.prototype._handle = function(item) {
if (_.isArray(item)) {
  return this.handleStack(item);
} else if (_.isString(item)) {
  return this.handleFile({file: item});
} else if (_.isObject(item)) {
  if (item.file) {
    return this.handleFile(item);
  } else if (item.redirect) {
    return this.handleRedirect(item);
...
```

#### <a name="apidoc.element.superstatic.responder.prototype.isNotModified"></a>[function <span class="apidocSignatureSpan">superstatic.responder.prototype.</span>isNotModified (stats)](#apidoc.element.superstatic.responder.prototype.isNotModified)
- description and source-code
```javascript
isNotModified = function (stats) {
  if (stats.etag && stats.etag === this.req.headers['if-none-match']) {
    return true;
  }

  var reqModified = this.req.headers['if-modified-since'];
  if (reqModified) {
    reqModified = new Date(reqModified).getTime();
  }
  if (stats.modified && reqModified && stats.modified < reqModified) {
    return true;
  }

  return false;
}
```
- example usage
```shell
...
Responder.prototype.handleFile = function(file) {
  var self = this;
  return this.provider(this.req, file.file).then(function(result) {
    if (!result) {
      return false;
    }

    if (self.isNotModified(result)) {
      return self.handleNotModified(result);
    }

    return self.handleFileStream(file, result);
  });
};
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
