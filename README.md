# api documentation for  [kerberos (v0.0.23)](https://github.com/christkv/kerberos#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-kerberos.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-kerberos) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-kerberos.svg)](https://travis-ci.org/npmdoc/node-npmdoc-kerberos)
#### Kerberos library for Node.js

[![NPM](https://nodei.co/npm/kerberos.png?downloads=true)](https://www.npmjs.com/package/kerberos)

[![apidoc](https://npmdoc.github.io/node-npmdoc-kerberos/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-kerberos_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-kerberos/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-kerberos/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-kerberos/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christian Amor Kvalheim"
    },
    "bugs": {
        "url": "https://github.com/christkv/kerberos/issues"
    },
    "dependencies": {
        "nan": "~2.5.1"
    },
    "description": "Kerberos library for Node.js",
    "devDependencies": {
        "nodeunit": "latest"
    },
    "directories": {},
    "dist": {
        "shasum": "6aa46afdb9786c6919388cc5b408f012c71f0fd1",
        "tarball": "https://registry.npmjs.org/kerberos/-/kerberos-0.0.23.tgz"
    },
    "gitHead": "035be2e4619d7f3d7ea5103da1f60a6045ef8d7c",
    "homepage": "https://github.com/christkv/kerberos#readme",
    "keywords": [
        "kerberos",
        "security",
        "authentication"
    ],
    "license": "Apache-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "christkv",
            "email": "christkv@gmail.com"
        }
    ],
    "name": "kerberos",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/christkv/kerberos.git"
    },
    "scripts": {
        "install": "(node-gyp rebuild) || (exit 0)",
        "test": "nodeunit ./test"
    },
    "version": "0.0.23"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module kerberos](#apidoc.module.kerberos)
1.  [function <span class="apidocSignatureSpan">kerberos.</span>Kerberos ()](#apidoc.element.kerberos.Kerberos)
1.  [function <span class="apidocSignatureSpan">kerberos.</span>processes.MongoAuthProcess (host, port, service_name, options)](#apidoc.element.kerberos.processes.MongoAuthProcess)
1.  object <span class="apidocSignatureSpan">kerberos.</span>Kerberos.prototype
1.  object <span class="apidocSignatureSpan">kerberos.</span>processes
1.  object <span class="apidocSignatureSpan">kerberos.</span>processes.MongoAuthProcess.prototype

#### [module kerberos.Kerberos](#apidoc.module.kerberos.Kerberos)
1.  [function <span class="apidocSignatureSpan">kerberos.</span>Kerberos ()](#apidoc.element.kerberos.Kerberos.Kerberos)
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>AUTH_GSS_COMPLETE
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>AUTH_GSS_CONTINUE
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_ANON_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_CONF_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_DELEG_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_INTEG_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_MUTUAL_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_PROT_READY_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_REPLAY_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_SEQUENCE_FLAG
1.  number <span class="apidocSignatureSpan">kerberos.Kerberos.</span>GSS_C_TRANS_FLAG

#### [module kerberos.Kerberos.prototype](#apidoc.module.kerberos.Kerberos.prototype)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>acquireAlternateCredentials (user_name, password, domain)](#apidoc.element.kerberos.Kerberos.prototype.acquireAlternateCredentials)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientClean (context, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientClean)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientInit (uri, flags, credentialsCache, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientInit)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientStep (context, challenge, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientStep)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientUnwrap (context, challenge, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientUnwrap)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientWrap (context, challenge, user_name, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientWrap)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSServerClean (context, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSServerClean)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSServerInit (service, constrained_delegation, username, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSServerInit)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSServerStep (context, authData, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSServerStep)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authUserKrb5Password (username, password, service, callback)](#apidoc.element.kerberos.Kerberos.prototype.authUserKrb5Password)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>decryptMessage (challenge)](#apidoc.element.kerberos.Kerberos.prototype.decryptMessage)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>encryptMessage (challenge)](#apidoc.element.kerberos.Kerberos.prototype.encryptMessage)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>prepareOutboundPackage (principal, inputdata)](#apidoc.element.kerberos.Kerberos.prototype.prepareOutboundPackage)
1.  [function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>queryContextAttribute (attribute)](#apidoc.element.kerberos.Kerberos.prototype.queryContextAttribute)

#### [module kerberos.processes](#apidoc.module.kerberos.processes)
1.  [function <span class="apidocSignatureSpan">kerberos.processes.</span>MongoAuthProcess (host, port, service_name, options)](#apidoc.element.kerberos.processes.MongoAuthProcess)

#### [module kerberos.processes.MongoAuthProcess](#apidoc.module.kerberos.processes.MongoAuthProcess)
1.  [function <span class="apidocSignatureSpan">kerberos.processes.</span>MongoAuthProcess (host, port, service_name, options)](#apidoc.element.kerberos.processes.MongoAuthProcess.MongoAuthProcess)

#### [module kerberos.processes.MongoAuthProcess.prototype](#apidoc.module.kerberos.processes.MongoAuthProcess.prototype)
1.  [function <span class="apidocSignatureSpan">kerberos.processes.MongoAuthProcess.prototype.</span>init (username, password, callback)](#apidoc.element.kerberos.processes.MongoAuthProcess.prototype.init)
1.  [function <span class="apidocSignatureSpan">kerberos.processes.MongoAuthProcess.prototype.</span>transition (payload, callback)](#apidoc.element.kerberos.processes.MongoAuthProcess.prototype.transition)



# <a name="apidoc.module.kerberos"></a>[module kerberos](#apidoc.module.kerberos)

#### <a name="apidoc.element.kerberos.Kerberos"></a>[function <span class="apidocSignatureSpan">kerberos.</span>Kerberos ()](#apidoc.element.kerberos.Kerberos)
- description and source-code
```javascript
Kerberos = function () {
  this._native_kerberos = new KerberosNative();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.processes.MongoAuthProcess"></a>[function <span class="apidocSignatureSpan">kerberos.</span>processes.MongoAuthProcess (host, port, service_name, options)](#apidoc.element.kerberos.processes.MongoAuthProcess)
- description and source-code
```javascript
processes.MongoAuthProcess = function (host, port, service_name, options) {
  // Check what system we are on
  if(process.platform == 'win32') {
    this._processor = new Win32MongoProcessor(host, port, service_name, options);
  } else {
    this._processor = new UnixMongoProcessor(host, port, service_name, options);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.kerberos.Kerberos"></a>[module kerberos.Kerberos](#apidoc.module.kerberos.Kerberos)

#### <a name="apidoc.element.kerberos.Kerberos.Kerberos"></a>[function <span class="apidocSignatureSpan">kerberos.</span>Kerberos ()](#apidoc.element.kerberos.Kerberos.Kerberos)
- description and source-code
```javascript
Kerberos = function () {
  this._native_kerberos = new KerberosNative();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.kerberos.Kerberos.prototype"></a>[module kerberos.Kerberos.prototype](#apidoc.module.kerberos.Kerberos.prototype)

#### <a name="apidoc.element.kerberos.Kerberos.prototype.acquireAlternateCredentials"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>acquireAlternateCredentials (user_name, password, domain)](#apidoc.element.kerberos.Kerberos.prototype.acquireAlternateCredentials)
- description and source-code
```javascript
acquireAlternateCredentials = function (user_name, password, domain) {
  return this._native_kerberos.acquireAlternateCredentials(user_name, password, domain);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSClientClean"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientClean (context, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientClean)
- description and source-code
```javascript
authGSSClientClean = function (context, callback) {
  return this._native_kerberos.authGSSClientClean(context, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSClientInit"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientInit (uri, flags, credentialsCache, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientInit)
- description and source-code
```javascript
authGSSClientInit = function (uri, flags, credentialsCache, callback) {
  if (typeof(credentialsCache) == 'function') {
    callback = credentialsCache;
    credentialsCache = '';
  }

  if (credentialsCache === undefined) {
      credentialsCache = '';
  }

  return this._native_kerberos.authGSSClientInit(uri, flags, credentialsCache, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSClientStep"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientStep (context, challenge, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientStep)
- description and source-code
```javascript
authGSSClientStep = function (context, challenge, callback) {
  if(typeof challenge == 'function') {
    callback = challenge;
    challenge = '';
  }

  return this._native_kerberos.authGSSClientStep(context, challenge, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSClientUnwrap"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientUnwrap (context, challenge, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientUnwrap)
- description and source-code
```javascript
authGSSClientUnwrap = function (context, challenge, callback) {
  if(typeof challenge == 'function') {
    callback = challenge;
    challenge = '';
  }

  return this._native_kerberos.authGSSClientUnwrap(context, challenge, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSClientWrap"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSClientWrap (context, challenge, user_name, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSClientWrap)
- description and source-code
```javascript
authGSSClientWrap = function (context, challenge, user_name, callback) {
  if(typeof user_name == 'function') {
    callback = user_name;
    user_name = '';
  }

  return this._native_kerberos.authGSSClientWrap(context, challenge, user_name, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSServerClean"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSServerClean (context, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSServerClean)
- description and source-code
```javascript
authGSSServerClean = function (context, callback) {
  return this._native_kerberos.authGSSServerClean(context, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSServerInit"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSServerInit (service, constrained_delegation, username, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSServerInit)
- description and source-code
```javascript
authGSSServerInit = function (service, constrained_delegation, username, callback) {
  if(typeof(constrained_delegation) === 'function') {
	  callback = constrained_delegation;
	  constrained_delegation = false;
	  username = null;
  }

  if (typeof(constrained_delegation) === 'string') {
	  throw new Error("S4U2Self protocol transation is not possible without enabling constrained delegation");
  }

  if (typeof(username) === 'function') {
	  callback = username;
	  username = null;
  }

  constrained_delegation = !!constrained_delegation;

  return this._native_kerberos.authGSSServerInit(service, constrained_delegation, username, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authGSSServerStep"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authGSSServerStep (context, authData, callback)](#apidoc.element.kerberos.Kerberos.prototype.authGSSServerStep)
- description and source-code
```javascript
authGSSServerStep = function (context, authData, callback) {
  return this._native_kerberos.authGSSServerStep(context, authData, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.authUserKrb5Password"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>authUserKrb5Password (username, password, service, callback)](#apidoc.element.kerberos.Kerberos.prototype.authUserKrb5Password)
- description and source-code
```javascript
authUserKrb5Password = function (username, password, service, callback) {
    return this._native_kerberos.authUserKrb5Password(username, password, service, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.decryptMessage"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>decryptMessage (challenge)](#apidoc.element.kerberos.Kerberos.prototype.decryptMessage)
- description and source-code
```javascript
decryptMessage = function (challenge) {
  return this._native_kerberos.decryptMessage(challenge);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.encryptMessage"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>encryptMessage (challenge)](#apidoc.element.kerberos.Kerberos.prototype.encryptMessage)
- description and source-code
```javascript
encryptMessage = function (challenge) {
  return this._native_kerberos.encryptMessage(challenge);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.prepareOutboundPackage"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>prepareOutboundPackage (principal, inputdata)](#apidoc.element.kerberos.Kerberos.prototype.prepareOutboundPackage)
- description and source-code
```javascript
prepareOutboundPackage = function (principal, inputdata) {
  return this._native_kerberos.prepareOutboundPackage(principal, inputdata);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.Kerberos.prototype.queryContextAttribute"></a>[function <span class="apidocSignatureSpan">kerberos.Kerberos.prototype.</span>queryContextAttribute (attribute)](#apidoc.element.kerberos.Kerberos.prototype.queryContextAttribute)
- description and source-code
```javascript
queryContextAttribute = function (attribute) {
  if(typeof attribute != 'number' && attribute != 0x00) throw new Error("Attribute not supported");
  return this._native_kerberos.queryContextAttribute(attribute);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.kerberos.processes"></a>[module kerberos.processes](#apidoc.module.kerberos.processes)

#### <a name="apidoc.element.kerberos.processes.MongoAuthProcess"></a>[function <span class="apidocSignatureSpan">kerberos.processes.</span>MongoAuthProcess (host, port, service_name, options)](#apidoc.element.kerberos.processes.MongoAuthProcess)
- description and source-code
```javascript
MongoAuthProcess = function (host, port, service_name, options) {
  // Check what system we are on
  if(process.platform == 'win32') {
    this._processor = new Win32MongoProcessor(host, port, service_name, options);
  } else {
    this._processor = new UnixMongoProcessor(host, port, service_name, options);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.kerberos.processes.MongoAuthProcess"></a>[module kerberos.processes.MongoAuthProcess](#apidoc.module.kerberos.processes.MongoAuthProcess)

#### <a name="apidoc.element.kerberos.processes.MongoAuthProcess.MongoAuthProcess"></a>[function <span class="apidocSignatureSpan">kerberos.processes.</span>MongoAuthProcess (host, port, service_name, options)](#apidoc.element.kerberos.processes.MongoAuthProcess.MongoAuthProcess)
- description and source-code
```javascript
MongoAuthProcess = function (host, port, service_name, options) {
  // Check what system we are on
  if(process.platform == 'win32') {
    this._processor = new Win32MongoProcessor(host, port, service_name, options);
  } else {
    this._processor = new UnixMongoProcessor(host, port, service_name, options);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.kerberos.processes.MongoAuthProcess.prototype"></a>[module kerberos.processes.MongoAuthProcess.prototype](#apidoc.module.kerberos.processes.MongoAuthProcess.prototype)

#### <a name="apidoc.element.kerberos.processes.MongoAuthProcess.prototype.init"></a>[function <span class="apidocSignatureSpan">kerberos.processes.MongoAuthProcess.prototype.</span>init (username, password, callback)](#apidoc.element.kerberos.processes.MongoAuthProcess.prototype.init)
- description and source-code
```javascript
init = function (username, password, callback) {
  this._processor.init(username, password, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.kerberos.processes.MongoAuthProcess.prototype.transition"></a>[function <span class="apidocSignatureSpan">kerberos.processes.MongoAuthProcess.prototype.</span>transition (payload, callback)](#apidoc.element.kerberos.processes.MongoAuthProcess.prototype.transition)
- description and source-code
```javascript
transition = function (payload, callback) {
  this._processor.transition(payload, callback);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
