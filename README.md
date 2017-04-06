# api documentation for  [browser-perf (v1.4.11)](https://github.com/axemclion/browser-perf#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-browser-perf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-browser-perf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-browser-perf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-browser-perf)
#### Measure browser rendering performance metrics

[![NPM](https://nodei.co/npm/browser-perf.png?downloads=true)](https://www.npmjs.com/package/browser-perf)

[![apidoc](https://npmdoc.github.io/node-npmdoc-browser-perf/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-browser-perf_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-browser-perf/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-browser-perf/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-browser-perf/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Parashuram"
    },
    "bin": {
        "browser-perf": "lib/cli.js"
    },
    "bugs": {
        "url": "https://github.com/axemclion/browser-perf/issues"
    },
    "dependencies": {
        "JSONStream": "^1.0.6",
        "byline": "^4.2.1",
        "cli-table": "~0.3.1",
        "commander": "^2.9.0",
        "debug": "^2.2.0",
        "event-stream": "^3.3.2",
        "glob": "^6.0.2",
        "jsmin": "~1.0.1",
        "q": "^1.4.1",
        "request": "^2.65.0",
        "wd": "^0.4.0"
    },
    "description": "Measure browser rendering performance metrics",
    "devDependencies": {
        "chai": "~3.4.0",
        "chai-as-promised": "^5.1.0",
        "mocha": "^2.3.3",
        "sinon": "^1.17.2"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "3d73394331438aa0dbf3455a98ab2306a035b2aa",
        "tarball": "https://registry.npmjs.org/browser-perf/-/browser-perf-1.4.11.tgz"
    },
    "gitHead": "db8aecd284725cb99c9e868c2d9bcde53f9b445a",
    "homepage": "https://github.com/axemclion/browser-perf#readme",
    "keywords": [
        "browser-perf",
        "rendering",
        "telemetry",
        "chromium",
        "performance",
        "high performance web sites",
        "metrics",
        "monitoring",
        "web development",
        "webperf"
    ],
    "license": "BSD-2-Clause",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "axemclion",
            "email": "code@r.nparashuram.com"
        }
    ],
    "name": "browser-perf",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/axemclion/browser-perf.git"
    },
    "scripts": {
        "test": "mocha --recursive --require=./test/test.helper.js ./test"
    },
    "version": "1.4.11"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module browser-perf](#apidoc.module.browser-perf)
1.  [function <span class="apidocSignatureSpan">browser-perf.</span>docs (source)](#apidoc.element.browser-perf.docs)
1.  [function <span class="apidocSignatureSpan">browser-perf.</span>runner (opts)](#apidoc.element.browser-perf.runner)
1.  object <span class="apidocSignatureSpan">browser-perf.</span>actions
1.  object <span class="apidocSignatureSpan">browser-perf.</span>docs.prototype
1.  object <span class="apidocSignatureSpan">browser-perf.</span>helpers
1.  object <span class="apidocSignatureSpan">browser-perf.</span>options
1.  object <span class="apidocSignatureSpan">browser-perf.</span>runner.prototype

#### [module browser-perf.actions](#apidoc.module.browser-perf.actions)
1.  [function <span class="apidocSignatureSpan">browser-perf.actions.</span>login (cfg)](#apidoc.element.browser-perf.actions.login)
1.  [function <span class="apidocSignatureSpan">browser-perf.actions.</span>scroll (cfg)](#apidoc.element.browser-perf.actions.scroll)
1.  [function <span class="apidocSignatureSpan">browser-perf.actions.</span>wait (cfg)](#apidoc.element.browser-perf.actions.wait)

#### [module browser-perf.docs](#apidoc.module.browser-perf.docs)
1.  [function <span class="apidocSignatureSpan">browser-perf.</span>docs (source)](#apidoc.element.browser-perf.docs.docs)

#### [module browser-perf.docs.prototype](#apidoc.module.browser-perf.docs.prototype)
1.  [function <span class="apidocSignatureSpan">browser-perf.docs.prototype.</span>get (metric)](#apidoc.element.browser-perf.docs.prototype.get)
1.  [function <span class="apidocSignatureSpan">browser-perf.docs.prototype.</span>getProp (metric, prop)](#apidoc.element.browser-perf.docs.prototype.getProp)

#### [module browser-perf.helpers](#apidoc.module.browser-perf.helpers)
1.  [function <span class="apidocSignatureSpan">browser-perf.helpers.</span>deepEquals (global, prop, val)](#apidoc.element.browser-perf.helpers.deepEquals)
1.  [function <span class="apidocSignatureSpan">browser-perf.helpers.</span>extend (obj1, obj2)](#apidoc.element.browser-perf.helpers.extend)
1.  [function <span class="apidocSignatureSpan">browser-perf.helpers.</span>fnCall (fn, args)](#apidoc.element.browser-perf.helpers.fnCall)
1.  [function <span class="apidocSignatureSpan">browser-perf.helpers.</span>metrics (value, category, source, unit, importance, tags)](#apidoc.element.browser-perf.helpers.metrics)

#### [module browser-perf.options](#apidoc.module.browser-perf.options)
1.  [function <span class="apidocSignatureSpan">browser-perf.options.</span>scrub (cfg)](#apidoc.element.browser-perf.options.scrub)
1.  object <span class="apidocSignatureSpan">browser-perf.options.</span>sanitizers

#### [module browser-perf.runner](#apidoc.module.browser-perf.runner)
1.  [function <span class="apidocSignatureSpan">browser-perf.</span>runner (opts)](#apidoc.element.browser-perf.runner.runner)

#### [module browser-perf.runner.prototype](#apidoc.module.browser-perf.runner.prototype)
1.  [function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>attachBrowser_ (sessionId)](#apidoc.element.browser-perf.runner.prototype.attachBrowser_)
1.  [function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>config (cb)](#apidoc.element.browser-perf.runner.prototype.config)
1.  [function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>setupMetrics_ ()](#apidoc.element.browser-perf.runner.prototype.setupMetrics_)
1.  [function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>start (sessionId, cb)](#apidoc.element.browser-perf.runner.prototype.start)
1.  [function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>stop (cb)](#apidoc.element.browser-perf.runner.prototype.stop)



# <a name="apidoc.module.browser-perf"></a>[module browser-perf](#apidoc.module.browser-perf)

#### <a name="apidoc.element.browser-perf.docs"></a>[function <span class="apidocSignatureSpan">browser-perf.</span>docs (source)](#apidoc.element.browser-perf.docs)
- description and source-code
```javascript
docs = function (source) {
	var glob = require('glob');
	var fs = require('fs');
	var path = require('path');

	var files;
	if (typeof source !== 'undefined' && typeof source === 'string') {
		files = [source + '.json'];
	} else if (Array.isArray(source)) {
		files = source.map(function(file) {
			return file + (path.extname(file) !== '.json' ? '.json' : '');
		});
	} else {
		files = glob.sync('*.json', {
			cwd: __dirname
		});
	}

	this.metrics = {};
	for (var i = 0; i < files.length; i++) {
		var fileContent = JSON.parse(fs.readFileSync(path.join(__dirname, files[i]), 'utf-8'));
		for (var key in fileContent) {
			this.metrics[key] = fileContent[key];
		}
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.runner"></a>[function <span class="apidocSignatureSpan">browser-perf.</span>runner (opts)](#apidoc.element.browser-perf.runner)
- description and source-code
```javascript
function Runner(opts) {
	this.opts = options.scrub(opts);
	this.metrics = null;
	this.browser = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.actions"></a>[module browser-perf.actions](#apidoc.module.browser-perf.actions)

#### <a name="apidoc.element.browser-perf.actions.login"></a>[function <span class="apidocSignatureSpan">browser-perf.actions.</span>login (cfg)](#apidoc.element.browser-perf.actions.login)
- description and source-code
```javascript
login = function (cfg) {
	cfg = cfg || {};
	debug = require('debug')('bp:actions:login');
	return function(browser) {
		debug('Loading login form');
		return browser.get(cfg.page).then(function() {
			debug('Filling in Username');
			return browser.elementByCssSelector(cfg.username.field)
		}).then(function(el) {
			return el.type(cfg.username.val || cfg.username.value);
		}).then(function() {
			debug('Filling in Password');
			return browser.elementByCssSelector(cfg.password.field);
		}).then(function(el) {
			return el.type(cfg.password.val || cfg.password.value);
		}).then(function() {
			return browser.elementByCssSelector(cfg.submit.field);
		}).then(function(el) {
			debug('Clicking submit');
			return el.click();
		}).then(function() {
			return browser.sleep(5000);
		});
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.actions.scroll"></a>[function <span class="apidocSignatureSpan">browser-perf.actions.</span>scroll (cfg)](#apidoc.element.browser-perf.actions.scroll)
- description and source-code
```javascript
scroll = function (cfg) {
	cfg = cfg || {};

	function scroll(browser) {

		var raf_scroll = jsmin(fs.readFileSync(__dirname + '/page_scripts/raf_scroll.js', 'utf-8')),
			chrome_scroll = jsmin(fs.readFileSync(__dirname + '/page_scripts/chrome_scroll.js', 'utf-8')),
			gesture_common = jsmin(fs.readFileSync(__dirname + '/page_scripts/gesture_common.js', 'utf-8'));

		var runner = function(opts) {
			console.log("Scrolling with ", opts);
			window.__scrollActionDone = false;
			window.__scrollAction = new __ScrollAction(function() {
				window.__scrollActionDone = true;
			});
			window.__scrollAction.start({
				element: eval(opts.el),
				left_start_percentage: opts.left_start_percentage,
				top_start_percentage: opts.top_start_percentage,
				direction: opts.direction,
				speed: opts.speed,
				gesture_source_type: opts.gesture_source_type
			});
		};

		debug('Initializing Scroll function');
		return browser.execute(gesture_common + chrome_scroll + raf_scroll + helpers.fnCall(runner, {
			left_start_percentage: 0.5,
			top_start_percentage: 0.5,
			direction: cfg.direction || 'down',
			speed: cfg.speed || 800,
			gesture_source_type: 0,
			el: cfg.scrollElement || 'document.body'
		})).then(function() {
			debug('Waiting for Scrolling to finish');
			return browser.waitFor({
				asserter: wd.asserters.jsCondition('(window.__scrollActionDone === true)', false),
				timeout: 1000 * 60 * 10,
				pollFreq: cfg.pollFreq || 2000
			});
		})
	};

	scroll.setup = function(cfg) {
		cfg.browsers = cfg.browsers.map(function(browser) {
			if (browser.browserName && (browser.browserName.match(/android/i) || browser.browserName.match(/chrome/i))) {
				helpers.extend(browser, {
					chromeOptions: {
						args: ['--enable-gpu-benchmarking', '--enable-thread-composting']
					}
				});
			}
			return browser;
		});
		return Q(cfg);
	};

	return scroll;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.actions.wait"></a>[function <span class="apidocSignatureSpan">browser-perf.actions.</span>wait (cfg)](#apidoc.element.browser-perf.actions.wait)
- description and source-code
```javascript
wait = function (cfg) {
	cfg = cfg || {};
	var debug = require('debug')('bp:actions:wait');
	return function(browser) {
		var duration = cfg || 5000;
		debug('Waiting for some time - %d', duration);
		return browser.sleep(duration);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.docs"></a>[module browser-perf.docs](#apidoc.module.browser-perf.docs)

#### <a name="apidoc.element.browser-perf.docs.docs"></a>[function <span class="apidocSignatureSpan">browser-perf.</span>docs (source)](#apidoc.element.browser-perf.docs.docs)
- description and source-code
```javascript
docs = function (source) {
	var glob = require('glob');
	var fs = require('fs');
	var path = require('path');

	var files;
	if (typeof source !== 'undefined' && typeof source === 'string') {
		files = [source + '.json'];
	} else if (Array.isArray(source)) {
		files = source.map(function(file) {
			return file + (path.extname(file) !== '.json' ? '.json' : '');
		});
	} else {
		files = glob.sync('*.json', {
			cwd: __dirname
		});
	}

	this.metrics = {};
	for (var i = 0; i < files.length; i++) {
		var fileContent = JSON.parse(fs.readFileSync(path.join(__dirname, files[i]), 'utf-8'));
		for (var key in fileContent) {
			this.metrics[key] = fileContent[key];
		}
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.docs.prototype"></a>[module browser-perf.docs.prototype](#apidoc.module.browser-perf.docs.prototype)

#### <a name="apidoc.element.browser-perf.docs.prototype.get"></a>[function <span class="apidocSignatureSpan">browser-perf.docs.prototype.</span>get (metric)](#apidoc.element.browser-perf.docs.prototype.get)
- description and source-code
```javascript
get = function (metric) {
	return this.metrics[metric] || {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.docs.prototype.getProp"></a>[function <span class="apidocSignatureSpan">browser-perf.docs.prototype.</span>getProp (metric, prop)](#apidoc.element.browser-perf.docs.prototype.getProp)
- description and source-code
```javascript
getProp = function (metric, prop) {
	return (typeof this.metrics[metric] !== 'undefined' ? this.metrics[metric][prop] : undefined);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.helpers"></a>[module browser-perf.helpers](#apidoc.module.browser-perf.helpers)

#### <a name="apidoc.element.browser-perf.helpers.deepEquals"></a>[function <span class="apidocSignatureSpan">browser-perf.helpers.</span>deepEquals (global, prop, val)](#apidoc.element.browser-perf.helpers.deepEquals)
- description and source-code
```javascript
deepEquals = function (global, prop, val) {
	var props = prop.split('.');
	for (var i = 0; i < props.length; i++) {
		if (typeof global !== 'object' || global === null){
			return false;
		}
		
		if (typeof global[props[i]] === 'undefined') {
			return false;
		}
		global = global[props[i]];
	}
	return global === val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.helpers.extend"></a>[function <span class="apidocSignatureSpan">browser-perf.helpers.</span>extend (obj1, obj2)](#apidoc.element.browser-perf.helpers.extend)
- description and source-code
```javascript
extend = function (obj1, obj2) {
	if (typeof obj1 !== 'object' && !obj1) {
		obj1 = {};
	}
	if (typeof obj2 !== 'object' && !obj2) {
		obj2 = {};
	}
	for (var key in obj2) {
		if (Array.isArray(obj1[key]) && Array.isArray(obj2[key])) {
			obj1[key] = obj1[key].concat(obj2[key]);
		} else if (typeof obj1[key] === 'object' && typeof obj2[key] === 'object' && !Array.isArray(obj1[key]) && !Array.isArray(obj2[
key])) {
			obj1[key] = extend(obj1[key], obj2[key]);
		} else {
			obj1[key] = obj2[key];
		}
	}
	return obj1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.helpers.fnCall"></a>[function <span class="apidocSignatureSpan">browser-perf.helpers.</span>fnCall (fn, args)](#apidoc.element.browser-perf.helpers.fnCall)
- description and source-code
```javascript
fnCall = function (fn, args) {
		args = args || '';
		if (typeof args === 'object') {
			args = JSON.stringify(args);
		}
		return '(' + jsmin(fn.toString()) + '(' + args + '));';
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.helpers.metrics"></a>[function <span class="apidocSignatureSpan">browser-perf.helpers.</span>metrics (value, category, source, unit, importance, tags)](#apidoc.element.browser-perf.helpers.metrics)
- description and source-code
```javascript
metrics = function (value, category, source, unit, importance, tags) {
	return {
		value: value,
		unit: unit || 'ms',
		category: category,
		source: source,
		tags: tags || [],
		importance: importance || 0
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.options"></a>[module browser-perf.options](#apidoc.module.browser-perf.options)

#### <a name="apidoc.element.browser-perf.options.scrub"></a>[function <span class="apidocSignatureSpan">browser-perf.options.</span>scrub (cfg)](#apidoc.element.browser-perf.options.scrub)
- description and source-code
```javascript
scrub = function (cfg) {
		cfg = cfg || {};
		sanitizers.forEach(function(sanitizer, i) {
			cfg = sanitizer(cfg);
		});
		return cfg;
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.runner"></a>[module browser-perf.runner](#apidoc.module.browser-perf.runner)

#### <a name="apidoc.element.browser-perf.runner.runner"></a>[function <span class="apidocSignatureSpan">browser-perf.</span>runner (opts)](#apidoc.element.browser-perf.runner.runner)
- description and source-code
```javascript
function Runner(opts) {
	this.opts = options.scrub(opts);
	this.metrics = null;
	this.browser = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.browser-perf.runner.prototype"></a>[module browser-perf.runner.prototype](#apidoc.module.browser-perf.runner.prototype)

#### <a name="apidoc.element.browser-perf.runner.prototype.attachBrowser_"></a>[function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>attachBrowser_ (sessionId)](#apidoc.element.browser-perf.runner.prototype.attachBrowser_)
- description and source-code
```javascript
attachBrowser_ = function (sessionId) {
	if (this.browser === null) {
		this.browser = wd.promiseRemote(this.opts.selenium);
		this.browser.on('status', function(data) {
			//log.debug(data);
		});
		this.browser.on('command', function(meth, path, data) {
			if (data && typeof data === 'object') {
				var data = JSON.stringify(data);
			}
			debug(meth, (path || '').substr(0, 70), (data || '').substr(0, 70));
		});
		return this.browser.attach(sessionId);
	} else {
		return Q();
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.runner.prototype.config"></a>[function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>config (cb)](#apidoc.element.browser-perf.runner.prototype.config)
- description and source-code
```javascript
config = function (cb) {
	var me = this;
	this.setupMetrics_().then(function() {
		cb(null, me.opts);
	}, function(err) {
		cb(err);
	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.runner.prototype.setupMetrics_"></a>[function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>setupMetrics_ ()](#apidoc.element.browser-perf.runner.prototype.setupMetrics_)
- description and source-code
```javascript
setupMetrics_ = function () {
	var me = this;
	if (this.metrics === null) {
		this.metrics = new Metrics(this.opts.metrics);
		return this.metrics.setup(this.opts);
	} else {
		return Q();
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.runner.prototype.start"></a>[function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>start (sessionId, cb)](#apidoc.element.browser-perf.runner.prototype.start)
- description and source-code
```javascript
start = function (sessionId, cb) {
	var me = this;
	if (typeof cb !== 'function') {
		cb = function() {};
	}
	this.setupMetrics_().then(function() {
		return me.attachBrowser_(sessionId);
	}).then(function() {
		me.metrics.start(me.browser).then(cb, cb);
	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.browser-perf.runner.prototype.stop"></a>[function <span class="apidocSignatureSpan">browser-perf.runner.prototype.</span>stop (cb)](#apidoc.element.browser-perf.runner.prototype.stop)
- description and source-code
```javascript
stop = function (cb) {
	var me = this;
	this.metrics.teardown(this.browser).then(function() {
		return me.metrics.getResults();
	}).then(function(data) {
		cb(undefined, data);
	}, function(err) {
		cb(err, null);
	});
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
