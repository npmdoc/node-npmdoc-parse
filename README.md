# api documentation for  [parse (v1.9.2)](https://www.parse.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-parse.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-parse) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-parse.svg)](https://travis-ci.org/npmdoc/node-npmdoc-parse)
#### The Parse JavaScript SDK

[![NPM](https://nodei.co/npm/parse.png?downloads=true)](https://www.npmjs.com/package/parse)

[![apidoc](https://npmdoc.github.io/node-npmdoc-parse/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-parse_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-parse/build/apidoc.html)

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
            "name": "andrewimm",
            "email": "andrewi@fb.com"
        },
        {
            "name": "grantland",
            "email": "grantlandchew@gmail.com"
        },
        {
            "name": "lacker",
            "email": "lacker@gmail.com"
        },
        {
            "name": "nlutsenko",
            "email": "nlutsenko@me.com"
        },
        {
            "name": "peterdotjs",
            "email": "pdotjs@gmail.com"
        },
        {
            "name": "wangmengyan95",
            "email": "wangmengyan95@gmail.com"
        }
    ],
    "name": "parse",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module parse](#apidoc.module.parse)
1.  [function <span class="apidocSignatureSpan">parse.</span>ACL (arg1)](#apidoc.element.parse.ACL)
1.  [function <span class="apidocSignatureSpan">parse.</span>Config ()](#apidoc.element.parse.Config)
1.  [function <span class="apidocSignatureSpan">parse.</span>Error (code, message)](#apidoc.element.parse.Error)
1.  [function <span class="apidocSignatureSpan">parse.</span>File (name, data, type)](#apidoc.element.parse.File)
1.  [function <span class="apidocSignatureSpan">parse.</span>GeoPoint (arg1, arg2)](#apidoc.element.parse.GeoPoint)
1.  [function <span class="apidocSignatureSpan">parse.</span>Installation (attributes)](#apidoc.element.parse.Installation)
1.  [function <span class="apidocSignatureSpan">parse.</span>LiveQueryClient (_ref)](#apidoc.element.parse.LiveQueryClient)
1.  [function <span class="apidocSignatureSpan">parse.</span>Object (className, attributes, options)](#apidoc.element.parse.Object)
1.  [function <span class="apidocSignatureSpan">parse.</span>Promise (executor)](#apidoc.element.parse.Promise)
1.  [function <span class="apidocSignatureSpan">parse.</span>Query (objectClass)](#apidoc.element.parse.Query)
1.  [function <span class="apidocSignatureSpan">parse.</span>Relation (parent, key)](#apidoc.element.parse.Relation)
1.  [function <span class="apidocSignatureSpan">parse.</span>Role (name, acl)](#apidoc.element.parse.Role)
1.  [function <span class="apidocSignatureSpan">parse.</span>Session (attributes)](#apidoc.element.parse.Session)
1.  [function <span class="apidocSignatureSpan">parse.</span>User (attributes)](#apidoc.element.parse.User)
1.  [function <span class="apidocSignatureSpan">parse.</span>_ajax ()](#apidoc.element.parse._ajax)
1.  [function <span class="apidocSignatureSpan">parse.</span>_decode (_, value)](#apidoc.element.parse._decode)
1.  [function <span class="apidocSignatureSpan">parse.</span>_encode (value, _, disallowObjects)](#apidoc.element.parse._encode)
1.  [function <span class="apidocSignatureSpan">parse.</span>_getInstallationId ()](#apidoc.element.parse._getInstallationId)
1.  [function <span class="apidocSignatureSpan">parse.</span>_initialize (applicationId, javaScriptKey, masterKey)](#apidoc.element.parse._initialize)
1.  [function <span class="apidocSignatureSpan">parse.</span>_request ()](#apidoc.element.parse._request)
1.  [function <span class="apidocSignatureSpan">parse.</span>initialize (applicationId, javaScriptKey)](#apidoc.element.parse.initialize)
1.  object <span class="apidocSignatureSpan">parse.</span>Analytics
1.  object <span class="apidocSignatureSpan">parse.</span>Cloud
1.  object <span class="apidocSignatureSpan">parse.</span>CoreManager
1.  object <span class="apidocSignatureSpan">parse.</span>FacebookUtils
1.  object <span class="apidocSignatureSpan">parse.</span>LiveQuery
1.  object <span class="apidocSignatureSpan">parse.</span>LiveQuery._events
1.  object <span class="apidocSignatureSpan">parse.</span>Op
1.  object <span class="apidocSignatureSpan">parse.</span>Parse
1.  object <span class="apidocSignatureSpan">parse.</span>Push
1.  object <span class="apidocSignatureSpan">parse.</span>Storage
1.  object <span class="apidocSignatureSpan">parse.</span>node

#### [module parse.Analytics](#apidoc.module.parse.Analytics)
1.  [function <span class="apidocSignatureSpan">parse.Analytics.</span>track (name, dimensions, options)](#apidoc.element.parse.Analytics.track)

#### [module parse.Cloud](#apidoc.module.parse.Cloud)
1.  [function <span class="apidocSignatureSpan">parse.Cloud.</span>run (name, data, options)](#apidoc.element.parse.Cloud.run)

#### [module parse.CoreManager](#apidoc.module.parse.CoreManager)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>get (key)](#apidoc.element.parse.CoreManager.get)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getAnalyticsController ()](#apidoc.element.parse.CoreManager.getAnalyticsController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getCloudController ()](#apidoc.element.parse.CoreManager.getCloudController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getConfigController ()](#apidoc.element.parse.CoreManager.getConfigController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getFileController ()](#apidoc.element.parse.CoreManager.getFileController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getHooksController ()](#apidoc.element.parse.CoreManager.getHooksController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getInstallationController ()](#apidoc.element.parse.CoreManager.getInstallationController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getLiveQueryController ()](#apidoc.element.parse.CoreManager.getLiveQueryController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getObjectController ()](#apidoc.element.parse.CoreManager.getObjectController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getObjectStateController ()](#apidoc.element.parse.CoreManager.getObjectStateController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getPushController ()](#apidoc.element.parse.CoreManager.getPushController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getQueryController ()](#apidoc.element.parse.CoreManager.getQueryController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getRESTController ()](#apidoc.element.parse.CoreManager.getRESTController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getSessionController ()](#apidoc.element.parse.CoreManager.getSessionController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getStorageController ()](#apidoc.element.parse.CoreManager.getStorageController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>getUserController ()](#apidoc.element.parse.CoreManager.getUserController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>set (key, value)](#apidoc.element.parse.CoreManager.set)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setAnalyticsController (controller)](#apidoc.element.parse.CoreManager.setAnalyticsController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setCloudController (controller)](#apidoc.element.parse.CoreManager.setCloudController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setConfigController (controller)](#apidoc.element.parse.CoreManager.setConfigController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setFileController (controller)](#apidoc.element.parse.CoreManager.setFileController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setHooksController (controller)](#apidoc.element.parse.CoreManager.setHooksController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setInstallationController (controller)](#apidoc.element.parse.CoreManager.setInstallationController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setLiveQueryController (controller)](#apidoc.element.parse.CoreManager.setLiveQueryController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setObjectController (controller)](#apidoc.element.parse.CoreManager.setObjectController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setObjectStateController (controller)](#apidoc.element.parse.CoreManager.setObjectStateController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setPushController (controller)](#apidoc.element.parse.CoreManager.setPushController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setQueryController (controller)](#apidoc.element.parse.CoreManager.setQueryController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setRESTController (controller)](#apidoc.element.parse.CoreManager.setRESTController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setSessionController (controller)](#apidoc.element.parse.CoreManager.setSessionController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setStorageController (controller)](#apidoc.element.parse.CoreManager.setStorageController)
1.  [function <span class="apidocSignatureSpan">parse.CoreManager.</span>setUserController (controller)](#apidoc.element.parse.CoreManager.setUserController)

#### [module parse.FacebookUtils](#apidoc.module.parse.FacebookUtils)
1.  [function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>init (options)](#apidoc.element.parse.FacebookUtils.init)
1.  [function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>isLinked (user)](#apidoc.element.parse.FacebookUtils.isLinked)
1.  [function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>link (user, permissions, options)](#apidoc.element.parse.FacebookUtils.link)
1.  [function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>logIn (permissions, options)](#apidoc.element.parse.FacebookUtils.logIn)
1.  [function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>unlink (user, options)](#apidoc.element.parse.FacebookUtils.unlink)

#### [module parse.LiveQuery](#apidoc.module.parse.LiveQuery)
1.  [function <span class="apidocSignatureSpan">parse.LiveQuery.</span>close ()](#apidoc.element.parse.LiveQuery.close)
1.  [function <span class="apidocSignatureSpan">parse.LiveQuery.</span>open ()](#apidoc.element.parse.LiveQuery.open)
1.  number <span class="apidocSignatureSpan">parse.LiveQuery.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">parse.LiveQuery.</span>_events
1.  object <span class="apidocSignatureSpan">parse.LiveQuery.</span>domain

#### [module parse.LiveQuery._events](#apidoc.module.parse.LiveQuery._events)
1.  [function <span class="apidocSignatureSpan">parse.LiveQuery._events.</span>error ()](#apidoc.element.parse.LiveQuery._events.error)

#### [module parse.Op](#apidoc.module.parse.Op)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>Add (value)](#apidoc.element.parse.Op.Add)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>AddUnique (value)](#apidoc.element.parse.Op.AddUnique)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>Increment (amount)](#apidoc.element.parse.Op.Increment)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>Relation (adds, removes)](#apidoc.element.parse.Op.Relation)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>Remove (value)](#apidoc.element.parse.Op.Remove)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>Set (value)](#apidoc.element.parse.Op.Set)
1.  [function <span class="apidocSignatureSpan">parse.Op.</span>Unset ()](#apidoc.element.parse.Op.Unset)

#### [module parse.Push](#apidoc.module.parse.Push)
1.  [function <span class="apidocSignatureSpan">parse.Push.</span>send (data, options)](#apidoc.element.parse.Push.send)

#### [module parse.Storage](#apidoc.module.parse.Storage)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>_clear ()](#apidoc.element.parse.Storage._clear)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>async ()](#apidoc.element.parse.Storage.async)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>generatePath (path)](#apidoc.element.parse.Storage.generatePath)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>getItem (path)](#apidoc.element.parse.Storage.getItem)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>getItemAsync (path)](#apidoc.element.parse.Storage.getItemAsync)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>removeItem (path)](#apidoc.element.parse.Storage.removeItem)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>removeItemAsync (path)](#apidoc.element.parse.Storage.removeItemAsync)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>setItem (path, value)](#apidoc.element.parse.Storage.setItem)
1.  [function <span class="apidocSignatureSpan">parse.Storage.</span>setItemAsync (path, value)](#apidoc.element.parse.Storage.setItemAsync)

#### [module parse.node](#apidoc.module.parse.node)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>ACL (arg1)](#apidoc.element.parse.node.ACL)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Config ()](#apidoc.element.parse.node.Config)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Error (code, message)](#apidoc.element.parse.node.Error)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>File (name, data, type)](#apidoc.element.parse.node.File)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>GeoPoint (arg1, arg2)](#apidoc.element.parse.node.GeoPoint)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Installation (attributes)](#apidoc.element.parse.node.Installation)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>LiveQueryClient (_ref)](#apidoc.element.parse.node.LiveQueryClient)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Object (className, attributes, options)](#apidoc.element.parse.node.Object)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Promise (executor)](#apidoc.element.parse.node.Promise)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Query (objectClass)](#apidoc.element.parse.node.Query)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Relation (parent, key)](#apidoc.element.parse.node.Relation)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Role (name, acl)](#apidoc.element.parse.node.Role)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>Session (attributes)](#apidoc.element.parse.node.Session)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>User (attributes)](#apidoc.element.parse.node.User)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>_ajax ()](#apidoc.element.parse.node._ajax)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>_decode (_, value)](#apidoc.element.parse.node._decode)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>_encode (value, _, disallowObjects)](#apidoc.element.parse.node._encode)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>_getInstallationId ()](#apidoc.element.parse.node._getInstallationId)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>_initialize (applicationId, javaScriptKey, masterKey)](#apidoc.element.parse.node._initialize)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>_request ()](#apidoc.element.parse.node._request)
1.  [function <span class="apidocSignatureSpan">parse.node.</span>initialize (applicationId, javaScriptKey, masterKey)](#apidoc.element.parse.node.initialize)
1.  object <span class="apidocSignatureSpan">parse.node.</span>Analytics
1.  object <span class="apidocSignatureSpan">parse.node.</span>Cloud
1.  object <span class="apidocSignatureSpan">parse.node.</span>CoreManager
1.  object <span class="apidocSignatureSpan">parse.node.</span>FacebookUtils
1.  object <span class="apidocSignatureSpan">parse.node.</span>Hooks
1.  object <span class="apidocSignatureSpan">parse.node.</span>LiveQuery
1.  object <span class="apidocSignatureSpan">parse.node.</span>Op
1.  object <span class="apidocSignatureSpan">parse.node.</span>Parse
1.  object <span class="apidocSignatureSpan">parse.node.</span>Push
1.  object <span class="apidocSignatureSpan">parse.node.</span>Storage



# <a name="apidoc.module.parse"></a>[module parse](#apidoc.module.parse)

#### <a name="apidoc.element.parse.ACL"></a>[function <span class="apidocSignatureSpan">parse.</span>ACL (arg1)](#apidoc.element.parse.ACL)
- description and source-code
```javascript
function ParseACL(arg1) {
  (0, _classCallCheck3.default)(this, ParseACL);

  this.permissionsById = {};
  if (arg1 && (typeof arg1 === 'undefined' ? 'undefined' : (0, _typeof3.default)(arg1)) === 'object') {
    if (arg1 instanceof _ParseUser2.default) {
      this.setReadAccess(arg1, true);
      this.setWriteAccess(arg1, true);
    } else {
      for (var userId in arg1) {
        var accessList = arg1[userId];
        if (typeof userId !== 'string') {
          throw new TypeError('Tried to create an ACL with an invalid user id.');
        }
        this.permissionsById[userId] = {};
        for (var permission in accessList) {
          var allowed = accessList[permission];
          if (permission !== 'read' && permission !== 'write') {
            throw new TypeError('Tried to create an ACL with an invalid permission type.');
          }
          if (typeof allowed !== 'boolean') {
            throw new TypeError('Tried to create an ACL with an invalid permission value.');
          }
          this.permissionsById[userId][permission] = allowed;
        }
      }
    }
  } else if (typeof arg1 === 'function') {
    throw new TypeError('ParseACL constructed with a function. Did you forget ()?');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Config"></a>[function <span class="apidocSignatureSpan">parse.</span>Config ()](#apidoc.element.parse.Config)
- description and source-code
```javascript
function ParseConfig() {
  (0, _classCallCheck3.default)(this, ParseConfig);

  this.attributes = {};
  this._escapedAttributes = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Error"></a>[function <span class="apidocSignatureSpan">parse.</span>Error (code, message)](#apidoc.element.parse.Error)
- description and source-code
```javascript
function ParseError(code, message) {
  (0, _classCallCheck3.default)(this, ParseError);

  this.code = code;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.File"></a>[function <span class="apidocSignatureSpan">parse.</span>File (name, data, type)](#apidoc.element.parse.File)
- description and source-code
```javascript
function ParseFile(name, data, type) {
  (0, _classCallCheck3.default)(this, ParseFile);

  var specifiedType = type || '';

  this._name = name;

  if (data !== undefined) {
    if (Array.isArray(data)) {
      this._source = {
        format: 'base64',
        base64: ParseFile.encodeBase64(data),
        type: specifiedType
      };
    } else if (typeof File !== 'undefined' && data instanceof File) {
      this._source = {
        format: 'file',
        file: data,
        type: specifiedType
      };
    } else if (data && typeof data.base64 === 'string') {
      var _base = data.base64;
      var commaIndex = _base.indexOf(',');

      if (commaIndex !== -1) {
        var matches = dataUriRegexp.exec(_base.slice(0, commaIndex + 1));
        // if data URI with type and charset, there will be 4 matches.
        this._source = {
          format: 'base64',
          base64: _base.slice(commaIndex + 1),
          type: matches[1]
        };
      } else {
        this._source = {
          format: 'base64',
          base64: _base,
          type: specifiedType
        };
      }
    } else {
      throw new TypeError('Cannot create a Parse.File with that data.');
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.GeoPoint"></a>[function <span class="apidocSignatureSpan">parse.</span>GeoPoint (arg1, arg2)](#apidoc.element.parse.GeoPoint)
- description and source-code
```javascript
function ParseGeoPoint(arg1, arg2) {
  (0, _classCallCheck3.default)(this, ParseGeoPoint);

  if (Array.isArray(arg1)) {
    ParseGeoPoint._validate(arg1[0], arg1[1]);
    this._latitude = arg1[0];
    this._longitude = arg1[1];
  } else if ((typeof arg1 === 'undefined' ? 'undefined' : (0, _typeof3.default)(arg1)) === 'object') {
    ParseGeoPoint._validate(arg1.latitude, arg1.longitude);
    this._latitude = arg1.latitude;
    this._longitude = arg1.longitude;
  } else if (typeof arg1 === 'number' && typeof arg2 === 'number') {
    ParseGeoPoint._validate(arg1, arg2);
    this._latitude = arg1;
    this._longitude = arg2;
  } else {
    this._latitude = 0;
    this._longitude = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Installation"></a>[function <span class="apidocSignatureSpan">parse.</span>Installation (attributes)](#apidoc.element.parse.Installation)
- description and source-code
```javascript
function Installation(attributes) {
  (0, _classCallCheck3.default)(this, Installation);

  var _this = (0, _possibleConstructorReturn3.default)(this, (Installation.__proto__ || (0, _getPrototypeOf2.default)(Installation
)).call(this, '_Installation'));

  if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
    if (!_this.set(attributes || {})) {
      throw new Error('Can\'t create an invalid Session');
    }
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.LiveQueryClient"></a>[function <span class="apidocSignatureSpan">parse.</span>LiveQueryClient (_ref)](#apidoc.element.parse.LiveQueryClient)
- description and source-code
```javascript
function LiveQueryClient(_ref) {
  var applicationId = _ref.applicationId;
  var serverURL = _ref.serverURL;
  var javascriptKey = _ref.javascriptKey;
  var masterKey = _ref.masterKey;
  var sessionToken = _ref.sessionToken;
  (0, _classCallCheck3.default)(this, LiveQueryClient);

  var _this = (0, _possibleConstructorReturn3.default)(this, (LiveQueryClient.__proto__ || (0, _getPrototypeOf2.default)(LiveQueryClient
)).call(this));

  if (!serverURL || serverURL.indexOf('ws') !== 0) {
    throw new Error('You need to set a proper Parse LiveQuery server url before using LiveQueryClient');
  }

  _this.reconnectHandle = null;
  _this.attempts = 1;;
  _this.id = 0;
  _this.requestId = 1;
  _this.serverURL = serverURL;
  _this.applicationId = applicationId;
  _this.javascriptKey = javascriptKey;
  _this.masterKey = masterKey;
  _this.sessionToken = sessionToken;
  _this.connectPromise = new _ParsePromise2.default();
  _this.subscriptions = new _map2.default();
  _this.state = CLIENT_STATE.INITIALIZED;
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Object"></a>[function <span class="apidocSignatureSpan">parse.</span>Object (className, attributes, options)](#apidoc.element.parse.Object)
- description and source-code
```javascript
function ParseObject(className, attributes, options) {
  (0, _classCallCheck3.default)(this, ParseObject);

  // Enable legacy initializers
  if (typeof this.initialize === 'function') {
    this.initialize.apply(this, arguments);
  }

  var toSet = null;
  this._objCount = objectCount++;
  if (typeof className === 'string') {
    this.className = className;
    if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
      toSet = attributes;
    }
  } else if (className && (typeof className === 'undefined' ? 'undefined' : (0, _typeof3.default)(className)) === 'object') {
    this.className = className.className;
    toSet = {};
    for (var attr in className) {
      if (attr !== 'className') {
        toSet[attr] = className[attr];
      }
    }
    if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
      options = attributes;
    }
  }
  if (toSet && !this.set(toSet, options)) {
    throw new Error('Can\'t create an invalid Parse Object');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Promise"></a>[function <span class="apidocSignatureSpan">parse.</span>Promise (executor)](#apidoc.element.parse.Promise)
- description and source-code
```javascript
function ParsePromise(executor) {
  (0, _classCallCheck3.default)(this, ParsePromise);

  this._resolved = false;
  this._rejected = false;
  this._resolvedCallbacks = [];
  this._rejectedCallbacks = [];

  if (typeof executor === 'function') {
    executor(this.resolve.bind(this), this.reject.bind(this));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Query"></a>[function <span class="apidocSignatureSpan">parse.</span>Query (objectClass)](#apidoc.element.parse.Query)
- description and source-code
```javascript
function ParseQuery(objectClass) {
  (0, _classCallCheck3.default)(this, ParseQuery);

  if (typeof objectClass === 'string') {
    if (objectClass === 'User' && _CoreManager2.default.get('PERFORM_USER_REWRITE')) {
      this.className = '_User';
    } else {
      this.className = objectClass;
    }
  } else if (objectClass instanceof _ParseObject2.default) {
    this.className = objectClass.className;
  } else if (typeof objectClass === 'function') {
    if (typeof objectClass.className === 'string') {
      this.className = objectClass.className;
    } else {
      var obj = new objectClass();
      this.className = obj.className;
    }
  } else {
    throw new TypeError('A ParseQuery must be constructed with a ParseObject or class name.');
  }

  this._where = {};
  this._include = [];
  this._limit = -1; // negative limit is not sent in the server request
  this._skip = 0;
  this._extraOptions = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Relation"></a>[function <span class="apidocSignatureSpan">parse.</span>Relation (parent, key)](#apidoc.element.parse.Relation)
- description and source-code
```javascript
function ParseRelation(parent, key) {
  (0, _classCallCheck3.default)(this, ParseRelation);

  this.parent = parent;
  this.key = key;
  this.targetClassName = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Role"></a>[function <span class="apidocSignatureSpan">parse.</span>Role (name, acl)](#apidoc.element.parse.Role)
- description and source-code
```javascript
function ParseRole(name, acl) {
  (0, _classCallCheck3.default)(this, ParseRole);

  var _this = (0, _possibleConstructorReturn3.default)(this, (ParseRole.__proto__ || (0, _getPrototypeOf2.default)(ParseRole)).call
(this, '_Role'));

  if (typeof name === 'string' && acl instanceof _ParseACL2.default) {
    _this.setName(name);
    _this.setACL(acl);
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Session"></a>[function <span class="apidocSignatureSpan">parse.</span>Session (attributes)](#apidoc.element.parse.Session)
- description and source-code
```javascript
function ParseSession(attributes) {
  (0, _classCallCheck3.default)(this, ParseSession);

  var _this = (0, _possibleConstructorReturn3.default)(this, (ParseSession.__proto__ || (0, _getPrototypeOf2.default)(ParseSession
)).call(this, '_Session'));

  if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
    if (!_this.set(attributes || {})) {
      throw new Error('Can\'t create an invalid Session');
    }
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.User"></a>[function <span class="apidocSignatureSpan">parse.</span>User (attributes)](#apidoc.element.parse.User)
- description and source-code
```javascript
function ParseUser(attributes) {
  (0, _classCallCheck3.default)(this, ParseUser);

  var _this = (0, _possibleConstructorReturn3.default)(this, (ParseUser.__proto__ || (0, _getPrototypeOf2.default)(ParseUser)).call
(this, '_User'));

  if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
    if (!_this.set(attributes || {})) {
      throw new Error('Can\'t create an invalid Parse User');
    }
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse._ajax"></a>[function <span class="apidocSignatureSpan">parse.</span>_ajax ()](#apidoc.element.parse._ajax)
- description and source-code
```javascript
_ajax = function () {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  return _CoreManager2.default.getRESTController().ajax.apply(null, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse._decode"></a>[function <span class="apidocSignatureSpan">parse.</span>_decode (_, value)](#apidoc.element.parse._decode)
- description and source-code
```javascript
_decode = function (_, value) {
  return (0, _decode2.default)(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse._encode"></a>[function <span class="apidocSignatureSpan">parse.</span>_encode (value, _, disallowObjects)](#apidoc.element.parse._encode)
- description and source-code
```javascript
_encode = function (value, _, disallowObjects) {
  return (0, _encode2.default)(value, disallowObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse._getInstallationId"></a>[function <span class="apidocSignatureSpan">parse.</span>_getInstallationId ()](#apidoc.element.parse._getInstallationId)
- description and source-code
```javascript
_getInstallationId = function () {
  return _CoreManager2.default.getInstallationController().currentInstallationId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse._initialize"></a>[function <span class="apidocSignatureSpan">parse.</span>_initialize (applicationId, javaScriptKey, masterKey)](#apidoc.element.parse._initialize)
- description and source-code
```javascript
_initialize = function (applicationId, javaScriptKey, masterKey) {
  _CoreManager2.default.set('APPLICATION_ID', applicationId);
  _CoreManager2.default.set('JAVASCRIPT_KEY', javaScriptKey);
  _CoreManager2.default.set('MASTER_KEY', masterKey);
  _CoreManager2.default.set('USE_MASTER_KEY', false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse._request"></a>[function <span class="apidocSignatureSpan">parse.</span>_request ()](#apidoc.element.parse._request)
- description and source-code
```javascript
_request = function () {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return _CoreManager2.default.getRESTController().request.apply(null, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.initialize"></a>[function <span class="apidocSignatureSpan">parse.</span>initialize (applicationId, javaScriptKey)](#apidoc.element.parse.initialize)
- description and source-code
```javascript
initialize = function (applicationId, javaScriptKey) {
  if ('browser' === 'browser' && _CoreManager2.default.get('IS_NODE')) {
    console.log('It looks like you\'re using the browser version of the SDK in a ' + 'node.js environment. You should require(\'
parse/node\') instead.');
  }
  Parse._initialize(applicationId, javaScriptKey);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.Analytics"></a>[module parse.Analytics](#apidoc.module.parse.Analytics)

#### <a name="apidoc.element.parse.Analytics.track"></a>[function <span class="apidocSignatureSpan">parse.Analytics.</span>track (name, dimensions, options)](#apidoc.element.parse.Analytics.track)
- description and source-code
```javascript
function track(name, dimensions, options) {
  name = name || '';
  name = name.replace(/^\s*/, '');
  name = name.replace(/\s*$/, '');
  if (name.length === 0) {
    throw new TypeError('A name for the custom event must be provided');
  }

  for (var key in dimensions) {
    if (typeof key !== 'string' || typeof dimensions[key] !== 'string') {
      throw new TypeError('track() dimensions expects keys and values of type "string".');
    }
  }

  options = options || {};
  return _CoreManager2.default.getAnalyticsController().track(name, dimensions)._thenRunCallbacks(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.Cloud"></a>[module parse.Cloud](#apidoc.module.parse.Cloud)

#### <a name="apidoc.element.parse.Cloud.run"></a>[function <span class="apidocSignatureSpan">parse.Cloud.</span>run (name, data, options)](#apidoc.element.parse.Cloud.run)
- description and source-code
```javascript
function run(name, data, options) {
  options = options || {};

  if (typeof name !== 'string' || name.length === 0) {
    throw new TypeError('Cloud function name must be a string.');
  }

  var requestOptions = {};
  if (options.useMasterKey) {
    requestOptions.useMasterKey = options.useMasterKey;
  }
  if (options.sessionToken) {
    requestOptions.sessionToken = options.sessionToken;
  }

  return _CoreManager2.default.getCloudController().run(name, data, requestOptions)._thenRunCallbacks(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.CoreManager"></a>[module parse.CoreManager](#apidoc.module.parse.CoreManager)

#### <a name="apidoc.element.parse.CoreManager.get"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>get (key)](#apidoc.element.parse.CoreManager.get)
- description and source-code
```javascript
get = function (key) {
  if (config.hasOwnProperty(key)) {
    return config[key];
  }
  throw new Error('Configuration key not found: ' + key);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getAnalyticsController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getAnalyticsController ()](#apidoc.element.parse.CoreManager.getAnalyticsController)
- description and source-code
```javascript
getAnalyticsController = function () {
  return config['AnalyticsController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getCloudController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getCloudController ()](#apidoc.element.parse.CoreManager.getCloudController)
- description and source-code
```javascript
getCloudController = function () {
  return config['CloudController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getConfigController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getConfigController ()](#apidoc.element.parse.CoreManager.getConfigController)
- description and source-code
```javascript
getConfigController = function () {
  return config['ConfigController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getFileController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getFileController ()](#apidoc.element.parse.CoreManager.getFileController)
- description and source-code
```javascript
getFileController = function () {
  return config['FileController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getHooksController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getHooksController ()](#apidoc.element.parse.CoreManager.getHooksController)
- description and source-code
```javascript
getHooksController = function () {
  return config['HooksController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getInstallationController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getInstallationController ()](#apidoc.element.parse.CoreManager.getInstallationController)
- description and source-code
```javascript
getInstallationController = function () {
  return config['InstallationController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getLiveQueryController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getLiveQueryController ()](#apidoc.element.parse.CoreManager.getLiveQueryController)
- description and source-code
```javascript
getLiveQueryController = function () {
  return config['LiveQueryController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getObjectController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getObjectController ()](#apidoc.element.parse.CoreManager.getObjectController)
- description and source-code
```javascript
getObjectController = function () {
  return config['ObjectController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getObjectStateController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getObjectStateController ()](#apidoc.element.parse.CoreManager.getObjectStateController)
- description and source-code
```javascript
getObjectStateController = function () {
  return config['ObjectStateController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getPushController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getPushController ()](#apidoc.element.parse.CoreManager.getPushController)
- description and source-code
```javascript
getPushController = function () {
  return config['PushController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getQueryController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getQueryController ()](#apidoc.element.parse.CoreManager.getQueryController)
- description and source-code
```javascript
getQueryController = function () {
  return config['QueryController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getRESTController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getRESTController ()](#apidoc.element.parse.CoreManager.getRESTController)
- description and source-code
```javascript
getRESTController = function () {
  return config['RESTController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getSessionController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getSessionController ()](#apidoc.element.parse.CoreManager.getSessionController)
- description and source-code
```javascript
getSessionController = function () {
  return config['SessionController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getStorageController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getStorageController ()](#apidoc.element.parse.CoreManager.getStorageController)
- description and source-code
```javascript
getStorageController = function () {
  return config['StorageController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.getUserController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>getUserController ()](#apidoc.element.parse.CoreManager.getUserController)
- description and source-code
```javascript
getUserController = function () {
  return config['UserController'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.set"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>set (key, value)](#apidoc.element.parse.CoreManager.set)
- description and source-code
```javascript
set = function (key, value) {
  config[key] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setAnalyticsController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setAnalyticsController (controller)](#apidoc.element.parse.CoreManager.setAnalyticsController)
- description and source-code
```javascript
setAnalyticsController = function (controller) {
  requireMethods('AnalyticsController', ['track'], controller);
  config['AnalyticsController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setCloudController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setCloudController (controller)](#apidoc.element.parse.CoreManager.setCloudController)
- description and source-code
```javascript
setCloudController = function (controller) {
  requireMethods('CloudController', ['run'], controller);
  config['CloudController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setConfigController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setConfigController (controller)](#apidoc.element.parse.CoreManager.setConfigController)
- description and source-code
```javascript
setConfigController = function (controller) {
  requireMethods('ConfigController', ['current', 'get'], controller);
  config['ConfigController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setFileController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setFileController (controller)](#apidoc.element.parse.CoreManager.setFileController)
- description and source-code
```javascript
setFileController = function (controller) {
  requireMethods('FileController', ['saveFile', 'saveBase64'], controller);
  config['FileController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setHooksController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setHooksController (controller)](#apidoc.element.parse.CoreManager.setHooksController)
- description and source-code
```javascript
setHooksController = function (controller) {
  requireMethods('HooksController', ['create', 'get', 'update', 'remove'], controller);
  config['HooksController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setInstallationController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setInstallationController (controller)](#apidoc.element.parse.CoreManager.setInstallationController)
- description and source-code
```javascript
setInstallationController = function (controller) {
  requireMethods('InstallationController', ['currentInstallationId'], controller);
  config['InstallationController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setLiveQueryController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setLiveQueryController (controller)](#apidoc.element.parse.CoreManager.setLiveQueryController)
- description and source-code
```javascript
setLiveQueryController = function (controller) {
  requireMethods('LiveQueryController', ['subscribe', 'unsubscribe', 'open', 'close'], controller);
  config['LiveQueryController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setObjectController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setObjectController (controller)](#apidoc.element.parse.CoreManager.setObjectController)
- description and source-code
```javascript
setObjectController = function (controller) {
  requireMethods('ObjectController', ['save', 'fetch', 'destroy'], controller);
  config['ObjectController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setObjectStateController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setObjectStateController (controller)](#apidoc.element.parse.CoreManager.setObjectStateController)
- description and source-code
```javascript
setObjectStateController = function (controller) {
  requireMethods('ObjectStateController', ['getState', 'initializeState', 'removeState', 'getServerData', 'setServerData', 'getPendingOps
', 'setPendingOp', 'pushPendingState', 'popPendingState', 'mergeFirstPendingState', 'getObjectCache', 'estimateAttribute', 'estimateAttributes
', 'commitServerChanges', 'enqueueTask', 'clearAllState'], controller);

  config['ObjectStateController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setPushController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setPushController (controller)](#apidoc.element.parse.CoreManager.setPushController)
- description and source-code
```javascript
setPushController = function (controller) {
  requireMethods('PushController', ['send'], controller);
  config['PushController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setQueryController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setQueryController (controller)](#apidoc.element.parse.CoreManager.setQueryController)
- description and source-code
```javascript
setQueryController = function (controller) {
  requireMethods('QueryController', ['find'], controller);
  config['QueryController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setRESTController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setRESTController (controller)](#apidoc.element.parse.CoreManager.setRESTController)
- description and source-code
```javascript
setRESTController = function (controller) {
  requireMethods('RESTController', ['request', 'ajax'], controller);
  config['RESTController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setSessionController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setSessionController (controller)](#apidoc.element.parse.CoreManager.setSessionController)
- description and source-code
```javascript
setSessionController = function (controller) {
  requireMethods('SessionController', ['getSession'], controller);
  config['SessionController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setStorageController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setStorageController (controller)](#apidoc.element.parse.CoreManager.setStorageController)
- description and source-code
```javascript
setStorageController = function (controller) {
  if (controller.async) {
    requireMethods('An async StorageController', ['getItemAsync', 'setItemAsync', 'removeItemAsync'], controller);
  } else {
    requireMethods('A synchronous StorageController', ['getItem', 'setItem', 'removeItem'], controller);
  }
  config['StorageController'] = controller;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.CoreManager.setUserController"></a>[function <span class="apidocSignatureSpan">parse.CoreManager.</span>setUserController (controller)](#apidoc.element.parse.CoreManager.setUserController)
- description and source-code
```javascript
setUserController = function (controller) {
  requireMethods('UserController', ['setCurrentUser', 'currentUser', 'currentUserAsync', 'signUp', 'logIn', 'become', 'logOut', '
requestPasswordReset', 'upgradeToRevocableSession', 'linkWith'], controller);
  config['UserController'] = controller;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.FacebookUtils"></a>[module parse.FacebookUtils](#apidoc.module.parse.FacebookUtils)

#### <a name="apidoc.element.parse.FacebookUtils.init"></a>[function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>init (options)](#apidoc.element.parse.FacebookUtils.init)
- description and source-code
```javascript
init = function (options) {
  if (typeof FB === 'undefined') {
    throw new Error('The Facebook JavaScript SDK must be loaded before calling init.');
  }
  initOptions = {};
  if (options) {
    for (var key in options) {
      initOptions[key] = options[key];
    }
  }
  if (initOptions.status && typeof console !== 'undefined') {
    var warn = console.warn || console.log || function () {};
    warn.call(console, 'The "status" flag passed into' + ' FB.init, when set to true, can interfere with Parse Facebook' + ' integration
, so it has been suppressed. Please call' + ' FB.getLoginStatus() explicitly if you require this behavior.');
  }
  initOptions.status = false;
  FB.init(initOptions);
  _ParseUser2.default._registerAuthenticationProvider(provider);
  initialized = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.FacebookUtils.isLinked"></a>[function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>isLinked (user)](#apidoc.element.parse.FacebookUtils.isLinked)
- description and source-code
```javascript
isLinked = function (user) {
  return user._isLinked('facebook');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.FacebookUtils.link"></a>[function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>link (user, permissions, options)](#apidoc.element.parse.FacebookUtils.link)
- description and source-code
```javascript
link = function (user, permissions, options) {
  if (!permissions || typeof permissions === 'string') {
    if (!initialized) {
      throw new Error('You must initialize FacebookUtils before calling link.');
    }
    requestedPermissions = permissions;
    return user._linkWith('facebook', options);
  } else {
    var newOptions = {};
    if (options) {
      for (var key in options) {
        newOptions[key] = options[key];
      }
    }
    newOptions.authData = permissions;
    return user._linkWith('facebook', newOptions);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.FacebookUtils.logIn"></a>[function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>logIn (permissions, options)](#apidoc.element.parse.FacebookUtils.logIn)
- description and source-code
```javascript
logIn = function (permissions, options) {
  if (!permissions || typeof permissions === 'string') {
    if (!initialized) {
      throw new Error('You must initialize FacebookUtils before calling logIn.');
    }
    requestedPermissions = permissions;
    return _ParseUser2.default._logInWith('facebook', options);
  } else {
    var newOptions = {};
    if (options) {
      for (var key in options) {
        newOptions[key] = options[key];
      }
    }
    newOptions.authData = permissions;
    return _ParseUser2.default._logInWith('facebook', newOptions);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.FacebookUtils.unlink"></a>[function <span class="apidocSignatureSpan">parse.FacebookUtils.</span>unlink (user, options)](#apidoc.element.parse.FacebookUtils.unlink)
- description and source-code
```javascript
unlink = function (user, options) {
  if (!initialized) {
    throw new Error('You must initialize FacebookUtils before calling unlink.');
  }
  return user._unlinkFrom('facebook', options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.LiveQuery"></a>[module parse.LiveQuery](#apidoc.module.parse.LiveQuery)

#### <a name="apidoc.element.parse.LiveQuery.close"></a>[function <span class="apidocSignatureSpan">parse.LiveQuery.</span>close ()](#apidoc.element.parse.LiveQuery.close)
- description and source-code
```javascript
function close() {
  var LiveQueryController = _CoreManager2.default.getLiveQueryController();
  LiveQueryController.close();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.LiveQuery.open"></a>[function <span class="apidocSignatureSpan">parse.LiveQuery.</span>open ()](#apidoc.element.parse.LiveQuery.open)
- description and source-code
```javascript
function open() {
  var LiveQueryController = _CoreManager2.default.getLiveQueryController();
  LiveQueryController.open();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.LiveQuery._events"></a>[module parse.LiveQuery._events](#apidoc.module.parse.LiveQuery._events)

#### <a name="apidoc.element.parse.LiveQuery._events.error"></a>[function <span class="apidocSignatureSpan">parse.LiveQuery._events.</span>error ()](#apidoc.element.parse.LiveQuery._events.error)
- description and source-code
```javascript
error = function () {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.Op"></a>[module parse.Op](#apidoc.module.parse.Op)

#### <a name="apidoc.element.parse.Op.Add"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>Add (value)](#apidoc.element.parse.Op.Add)
- description and source-code
```javascript
function AddOp(value) {
  (0, _classCallCheck3.default)(this, AddOp);

  var _this4 = (0, _possibleConstructorReturn3.default)(this, (AddOp.__proto__ || (0, _getPrototypeOf2.default)(AddOp)).call(this
));

  _this4._value = Array.isArray(value) ? value : [value];
  return _this4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Op.AddUnique"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>AddUnique (value)](#apidoc.element.parse.Op.AddUnique)
- description and source-code
```javascript
function AddUniqueOp(value) {
  (0, _classCallCheck3.default)(this, AddUniqueOp);

  var _this5 = (0, _possibleConstructorReturn3.default)(this, (AddUniqueOp.__proto__ || (0, _getPrototypeOf2.default)(AddUniqueOp
)).call(this));

  _this5._value = (0, _unique2.default)(Array.isArray(value) ? value : [value]);
  return _this5;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Op.Increment"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>Increment (amount)](#apidoc.element.parse.Op.Increment)
- description and source-code
```javascript
function IncrementOp(amount) {
  (0, _classCallCheck3.default)(this, IncrementOp);

  var _this3 = (0, _possibleConstructorReturn3.default)(this, (IncrementOp.__proto__ || (0, _getPrototypeOf2.default)(IncrementOp
)).call(this));

  if (typeof amount !== 'number') {
    throw new TypeError('Increment Op must be initialized with a numeric amount.');
  }
  _this3._amount = amount;
  return _this3;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Op.Relation"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>Relation (adds, removes)](#apidoc.element.parse.Op.Relation)
- description and source-code
```javascript
function RelationOp(adds, removes) {
  (0, _classCallCheck3.default)(this, RelationOp);

  var _this7 = (0, _possibleConstructorReturn3.default)(this, (RelationOp.__proto__ || (0, _getPrototypeOf2.default)(RelationOp)).
call(this));

  _this7._targetClassName = null;

  if (Array.isArray(adds)) {
    _this7.relationsToAdd = (0, _unique2.default)(adds.map(_this7._extractId, _this7));
  }

  if (Array.isArray(removes)) {
    _this7.relationsToRemove = (0, _unique2.default)(removes.map(_this7._extractId, _this7));
  }
  return _this7;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Op.Remove"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>Remove (value)](#apidoc.element.parse.Op.Remove)
- description and source-code
```javascript
function RemoveOp(value) {
  (0, _classCallCheck3.default)(this, RemoveOp);

  var _this6 = (0, _possibleConstructorReturn3.default)(this, (RemoveOp.__proto__ || (0, _getPrototypeOf2.default)(RemoveOp)).call
(this));

  _this6._value = (0, _unique2.default)(Array.isArray(value) ? value : [value]);
  return _this6;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Op.Set"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>Set (value)](#apidoc.element.parse.Op.Set)
- description and source-code
```javascript
function SetOp(value) {
  (0, _classCallCheck3.default)(this, SetOp);

  var _this = (0, _possibleConstructorReturn3.default)(this, (SetOp.__proto__ || (0, _getPrototypeOf2.default)(SetOp)).call(this
));

  _this._value = value;
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Op.Unset"></a>[function <span class="apidocSignatureSpan">parse.Op.</span>Unset ()](#apidoc.element.parse.Op.Unset)
- description and source-code
```javascript
function UnsetOp() {
  (0, _classCallCheck3.default)(this, UnsetOp);
  return (0, _possibleConstructorReturn3.default)(this, (UnsetOp.__proto__ || (0, _getPrototypeOf2.default)(UnsetOp)).apply(this
, arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.Push"></a>[module parse.Push](#apidoc.module.parse.Push)

#### <a name="apidoc.element.parse.Push.send"></a>[function <span class="apidocSignatureSpan">parse.Push.</span>send (data, options)](#apidoc.element.parse.Push.send)
- description and source-code
```javascript
function send(data, options) {
  options = options || {};

  if (data.where && data.where instanceof _ParseQuery2.default) {
    data.where = data.where.toJSON().where;
  }

  if (data.push_time && (0, _typeof3.default)(data.push_time) === 'object') {
    data.push_time = data.push_time.toJSON();
  }

  if (data.expiration_time && (0, _typeof3.default)(data.expiration_time) === 'object') {
    data.expiration_time = data.expiration_time.toJSON();
  }

  if (data.expiration_time && data.expiration_interval) {
    throw new Error('expiration_time and expiration_interval cannot both be set.');
  }

  return _CoreManager2.default.getPushController().send(data, {
    useMasterKey: options.useMasterKey
  })._thenRunCallbacks(options);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.Storage"></a>[module parse.Storage](#apidoc.module.parse.Storage)

#### <a name="apidoc.element.parse.Storage._clear"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>_clear ()](#apidoc.element.parse.Storage._clear)
- description and source-code
```javascript
_clear = function () {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.hasOwnProperty('clear')) {
    controller.clear();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.async"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>async ()](#apidoc.element.parse.Storage.async)
- description and source-code
```javascript
async = function () {
  var controller = _CoreManager2.default.getStorageController();
  return !!controller.async;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.generatePath"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>generatePath (path)](#apidoc.element.parse.Storage.generatePath)
- description and source-code
```javascript
generatePath = function (path) {
  if (!_CoreManager2.default.get('APPLICATION_ID')) {
    throw new Error('You need to call Parse.initialize before using Parse.');
  }
  if (typeof path !== 'string') {
    throw new Error('Tried to get a Storage path that was not a String.');
  }
  if (path[0] === '/') {
    path = path.substr(1);
  }
  return 'Parse/' + _CoreManager2.default.get('APPLICATION_ID') + '/' + path;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.getItem"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>getItem (path)](#apidoc.element.parse.Storage.getItem)
- description and source-code
```javascript
getItem = function (path) {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.async === 1) {
    throw new Error('Synchronous storage is not supported by the current storage controller');
  }
  return controller.getItem(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.getItemAsync"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>getItemAsync (path)](#apidoc.element.parse.Storage.getItemAsync)
- description and source-code
```javascript
getItemAsync = function (path) {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.async === 1) {
    return controller.getItemAsync(path);
  }
  return _ParsePromise2.default.as(controller.getItem(path));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.removeItem"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>removeItem (path)](#apidoc.element.parse.Storage.removeItem)
- description and source-code
```javascript
removeItem = function (path) {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.async === 1) {
    throw new Error('Synchronous storage is not supported by the current storage controller');
  }
  return controller.removeItem(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.removeItemAsync"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>removeItemAsync (path)](#apidoc.element.parse.Storage.removeItemAsync)
- description and source-code
```javascript
removeItemAsync = function (path) {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.async === 1) {
    return controller.removeItemAsync(path);
  }
  return _ParsePromise2.default.as(controller.removeItem(path));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.setItem"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>setItem (path, value)](#apidoc.element.parse.Storage.setItem)
- description and source-code
```javascript
setItem = function (path, value) {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.async === 1) {
    throw new Error('Synchronous storage is not supported by the current storage controller');
  }
  return controller.setItem(path, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.Storage.setItemAsync"></a>[function <span class="apidocSignatureSpan">parse.Storage.</span>setItemAsync (path, value)](#apidoc.element.parse.Storage.setItemAsync)
- description and source-code
```javascript
setItemAsync = function (path, value) {
  var controller = _CoreManager2.default.getStorageController();
  if (controller.async === 1) {
    return controller.setItemAsync(path, value);
  }
  return _ParsePromise2.default.as(controller.setItem(path, value));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.parse.node"></a>[module parse.node](#apidoc.module.parse.node)

#### <a name="apidoc.element.parse.node.ACL"></a>[function <span class="apidocSignatureSpan">parse.node.</span>ACL (arg1)](#apidoc.element.parse.node.ACL)
- description and source-code
```javascript
function ParseACL(arg1) {
  (0, _classCallCheck3.default)(this, ParseACL);

  this.permissionsById = {};
  if (arg1 && (typeof arg1 === 'undefined' ? 'undefined' : (0, _typeof3.default)(arg1)) === 'object') {
    if (arg1 instanceof _ParseUser2.default) {
      this.setReadAccess(arg1, true);
      this.setWriteAccess(arg1, true);
    } else {
      for (var userId in arg1) {
        var accessList = arg1[userId];
        if (typeof userId !== 'string') {
          throw new TypeError('Tried to create an ACL with an invalid user id.');
        }
        this.permissionsById[userId] = {};
        for (var permission in accessList) {
          var allowed = accessList[permission];
          if (permission !== 'read' && permission !== 'write') {
            throw new TypeError('Tried to create an ACL with an invalid permission type.');
          }
          if (typeof allowed !== 'boolean') {
            throw new TypeError('Tried to create an ACL with an invalid permission value.');
          }
          this.permissionsById[userId][permission] = allowed;
        }
      }
    }
  } else if (typeof arg1 === 'function') {
    throw new TypeError('ParseACL constructed with a function. Did you forget ()?');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Config"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Config ()](#apidoc.element.parse.node.Config)
- description and source-code
```javascript
function ParseConfig() {
  (0, _classCallCheck3.default)(this, ParseConfig);

  this.attributes = {};
  this._escapedAttributes = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Error"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Error (code, message)](#apidoc.element.parse.node.Error)
- description and source-code
```javascript
function ParseError(code, message) {
  (0, _classCallCheck3.default)(this, ParseError);

  this.code = code;
  this.message = message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.File"></a>[function <span class="apidocSignatureSpan">parse.node.</span>File (name, data, type)](#apidoc.element.parse.node.File)
- description and source-code
```javascript
function ParseFile(name, data, type) {
  (0, _classCallCheck3.default)(this, ParseFile);

  var specifiedType = type || '';

  this._name = name;

  if (data !== undefined) {
    if (Array.isArray(data)) {
      this._source = {
        format: 'base64',
        base64: ParseFile.encodeBase64(data),
        type: specifiedType
      };
    } else if (typeof File !== 'undefined' && data instanceof File) {
      this._source = {
        format: 'file',
        file: data,
        type: specifiedType
      };
    } else if (data && typeof data.base64 === 'string') {
      var _base = data.base64;
      var commaIndex = _base.indexOf(',');

      if (commaIndex !== -1) {
        var matches = dataUriRegexp.exec(_base.slice(0, commaIndex + 1));
        // if data URI with type and charset, there will be 4 matches.
        this._source = {
          format: 'base64',
          base64: _base.slice(commaIndex + 1),
          type: matches[1]
        };
      } else {
        this._source = {
          format: 'base64',
          base64: _base,
          type: specifiedType
        };
      }
    } else {
      throw new TypeError('Cannot create a Parse.File with that data.');
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.GeoPoint"></a>[function <span class="apidocSignatureSpan">parse.node.</span>GeoPoint (arg1, arg2)](#apidoc.element.parse.node.GeoPoint)
- description and source-code
```javascript
function ParseGeoPoint(arg1, arg2) {
  (0, _classCallCheck3.default)(this, ParseGeoPoint);

  if (Array.isArray(arg1)) {
    ParseGeoPoint._validate(arg1[0], arg1[1]);
    this._latitude = arg1[0];
    this._longitude = arg1[1];
  } else if ((typeof arg1 === 'undefined' ? 'undefined' : (0, _typeof3.default)(arg1)) === 'object') {
    ParseGeoPoint._validate(arg1.latitude, arg1.longitude);
    this._latitude = arg1.latitude;
    this._longitude = arg1.longitude;
  } else if (typeof arg1 === 'number' && typeof arg2 === 'number') {
    ParseGeoPoint._validate(arg1, arg2);
    this._latitude = arg1;
    this._longitude = arg2;
  } else {
    this._latitude = 0;
    this._longitude = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Installation"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Installation (attributes)](#apidoc.element.parse.node.Installation)
- description and source-code
```javascript
function Installation(attributes) {
  (0, _classCallCheck3.default)(this, Installation);

  var _this = (0, _possibleConstructorReturn3.default)(this, (Installation.__proto__ || (0, _getPrototypeOf2.default)(Installation
)).call(this, '_Installation'));

  if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
    if (!_this.set(attributes || {})) {
      throw new Error('Can\'t create an invalid Session');
    }
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.LiveQueryClient"></a>[function <span class="apidocSignatureSpan">parse.node.</span>LiveQueryClient (_ref)](#apidoc.element.parse.node.LiveQueryClient)
- description and source-code
```javascript
function LiveQueryClient(_ref) {
  var applicationId = _ref.applicationId;
  var serverURL = _ref.serverURL;
  var javascriptKey = _ref.javascriptKey;
  var masterKey = _ref.masterKey;
  var sessionToken = _ref.sessionToken;
  (0, _classCallCheck3.default)(this, LiveQueryClient);

  var _this = (0, _possibleConstructorReturn3.default)(this, (LiveQueryClient.__proto__ || (0, _getPrototypeOf2.default)(LiveQueryClient
)).call(this));

  if (!serverURL || serverURL.indexOf('ws') !== 0) {
    throw new Error('You need to set a proper Parse LiveQuery server url before using LiveQueryClient');
  }

  _this.reconnectHandle = null;
  _this.attempts = 1;;
  _this.id = 0;
  _this.requestId = 1;
  _this.serverURL = serverURL;
  _this.applicationId = applicationId;
  _this.javascriptKey = javascriptKey;
  _this.masterKey = masterKey;
  _this.sessionToken = sessionToken;
  _this.connectPromise = new _ParsePromise2.default();
  _this.subscriptions = new _map2.default();
  _this.state = CLIENT_STATE.INITIALIZED;
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Object"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Object (className, attributes, options)](#apidoc.element.parse.node.Object)
- description and source-code
```javascript
function ParseObject(className, attributes, options) {
  (0, _classCallCheck3.default)(this, ParseObject);

  // Enable legacy initializers
  if (typeof this.initialize === 'function') {
    this.initialize.apply(this, arguments);
  }

  var toSet = null;
  this._objCount = objectCount++;
  if (typeof className === 'string') {
    this.className = className;
    if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
      toSet = attributes;
    }
  } else if (className && (typeof className === 'undefined' ? 'undefined' : (0, _typeof3.default)(className)) === 'object') {
    this.className = className.className;
    toSet = {};
    for (var attr in className) {
      if (attr !== 'className') {
        toSet[attr] = className[attr];
      }
    }
    if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
      options = attributes;
    }
  }
  if (toSet && !this.set(toSet, options)) {
    throw new Error('Can\'t create an invalid Parse Object');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Promise"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Promise (executor)](#apidoc.element.parse.node.Promise)
- description and source-code
```javascript
function ParsePromise(executor) {
  (0, _classCallCheck3.default)(this, ParsePromise);

  this._resolved = false;
  this._rejected = false;
  this._resolvedCallbacks = [];
  this._rejectedCallbacks = [];

  if (typeof executor === 'function') {
    executor(this.resolve.bind(this), this.reject.bind(this));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Query"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Query (objectClass)](#apidoc.element.parse.node.Query)
- description and source-code
```javascript
function ParseQuery(objectClass) {
  (0, _classCallCheck3.default)(this, ParseQuery);

  if (typeof objectClass === 'string') {
    if (objectClass === 'User' && _CoreManager2.default.get('PERFORM_USER_REWRITE')) {
      this.className = '_User';
    } else {
      this.className = objectClass;
    }
  } else if (objectClass instanceof _ParseObject2.default) {
    this.className = objectClass.className;
  } else if (typeof objectClass === 'function') {
    if (typeof objectClass.className === 'string') {
      this.className = objectClass.className;
    } else {
      var obj = new objectClass();
      this.className = obj.className;
    }
  } else {
    throw new TypeError('A ParseQuery must be constructed with a ParseObject or class name.');
  }

  this._where = {};
  this._include = [];
  this._limit = -1; // negative limit is not sent in the server request
  this._skip = 0;
  this._extraOptions = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Relation"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Relation (parent, key)](#apidoc.element.parse.node.Relation)
- description and source-code
```javascript
function ParseRelation(parent, key) {
  (0, _classCallCheck3.default)(this, ParseRelation);

  this.parent = parent;
  this.key = key;
  this.targetClassName = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Role"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Role (name, acl)](#apidoc.element.parse.node.Role)
- description and source-code
```javascript
function ParseRole(name, acl) {
  (0, _classCallCheck3.default)(this, ParseRole);

  var _this = (0, _possibleConstructorReturn3.default)(this, (ParseRole.__proto__ || (0, _getPrototypeOf2.default)(ParseRole)).call
(this, '_Role'));

  if (typeof name === 'string' && acl instanceof _ParseACL2.default) {
    _this.setName(name);
    _this.setACL(acl);
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.Session"></a>[function <span class="apidocSignatureSpan">parse.node.</span>Session (attributes)](#apidoc.element.parse.node.Session)
- description and source-code
```javascript
function ParseSession(attributes) {
  (0, _classCallCheck3.default)(this, ParseSession);

  var _this = (0, _possibleConstructorReturn3.default)(this, (ParseSession.__proto__ || (0, _getPrototypeOf2.default)(ParseSession
)).call(this, '_Session'));

  if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
    if (!_this.set(attributes || {})) {
      throw new Error('Can\'t create an invalid Session');
    }
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.User"></a>[function <span class="apidocSignatureSpan">parse.node.</span>User (attributes)](#apidoc.element.parse.node.User)
- description and source-code
```javascript
function ParseUser(attributes) {
  (0, _classCallCheck3.default)(this, ParseUser);

  var _this = (0, _possibleConstructorReturn3.default)(this, (ParseUser.__proto__ || (0, _getPrototypeOf2.default)(ParseUser)).call
(this, '_User'));

  if (attributes && (typeof attributes === 'undefined' ? 'undefined' : (0, _typeof3.default)(attributes)) === 'object') {
    if (!_this.set(attributes || {})) {
      throw new Error('Can\'t create an invalid Parse User');
    }
  }
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node._ajax"></a>[function <span class="apidocSignatureSpan">parse.node.</span>_ajax ()](#apidoc.element.parse.node._ajax)
- description and source-code
```javascript
_ajax = function () {
  for (var _len2 = arguments.length, args = Array(_len2), _key2 = 0; _key2 < _len2; _key2++) {
    args[_key2] = arguments[_key2];
  }

  return _CoreManager2.default.getRESTController().ajax.apply(null, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node._decode"></a>[function <span class="apidocSignatureSpan">parse.node.</span>_decode (_, value)](#apidoc.element.parse.node._decode)
- description and source-code
```javascript
_decode = function (_, value) {
  return (0, _decode2.default)(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node._encode"></a>[function <span class="apidocSignatureSpan">parse.node.</span>_encode (value, _, disallowObjects)](#apidoc.element.parse.node._encode)
- description and source-code
```javascript
_encode = function (value, _, disallowObjects) {
  return (0, _encode2.default)(value, disallowObjects);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node._getInstallationId"></a>[function <span class="apidocSignatureSpan">parse.node.</span>_getInstallationId ()](#apidoc.element.parse.node._getInstallationId)
- description and source-code
```javascript
_getInstallationId = function () {
  return _CoreManager2.default.getInstallationController().currentInstallationId();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node._initialize"></a>[function <span class="apidocSignatureSpan">parse.node.</span>_initialize (applicationId, javaScriptKey, masterKey)](#apidoc.element.parse.node._initialize)
- description and source-code
```javascript
_initialize = function (applicationId, javaScriptKey, masterKey) {
  _CoreManager2.default.set('APPLICATION_ID', applicationId);
  _CoreManager2.default.set('JAVASCRIPT_KEY', javaScriptKey);
  _CoreManager2.default.set('MASTER_KEY', masterKey);
  _CoreManager2.default.set('USE_MASTER_KEY', false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node._request"></a>[function <span class="apidocSignatureSpan">parse.node.</span>_request ()](#apidoc.element.parse.node._request)
- description and source-code
```javascript
_request = function () {
  for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {
    args[_key] = arguments[_key];
  }

  return _CoreManager2.default.getRESTController().request.apply(null, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.parse.node.initialize"></a>[function <span class="apidocSignatureSpan">parse.node.</span>initialize (applicationId, javaScriptKey, masterKey)](#apidoc.element.parse.node.initialize)
- description and source-code
```javascript
initialize = function (applicationId, javaScriptKey, masterKey) {
  _CoreManager2.default.set('APPLICATION_ID', applicationId);
  _CoreManager2.default.set('JAVASCRIPT_KEY', javaScriptKey);
  _CoreManager2.default.set('MASTER_KEY', masterKey);
  _CoreManager2.default.set('USE_MASTER_KEY', false);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
