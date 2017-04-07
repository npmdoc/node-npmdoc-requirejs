# api documentation for  [requirejs (v2.3.3)](http://github.com/jrburke/r.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-requirejs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-requirejs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-requirejs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-requirejs)
#### Node adapter for RequireJS, for loading AMD modules. Includes RequireJS optimizer

[![NPM](https://nodei.co/npm/requirejs.png?downloads=true)](https://www.npmjs.com/package/requirejs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-requirejs/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-requirejs%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-requirejs/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-requirejs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-requirejs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Burke",
        "email": "jrburke@gmail.com",
        "url": "http://github.com/jrburke"
    },
    "bin": {
        "r.js": "./bin/r.js",
        "r_js": "./bin/r.js"
    },
    "bugs": {
        "url": "https://github.com/jrburke/r.js/issues"
    },
    "dependencies": {},
    "description": "Node adapter for RequireJS, for loading AMD modules. Includes RequireJS optimizer",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "aa59fd3a0287eaf407959a138228044b5dd6a6a3",
        "tarball": "https://registry.npmjs.org/requirejs/-/requirejs-2.3.3.tgz"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "homepage": "http://github.com/jrburke/r.js",
    "license": "MIT",
    "main": "./bin/r.js",
    "maintainers": [
        {
            "name": "jrburke",
            "email": "jrburke@gmail.com"
        }
    ],
    "name": "requirejs",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jrburke/r.js.git"
    },
    "scripts": {},
    "version": "2.3.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module requirejs](#apidoc.module.requirejs)
1.  boolean <span class="apidocSignatureSpan">requirejs.</span>isBrowser
1.  [function <span class="apidocSignatureSpan">requirejs.</span>config (config)](#apidoc.element.requirejs.config)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>createNode (config, moduleName, url)](#apidoc.element.requirejs.createNode)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>define (name, deps, callback)](#apidoc.element.requirejs.define)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>defined ()](#apidoc.element.requirejs.defined)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>exec (text)](#apidoc.element.requirejs.exec)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>get (context, moduleName, relModuleMap, localRequire)](#apidoc.element.requirejs.get)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>load (context, moduleName, url)](#apidoc.element.requirejs.load)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>makeNodeWrapper (contents)](#apidoc.element.requirejs.makeNodeWrapper)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>nextTick (fn)](#apidoc.element.requirejs.nextTick)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>nodeRequire (path)](#apidoc.element.requirejs.nodeRequire)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>onError (err)](#apidoc.element.requirejs.onError)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>optimize (config, callback, errback)](#apidoc.element.requirejs.optimize)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>specified ()](#apidoc.element.requirejs.specified)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>toUrl ()](#apidoc.element.requirejs.toUrl)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>undef ()](#apidoc.element.requirejs.undef)
1.  object <span class="apidocSignatureSpan">requirejs.</span>jsExtRegExp
1.  object <span class="apidocSignatureSpan">requirejs.</span>nodeRequire.extensions
1.  object <span class="apidocSignatureSpan">requirejs.</span>s
1.  object <span class="apidocSignatureSpan">requirejs.</span>tools
1.  string <span class="apidocSignatureSpan">requirejs.</span>version

#### [module requirejs.nodeRequire](#apidoc.module.requirejs.nodeRequire)
1.  [function <span class="apidocSignatureSpan">requirejs.</span>nodeRequire (path)](#apidoc.element.requirejs.nodeRequire.nodeRequire)
1.  [function <span class="apidocSignatureSpan">requirejs.nodeRequire.</span>resolve (request)](#apidoc.element.requirejs.nodeRequire.resolve)
1.  object <span class="apidocSignatureSpan">requirejs.nodeRequire.</span>cache
1.  object <span class="apidocSignatureSpan">requirejs.nodeRequire.</span>extensions
1.  object <span class="apidocSignatureSpan">requirejs.nodeRequire.</span>main

#### [module requirejs.nodeRequire.extensions](#apidoc.module.requirejs.nodeRequire.extensions)

#### [module requirejs.s](#apidoc.module.requirejs.s)
1.  [function <span class="apidocSignatureSpan">requirejs.s.</span>newContext (contextName)](#apidoc.element.requirejs.s.newContext)
1.  object <span class="apidocSignatureSpan">requirejs.s.</span>contexts

#### [module requirejs.tools](#apidoc.module.requirejs.tools)
1.  [function <span class="apidocSignatureSpan">requirejs.tools.</span>useLib (contextName, callback)](#apidoc.element.requirejs.tools.useLib)



# <a name="apidoc.module.requirejs"></a>[module requirejs](#apidoc.module.requirejs)

#### <a name="apidoc.element.requirejs.config"></a>[function <span class="apidocSignatureSpan">requirejs.</span>config (config)](#apidoc.element.requirejs.config)
- description and source-code
```javascript
config = function (config) {
    return req(config);
}
```
- example usage
```shell
...
        context.configure(config);
    }

    return context.require(deps, callback, errback);
};

/**
 * Support require.config() to make it easier to cooperate with other
 * AMD loaders on globally agreed names.
 */
req.config = function (config) {
    return req(config);
};

/**
...
```

#### <a name="apidoc.element.requirejs.createNode"></a>[function <span class="apidocSignatureSpan">requirejs.</span>createNode (config, moduleName, url)](#apidoc.element.requirejs.createNode)
- description and source-code
```javascript
createNode = function (config, moduleName, url) {
    var node = config.xhtml ?
            document.createElementNS('http://www.w3.org/1999/xhtml', 'html:script') :
            document.createElement('script');
    node.type = config.scriptType || 'text/javascript';
    node.charset = 'utf-8';
    node.async = true;
    return node;
}
```
- example usage
```shell
...
     * @param {Object} url the URL to the module.
     */
    req.load = function (context, moduleName, url) {
        var config = (context && context.config) || {},
node;
        if (isBrowser) {
//In the browser so use a script tag
node = req.createNode(config, moduleName, url);

node.setAttribute('data-requirecontext', context.contextName);
node.setAttribute('data-requiremodule', moduleName);

//Set up load listener. Test attachEvent first because IE9 has
//a subtle issue in its addEventListener and script onload firings
//that do not match the behavior of all other browsers with
...
```

#### <a name="apidoc.element.requirejs.define"></a>[function <span class="apidocSignatureSpan">requirejs.</span>define (name, deps, callback)](#apidoc.element.requirejs.define)
- description and source-code
```javascript
define = function (name, deps, callback) {
    var node, context;

    //Allow for anonymous modules
    if (typeof name !== 'string') {
        //Adjust args appropriately
        callback = deps;
        deps = name;
        name = null;
    }

    //This module may not have dependencies
    if (!isArray(deps)) {
        callback = deps;
        deps = null;
    }

    //If no name, and callback is a function, then figure out if it a
    //CommonJS thing with dependencies.
    if (!deps && isFunction(callback)) {
        deps = [];
        //Remove comments from the callback string,
        //look for require calls, and pull them into the dependencies,
        //but only if there are function args.
        if (callback.length) {
            callback
                .toString()
                .replace(commentRegExp, commentReplace)
                .replace(cjsRequireRegExp, function (match, dep) {
                    deps.push(dep);
                });

            //May be a CommonJS thing even without require calls, but still
            //could use exports, and module. Avoid doing exports and module
            //work though if it just needs require.
            //REQUIRES the function to expect the CommonJS variables in the
            //order listed below.
            deps = (callback.length === 1 ? ['require'] : ['require', 'exports', 'module']).concat(deps);
        }
    }

    //If in IE 6-8 and hit an anonymous define() call, do the interactive
    //work.
    if (useInteractive) {
        node = currentlyAddingScript || getInteractiveScript();
        if (node) {
            if (!name) {
                name = node.getAttribute('data-requiremodule');
            }
            context = contexts[node.getAttribute('data-requirecontext')];
        }
    }

    //Always save off evaluating the def call until the script onload handler.
    //This allows multiple modules to be in a file without prematurely
    //tracing dependencies, and allows for anonymous module support,
    //where the module name is not known until the script onload event
    //occurs. If no context, use the global queue, and get it processed
    //in the onscript load callback.
    if (context) {
        context.defQueue.push([name, deps, callback]);
        context.defQueueMap[name] = true;
    } else {
        globalDefQueue.push([name, deps, callback]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.defined"></a>[function <span class="apidocSignatureSpan">requirejs.</span>defined ()](#apidoc.element.requirejs.defined)
- description and source-code
```javascript
defined = function () {
    var ctx = contexts[defContextName];
    return ctx.require[prop].apply(ctx, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.exec"></a>[function <span class="apidocSignatureSpan">requirejs.</span>exec (text)](#apidoc.element.requirejs.exec)
- description and source-code
```javascript
exec = function (text) {
<span class="apidocCodeCommentSpan">    /*jslint evil: true */
</span>    text = req.makeNodeWrapper(text);
    return eval(text);
}
```
- example usage
```shell
...


/** vim: et:ts=4:sw=4:sts=4
 * @license RequireJS 2.3.3 Copyright jQuery Foundation and other contributors.
 * Released under MIT license, https://github.com/requirejs/requirejs/blob/master/LICENSE
 */
//Not using strict: uneven strict support in browsers, #392, and causes
//problems with requirejs.exec()/transpiler plugins that may not be strict.
/*jslint regexp: true, nomen: true, sloppy: true */
/*global window, navigator, document, importScripts, setTimeout, opera */

var requirejs, require, define;
(function (global, setTimeout) {
var req, s, head, baseElement, dataMain, src,
    interactiveScript, currentlyAddingScript, mainScript, subPath,
...
```

#### <a name="apidoc.element.requirejs.get"></a>[function <span class="apidocSignatureSpan">requirejs.</span>get (context, moduleName, relModuleMap, localRequire)](#apidoc.element.requirejs.get)
- description and source-code
```javascript
get = function (context, moduleName, relModuleMap, localRequire) {
    if (moduleName === "require" || moduleName === "exports" || moduleName === "module") {
        context.onError(makeError("Explicit require of " + moduleName + " is not allowed.", moduleName));
    }

    var ret, oldTick,
        moduleMap = context.makeModuleMap(moduleName, relModuleMap, false, true);

    //Normalize module name, if it contains . or ..
    moduleName = moduleMap.id;

    if (hasProp(context.defined, moduleName)) {
        ret = context.defined[moduleName];
    } else {
        if (ret === undefined) {
            //Make sure nextTick for this type of call is sync-based.
            oldTick = context.nextTick;
            context.nextTick = syncTick;
            try {
                if (moduleMap.prefix) {
                    //A plugin, call requirejs to handle it. Now that
                    //nextTick is syncTick, the require will complete
                    //synchronously.
                    localRequire([moduleMap.originalName]);

                    //Now that plugin is loaded, can regenerate the moduleMap
                    //to get the final, normalized ID.
                    moduleMap = context.makeModuleMap(moduleMap.originalName, relModuleMap, false, true);
                    moduleName = moduleMap.id;
                } else {
                    //Try to dynamically fetch it.
                    req.load(context, moduleName, moduleMap.url);

                    //Enable the module
                    context.enable(moduleMap, relModuleMap);
                }

                //Break any cycles by requiring it normally, but this will
                //finish synchronously
                context.require([moduleName]);

                //The above calls are sync, so can do the next thing safely.
                ret = context.defined[moduleName];
            } finally {
                context.nextTick = oldTick;
            }
        }
    }

    return ret;
}
```
- example usage
```shell
...
if (relMap && hasProp(handlers, deps)) {
    return handlers[deps](registry[relMap.id]);
}

//Synchronous access to one module. If require.get is
//available (as in the Node adapter), prefer that.
if (req.get) {
    return req.get(context, deps, relMap, localRequire);
}

//Normalize module name, if it contains . or ..
map = makeModuleMap(deps, relMap, false, true);
id = map.id;

if (!hasProp(defined, id)) {
...
```

#### <a name="apidoc.element.requirejs.load"></a>[function <span class="apidocSignatureSpan">requirejs.</span>load (context, moduleName, url)](#apidoc.element.requirejs.load)
- description and source-code
```javascript
load = function (context, moduleName, url) {
    var contents, err,
        config = context.config;

    if (config.shim[moduleName] && (!config.suppress || !config.suppress.nodeShim)) {
        console.warn('Shim config not supported in Node, may or may not work. Detected ' +
                        'for module: ' + moduleName);
    }

    if (exists(url)) {
        contents = fs.readFileSync(url, 'utf8');

        contents = req.makeNodeWrapper(contents);
        try {
            vm.runInThisContext(contents, fs.realpathSync(url));
        } catch (e) {
            err = new Error('Evaluating ' + url + ' as module "' +
                            moduleName + '" failed with error: ' + e);
            err.originalError = e;
            err.moduleName = moduleName;
            err.requireModules = [moduleName];
            err.fileName = url;
            return context.onError(err);
        }
    } else {
        def(moduleName, function () {
            //Get the original name, since relative requires may be
            //resolved differently in node (issue #202). Also, if relative,
            //make it relative to the URL of the item requesting it
            //(issue #393)
            var dirName,
                map = hasProp(context.registry, moduleName) &&
                        context.registry[moduleName].map,
                parentMap = map && map.parentMap,
                originalName = map && map.originalName;

            if (originalName.charAt(0) === '.' && parentMap) {
                dirName = parentMap.url.split('/');
                dirName.pop();
                originalName = dirName.join('/') + '/' + originalName;
            }

            try {
                return (context.config.nodeRequire || req.nodeRequire)(originalName);
            } catch (e) {
                err = new Error('Tried loading "' + moduleName + '" at ' +
                                 url + ' then tried node\'s require("' +
                                    originalName + '") and it failed ' +
                                 'with error: ' + e);
                err.originalError = e;
                err.moduleName = originalName;
                err.requireModules = [moduleName];
                throw err;
            }
        });
    }

    //Support anonymous modules.
    context.completeLoad(moduleName);
}
```
- example usage
```shell
...

    //If the manager is for a plugin managed resource,
    //ask the plugin to load it now.
    if (this.shim) {
        context.makeRequire(this.map, {
            enableBuildCallback: true
        })(this.shim.deps || [], bind(this, function () {
            return map.prefix ? this.callPlugin() : this.load();
        }));
    } else {
        //Regular dependency.
        return map.prefix ? this.callPlugin() : this.load();
    }
},
...
```

#### <a name="apidoc.element.requirejs.makeNodeWrapper"></a>[function <span class="apidocSignatureSpan">requirejs.</span>makeNodeWrapper (contents)](#apidoc.element.requirejs.makeNodeWrapper)
- description and source-code
```javascript
makeNodeWrapper = function (contents) {
    return '(function (require, requirejs, define) { ' +
            contents +
            '\n}(requirejsVars.require, requirejsVars.requirejs, requirejsVars.define));';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.nextTick"></a>[function <span class="apidocSignatureSpan">requirejs.</span>nextTick (fn)](#apidoc.element.requirejs.nextTick)
- description and source-code
```javascript
nextTick = function (fn) {
    process.nextTick(fn);
}
```
- example usage
```shell
...
return defined[id];
                    }

                    //Grab defines waiting in the global queue.
                    intakeDefines();

                    //Mark all the dependencies as needing to be loaded.
                    context.nextTick(function () {
//Some defines could have been added since the
//require call, collect them.
intakeDefines();

requireMod = getModule(makeModuleMap(null, relMap));

//Store if map config should be applied to this require
...
```

#### <a name="apidoc.element.requirejs.nodeRequire"></a>[function <span class="apidocSignatureSpan">requirejs.</span>nodeRequire (path)](#apidoc.element.requirejs.nodeRequire)
- description and source-code
```javascript
function require(path) {
  try {
    exports.requireDepth += 1;
    return self.require(path);
  } finally {
    exports.requireDepth -= 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.onError"></a>[function <span class="apidocSignatureSpan">requirejs.</span>onError (err)](#apidoc.element.requirejs.onError)
- description and source-code
```javascript
function defaultOnError(err) {
    throw err;
}
```
- example usage
```shell
...
                    notified = true;
                    mod.emit('error', err);
                }
            }
        });

        if (!notified) {
            req.onError(err);
        }
    }
}

/**
 * Internal method to transfer globalQueue items to this context's
 * defQueue.
...
```

#### <a name="apidoc.element.requirejs.optimize"></a>[function <span class="apidocSignatureSpan">requirejs.</span>optimize (config, callback, errback)](#apidoc.element.requirejs.optimize)
- description and source-code
```javascript
optimize = function (config, callback, errback) {
    if (!loadedOptimizedLib) {
        loadLib();
        loadedOptimizedLib = true;
    }

    //Create the function that will be called once build modules
    //have been loaded.
    var runBuild = function (build, logger, quit) {
        //Make sure config has a log level, and if not,
        //make it "silent" by default.
        config.logLevel = config.hasOwnProperty('logLevel') ?
                          config.logLevel : logger.SILENT;

        //Reset build internals first in case this is part
        //of a long-running server process that could have
        //exceptioned out in a bad state. It is only defined
        //after the first call though.
        if (requirejs._buildReset) {
            requirejs._buildReset();
            requirejs._cacheReset();
        }

        function done(result) {
            //And clean up, in case something else triggers
            //a build in another pathway.
            if (requirejs._buildReset) {
                requirejs._buildReset();
                requirejs._cacheReset();
            }

            // Ensure errors get propagated to the errback
            if (result instanceof Error) {
              throw result;
            }

            return result;
        }

        errback = errback || function (err) {
            // Using console here since logger may have
            // turned off error logging. Since quit is
            // called want to be sure a message is printed.
            console.log(err);
            quit(1);
        };

        build(config).then(done, done).then(callback, errback);
    };

    requirejs({
        context: 'build'
    }, ['build', 'logger', 'env!env/quit'], runBuild);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.specified"></a>[function <span class="apidocSignatureSpan">requirejs.</span>specified ()](#apidoc.element.requirejs.specified)
- description and source-code
```javascript
specified = function () {
    var ctx = contexts[defContextName];
    return ctx.require[prop].apply(ctx, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.toUrl"></a>[function <span class="apidocSignatureSpan">requirejs.</span>toUrl ()](#apidoc.element.requirejs.toUrl)
- description and source-code
```javascript
toUrl = function () {
    var ctx = contexts[defContextName];
    return ctx.require[prop].apply(ctx, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.undef"></a>[function <span class="apidocSignatureSpan">requirejs.</span>undef ()](#apidoc.element.requirejs.undef)
- description and source-code
```javascript
undef = function () {
    var ctx = contexts[defContextName];
    return ctx.require[prop].apply(ctx, arguments);
}
```
- example usage
```shell
...

        function hasPathFallback(id) {
            var pathConfig = getOwn(config.paths, id);
            if (pathConfig && isArray(pathConfig) && pathConfig.length > 1) {
//Pop off the first array value, since it failed, and
//retry
pathConfig.shift();
context.require.undef(id);

//Custom require that does not do map translation, since
//ID is "absolute", already mapped/resolved.
context.makeRequire(null, {
    skipMap: true
})([id]);
...
```



# <a name="apidoc.module.requirejs.nodeRequire"></a>[module requirejs.nodeRequire](#apidoc.module.requirejs.nodeRequire)

#### <a name="apidoc.element.requirejs.nodeRequire.nodeRequire"></a>[function <span class="apidocSignatureSpan">requirejs.</span>nodeRequire (path)](#apidoc.element.requirejs.nodeRequire.nodeRequire)
- description and source-code
```javascript
function require(path) {
  try {
    exports.requireDepth += 1;
    return self.require(path);
  } finally {
    exports.requireDepth -= 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.requirejs.nodeRequire.resolve"></a>[function <span class="apidocSignatureSpan">requirejs.nodeRequire.</span>resolve (request)](#apidoc.element.requirejs.nodeRequire.resolve)
- description and source-code
```javascript
function resolve(request) {
  return Module._resolveFilename(request, self);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.requirejs.nodeRequire.extensions"></a>[module requirejs.nodeRequire.extensions](#apidoc.module.requirejs.nodeRequire.extensions)



# <a name="apidoc.module.requirejs.s"></a>[module requirejs.s](#apidoc.module.requirejs.s)

#### <a name="apidoc.element.requirejs.s.newContext"></a>[function <span class="apidocSignatureSpan">requirejs.s.</span>newContext (contextName)](#apidoc.element.requirejs.s.newContext)
- description and source-code
```javascript
function newContext(contextName) {
    var inCheckLoaded, Module, context, handlers,
        checkLoadedTimeoutId,
        config = {
            //Defaults. Do not set a default for map
            //config to speed up normalize(), which
            //will run faster if there is no default.
            waitSeconds: 7,
            baseUrl: './',
            paths: {},
            bundles: {},
            pkgs: {},
            shim: {},
            config: {}
        },
        registry = {},
        //registry of just enabled modules, to speed
        //cycle breaking code when lots of modules
        //are registered, but not activated.
        enabledRegistry = {},
        undefEvents = {},
        defQueue = [],
        defined = {},
        urlFetched = {},
        bundlesMap = {},
        requireCounter = 1,
        unnormalizedCounter = 1;

<span class="apidocCodeCommentSpan">    /**
     * Trims the . and .. from an array of path segments.
     * It will keep a leading path segment if a .. will become
     * the first path segment, to help with module name lookups,
     * which act like paths, but can be remapped. But the end result,
     * all paths that use this function should look normalized.
     * NOTE: this method MODIFIES the input array.
     * @param {Array} ary the array of path segments.
     */
</span>    function trimDots(ary) {
        var i, part;
        for (i = 0; i < ary.length; i++) {
            part = ary[i];
            if (part === '.') {
                ary.splice(i, 1);
                i -= 1;
            } else if (part === '..') {
                // If at the start, or previous value is still ..,
                // keep them so that when converted to a path it may
                // still work when converted to a path, even though
                // as an ID it is less than ideal. In larger point
                // releases, may be better to just kick out an error.
                if (i === 0 || (i === 1 && ary[2] === '..') || ary[i - 1] === '..') {
                    continue;
                } else if (i > 0) {
                    ary.splice(i - 1, 2);
                    i -= 2;
                }
            }
        }
    }

    /**
     * Given a relative module name, like ./something, normalize it to
     * a real name that can be mapped to a path.
     * @param {String} name the relative name
     * @param {String} baseName a real name that the name arg is relative
     * to.
     * @param {Boolean} applyMap apply the map config to the value. Should
     * only be done if this normalization is for a dependency ID.
     * @returns {String} normalized name
     */
    function normalize(name, baseName, applyMap) {
        var pkgMain, mapValue, nameParts, i, j, nameSegment, lastIndex,
            foundMap, foundI, foundStarMap, starI, normalizedBaseParts,
            baseParts = (baseName && baseName.split('/')),
            map = config.map,
            starMap = map && map['*'];

        //Adjust any relative paths.
        if (name) {
            name = name.split('/');
            lastIndex = name.length - 1;

            // If wanting node ID compatibility, strip .js from end
            // of IDs. Have to do this here, and not in nameToUrl
            // because node allows either .js or non .js to map
            // to same file.
            if (config.nodeIdCompat && jsSuffixRegExp.test(name[lastIndex])) {
                name[lastIndex] = name[lastIndex].replace(jsSuffixRegExp, '');
            }

            // Starts with a '.' so need the baseName
            if (name[0].charAt(0) === '.' && baseParts) {
                //Convert baseName to array, and lop off the last part,
                //so that . matches that 'directory' and not name of the baseName's
                //module. For instance, baseName of 'one/two/three', maps to
                //'one/two/three.js', but we want the directory, 'one/two' for
                //this normalization.
                normalizedBaseParts = baseParts.slice(0, baseParts.length - 1);
                name = normalizedBaseParts.concat(name);
            } ...
```
- example usage
```shell
...

if (config && config.context) {
    contextName = config.context;
}

context = getOwn(contexts, contextName);
if (!context) {
    context = contexts[contextName] = req.s.newContext(contextName);
}

if (config) {
    context.configure(config);
}

return context.require(deps, callback, errback);
...
```



# <a name="apidoc.module.requirejs.tools"></a>[module requirejs.tools](#apidoc.module.requirejs.tools)

#### <a name="apidoc.element.requirejs.tools.useLib"></a>[function <span class="apidocSignatureSpan">requirejs.tools.</span>useLib (contextName, callback)](#apidoc.element.requirejs.tools.useLib)
- description and source-code
```javascript
useLib = function (contextName, callback) {
    if (!callback) {
        callback = contextName;
        contextName = 'uselib';
    }

    if (!useLibLoaded[contextName]) {
        loadLib();
        useLibLoaded[contextName] = true;
    }

    var req = requirejs({
        context: contextName
    });

    req(['build'], function () {
        callback(req);
    });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
