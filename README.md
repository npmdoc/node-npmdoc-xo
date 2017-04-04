# api documentation for  [xo (v0.18.1)](https://github.com/sindresorhus/xo#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-xo.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xo) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xo.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xo)
#### JavaScript happiness style linter ❤️

[![NPM](https://nodei.co/npm/xo.png?downloads=true)](https://www.npmjs.com/package/xo)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xo/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-xo_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xo/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xo/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xo/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sindre Sorhus",
        "email": "sindresorhus@gmail.com",
        "url": "sindresorhus.com"
    },
    "bin": {
        "xo": "cli.js"
    },
    "bugs": {
        "url": "https://github.com/sindresorhus/xo/issues"
    },
    "dependencies": {
        "arrify": "^1.0.0",
        "debug": "^2.2.0",
        "deep-assign": "^1.0.0",
        "eslint": "^3.18.0",
        "eslint-config-xo": "^0.18.0",
        "eslint-formatter-pretty": "^1.0.0",
        "eslint-plugin-ava": "^4.2.0",
        "eslint-plugin-import": "^2.0.0",
        "eslint-plugin-no-use-extend-native": "^0.3.2",
        "eslint-plugin-promise": "^3.4.0",
        "eslint-plugin-unicorn": "^2.1.0",
        "get-stdin": "^5.0.0",
        "globby": "^6.0.0",
        "has-flag": "^2.0.0",
        "lodash.isequal": "^4.4.0",
        "meow": "^3.4.2",
        "multimatch": "^2.1.0",
        "parse-gitignore": "^0.3.1",
        "path-exists": "^3.0.0",
        "pkg-conf": "^2.0.0",
        "resolve-cwd": "^1.0.0",
        "resolve-from": "^2.0.0",
        "update-notifier": "^2.1.0",
        "xo-init": "^0.5.0"
    },
    "description": "JavaScript happiness style linter ❤️",
    "devDependencies": {
        "ava": "*",
        "coveralls": "^2.11.9",
        "eslint-config-xo-react": "^0.10.0",
        "eslint-plugin-react": "^6.3.0",
        "execa": "^0.6.1",
        "nyc": "^10.1.2",
        "pify": "^2.3.0",
        "proxyquire": "^1.7.3",
        "temp-write": "^3.1.0",
        "xo": "github:sindresorhus/xo#v0.17.1"
    },
    "directories": {},
    "dist": {
        "shasum": "529bb1cbd612f200221d76df90639d5c88cedf54",
        "tarball": "https://registry.npmjs.org/xo/-/xo-0.18.1.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "index.js",
        "cli.js",
        "options-manager.js",
        "config"
    ],
    "gitHead": "d82bdea1dcccdf27bb8358516150034f7a8e2c41",
    "homepage": "https://github.com/sindresorhus/xo#readme",
    "keywords": [
        "❤️",
        "cli-app",
        "cli",
        "xo",
        "xoxo",
        "hugs",
        "kisses",
        "happy",
        "happiness",
        "code",
        "quality",
        "style",
        "lint",
        "linter",
        "jscs",
        "jshint",
        "jslint",
        "eslint",
        "validate",
        "code style",
        "standard",
        "strict",
        "check",
        "checker",
        "verify",
        "enforce",
        "hint",
        "simple"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "jamestalmage",
            "email": "james@talmage.io"
        },
        {
            "name": "marionebl",
            "email": "root@mario-nebl.de"
        },
        {
            "name": "sindresorhus",
            "email": "sindresorhus@gmail.com"
        }
    ],
    "name": "xo",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sindresorhus/xo.git"
    },
    "scripts": {
        "coveralls": "nyc report --reporter=text-lcov | coveralls",
        "test": "xo && nyc ava"
    },
    "version": "0.18.1",
    "xo": {
        "esnext": true
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module xo](#apidoc.module.xo)
1.  [function <span class="apidocSignatureSpan">xo.</span>getErrorResults (results)](#apidoc.element.xo.getErrorResults)
1.  [function <span class="apidocSignatureSpan">xo.</span>getFormatter (format)](#apidoc.element.xo.getFormatter)
1.  [function <span class="apidocSignatureSpan">xo.</span>lintFiles (patterns, opts)](#apidoc.element.xo.lintFiles)
1.  [function <span class="apidocSignatureSpan">xo.</span>lintText (str, opts)](#apidoc.element.xo.lintText)
1.  [function <span class="apidocSignatureSpan">xo.</span>outputFixes (report)](#apidoc.element.xo.outputFixes)
1.  object <span class="apidocSignatureSpan">xo.</span>options_manager

#### [module xo.options_manager](#apidoc.module.xo.options_manager)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>buildConfig ( emptyOptions()](#apidoc.element.xo.options_manager.buildConfig)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>emptyOptions ()](#apidoc.element.xo.options_manager.emptyOptions)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>findApplicableOverrides (path, overrides)](#apidoc.element.xo.options_manager.findApplicableOverrides)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>getGitIgnores ('**/.gitignore', { ignore: opts.ignores || [], cwd: opts.cwd || process.cwd()](#apidoc.element.xo.options_manager.getGitIgnores)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>getIgnores (opts.ignores || [])](#apidoc.element.xo.options_manager.getIgnores)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>groupConfigs (paths, baseOptions, overrides)](#apidoc.element.xo.options_manager.groupConfigs)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>mergeApplicableOverrides (baseOptions, applicableOverrides)](#apidoc.element.xo.options_manager.mergeApplicableOverrides)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>mergeWithPkgConf ({cwd: process.cwd()](#apidoc.element.xo.options_manager.mergeWithPkgConf)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>normalizeOpts ({}, opts)](#apidoc.element.xo.options_manager.normalizeOpts)
1.  [function <span class="apidocSignatureSpan">xo.options_manager.</span>preprocess (opts)](#apidoc.element.xo.options_manager.preprocess)
1.  object <span class="apidocSignatureSpan">xo.options_manager.</span>DEFAULT_CONFIG
1.  object <span class="apidocSignatureSpan">xo.options_manager.</span>DEFAULT_IGNORE



# <a name="apidoc.module.xo"></a>[module xo](#apidoc.module.xo)

#### <a name="apidoc.element.xo.getErrorResults"></a>[function <span class="apidocSignatureSpan">xo.</span>getErrorResults (results)](#apidoc.element.xo.getErrorResults)
- description and source-code
```javascript
getErrorResults = function (results) {
    const filtered = [];

    results.forEach(result => {
        const filteredMessages = result.messages.filter(isErrorMessage);

        if (filteredMessages.length > 0) {
            filtered.push(
                Object.assign(result, {
                    messages: filteredMessages,
                    errorCount: filteredMessages.length,
                    warningCount: 0
                })
            );
        }
    });

    return filtered;
}
```
- example usage
```shell
...
	const engine = new eslint.CLIEngine(config);
	const report = engine.executeOnFiles(paths, config);

	return processReport(report, opts);
}

function processReport(report, opts) {
	report.results = opts.quiet ? eslint.CLIEngine.getErrorResults(report.results) : report.results;
	return report;
}

exports.getFormatter = eslint.CLIEngine.getFormatter;
exports.getErrorResults = eslint.CLIEngine.getErrorResults;
exports.outputFixes = eslint.CLIEngine.outputFixes;
...
```

#### <a name="apidoc.element.xo.getFormatter"></a>[function <span class="apidocSignatureSpan">xo.</span>getFormatter (format)](#apidoc.element.xo.getFormatter)
- description and source-code
```javascript
getFormatter = function (format) {

    let formatterPath;

    // default is stylish
    format = format || "stylish";

    // only strings are valid formatters
    if (typeof format === "string") {

        // replace \ with / for Windows compatibility
        format = format.replace(/\\/g, "/");

        // if there's a slash, then it's a file
        if (format.indexOf("/") > -1) {
            const cwd = this.options ? this.options.cwd : process.cwd();

            formatterPath = path.resolve(cwd, format);
        } else {
            formatterPath = './formatters/${format}';
        }

        try {
            return require(formatterPath);
        } catch (ex) {
            ex.message = 'There was a problem loading formatter: ${formatterPath}\nError: ${ex.message}';
            throw ex;
        }

    } else {
        return null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xo.lintFiles"></a>[function <span class="apidocSignatureSpan">xo.</span>lintFiles (patterns, opts)](#apidoc.element.xo.lintFiles)
- description and source-code
```javascript
(patterns, opts) => {
	opts = optionsManager.preprocess(opts);
	patterns = patterns.length === 0 ? ['**/*'] : arrify(patterns);

	const gitIgnores = optionsManager.getGitIgnores(opts);
	const glob = patterns.concat(gitIgnores);

	return globby(glob, {ignore: opts.ignores, nodir: true}).then(paths => {
		// Filter out unwanted file extensions
		// for silly users that don't specify an extension in the glob pattern
		paths = paths.filter(x => {
			// Remove dot before the actual extension
			const ext = path.extname(x).replace('.', '');
			return opts.extensions.indexOf(ext) !== -1;
		});

		if (!(opts.overrides && opts.overrides.length > 0)) {
			return runEslint(paths, opts);
		}

		const overrides = opts.overrides;
		delete opts.overrides;

		const grouped = optionsManager.groupConfigs(paths, opts, overrides);

		return mergeReports(grouped.map(data => runEslint(data.paths, data.opts)));
	});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xo.lintText"></a>[function <span class="apidocSignatureSpan">xo.</span>lintText (str, opts)](#apidoc.element.xo.lintText)
- description and source-code
```javascript
(str, opts) => {
	opts = optionsManager.preprocess(opts);

	if (opts.overrides && opts.overrides.length > 0) {
		const overrides = opts.overrides;
		delete opts.overrides;

		const filename = path.relative(opts.cwd, opts.filename);

		const foundOverrides = optionsManager.findApplicableOverrides(filename, overrides);
		opts = optionsManager.mergeApplicableOverrides(opts, foundOverrides.applicable);
	}

	opts = optionsManager.buildConfig(opts);
	const defaultIgnores = optionsManager.getIgnores({}).ignores;

	if (opts.ignores && !isEqual(defaultIgnores, opts.ignores) && typeof opts.filename !== 'string') {
		throw new Error('The 'ignores' option requires the 'filename' option to be defined.');
	}

	if (opts.filename) {
		const filename = path.relative(opts.cwd, opts.filename);
		const gitIgnores = optionsManager.getGitIgnores(opts);
		const glob = [filename].concat(gitIgnores);

		if (multimatch(glob, opts.ignores).length > 0) {
			return {
				errorCount: 0,
				warningCount: 0,
				results: [{
					errorCount: 0,
					filePath: filename,
					messages: [],
					warningCount: 0
				}]
			};
		}
	}

	const engine = new eslint.CLIEngine(opts);
	const report = engine.executeOnText(str, opts.filename);

	return processReport(report, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xo.outputFixes"></a>[function <span class="apidocSignatureSpan">xo.</span>outputFixes (report)](#apidoc.element.xo.outputFixes)
- description and source-code
```javascript
outputFixes = function (report) {
    report.results.filter(result => result.hasOwnProperty("output")).forEach(result => {
        fs.writeFileSync(result.filePath, result.output);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.xo.options_manager"></a>[module xo.options_manager](#apidoc.module.xo.options_manager)

#### <a name="apidoc.element.xo.options_manager.buildConfig"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>buildConfig ( emptyOptions()](#apidoc.element.xo.options_manager.buildConfig)
- description and source-code
```javascript
opts => {
	const config = deepAssign( emptyOptions(),
		DEFAULT_CONFIG,
		opts
	);

	if (opts.space) {
		const spaces = typeof opts.space === 'number' ? opts.space : 2;
		config.rules.indent = ['error', spaces, {SwitchCase: 1}];

		// Only apply if the user has the React plugin
		if (opts.cwd && resolveFrom(opts.cwd, 'eslint-plugin-react')) {
			config.plugins = config.plugins.concat('react');
			config.rules['react/jsx-indent-props'] = ['error', spaces];
			config.rules['react/jsx-indent'] = ['error', spaces];
		}
	}

	if (opts.semicolon === false) {
		config.rules.semi = ['error', 'never'];
		config.rules['semi-spacing'] = ['error', {
			before: false,
			after: true
		}];
	}

	if (opts.esnext !== false) {
		config.baseConfig.extends = ['xo/esnext', path.join(__dirname, 'config/plugins.js')];
	}

	if (opts.rules) {
		Object.assign(config.rules, opts.rules);
	}

	if (opts.settings) {
		config.baseConfig.settings = opts.settings;
	}

	if (opts.parser) {
		config.baseConfig.parser = opts.parser;
	}

	if (opts.extends && opts.extends.length > 0) {
		// TODO: this logic needs to be improved, preferably use the same code as ESLint
		// user's configs must be resolved to their absolute paths
		const configs = opts.extends.map(name => {
			// Don't do anything if it's a filepath
			if (pathExists.sync(name)) {
				return name;
			}

			// Don't do anything if it's a config from a plugin
			if (name.startsWith('plugin:')) {
				return name;
			}

			if (!name.includes('eslint-config-')) {
				name = 'eslint-config-${name}';
			}

			const ret = resolveFrom(opts.cwd, name);

			if (!ret) {
				throw new Error('Couldn't find ESLint config: ${name}');
			}

			return ret;
		});

		config.baseConfig.extends = config.baseConfig.extends.concat(configs);
	}

	return config;
}
```
- example usage
```shell
...

		const filename = path.relative(opts.cwd, opts.filename);

		const foundOverrides = optionsManager.findApplicableOverrides(filename, overrides);
		opts = optionsManager.mergeApplicableOverrides(opts, foundOverrides.applicable);
	}

	opts = optionsManager.buildConfig(opts);
	const defaultIgnores = optionsManager.getIgnores({}).ignores;

	if (opts.ignores && !isEqual(defaultIgnores, opts.ignores) && typeof opts.filename !== 'string') {
		throw new Error('The 'ignores' option requires the 'filename' option to be defined.');
	}

	if (opts.filename) {
...
```

#### <a name="apidoc.element.xo.options_manager.emptyOptions"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>emptyOptions ()](#apidoc.element.xo.options_manager.emptyOptions)
- description and source-code
```javascript
() => ({
	rules: {},
	settings: {},
	globals: [],
	envs: [],
	plugins: [],
	extends: []
})
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xo.options_manager.findApplicableOverrides"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>findApplicableOverrides (path, overrides)](#apidoc.element.xo.options_manager.findApplicableOverrides)
- description and source-code
```javascript
(path, overrides) => {
	let hash = 0;
	const applicable = [];

	overrides.forEach(override => {
		hash <<= 1;

		if (multimatch(path, override.files).length > 0) {
			applicable.push(override);
			hash |= 1;
		}
	});

	return {
		hash,
		applicable
	};
}
```
- example usage
```shell
...

	if (opts.overrides && opts.overrides.length > 0) {
		const overrides = opts.overrides;
		delete opts.overrides;

		const filename = path.relative(opts.cwd, opts.filename);

		const foundOverrides = optionsManager.findApplicableOverrides(filename, overrides);
		opts = optionsManager.mergeApplicableOverrides(opts, foundOverrides.applicable);
	}

	opts = optionsManager.buildConfig(opts);
	const defaultIgnores = optionsManager.getIgnores({}).ignores;

	if (opts.ignores && !isEqual(defaultIgnores, opts.ignores) && typeof opts.filename !== 'string') {
...
```

#### <a name="apidoc.element.xo.options_manager.getGitIgnores"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>getGitIgnores ('**/.gitignore', { ignore: opts.ignores || [], cwd: opts.cwd || process.cwd()](#apidoc.element.xo.options_manager.getGitIgnores)
- description and source-code
```javascript
opts => globby
	.sync('**/.gitignore', { ignore: opts.ignores || [], cwd: opts.cwd || process.cwd()
	})
	.map(pathToGitignore => {
		const patterns = parseGitignore(pathToGitignore);
		const base = path.dirname(pathToGitignore);

		return patterns
			.map(pattern => {
				const negate = !pattern.startsWith('!');
				const patternPath = negate ? pattern : pattern.substr(1);
				return {negate, pattern: path.join(base, patternPath)};
			})
			.sort(pattern => pattern.negate ? 1 : -1)
			.map(item => item.negate ? '!${item.pattern}' : item.pattern);
	})
	.reduce((a, b) => a.concat(b), [])
```
- example usage
```shell
...

	if (opts.ignores && !isEqual(defaultIgnores, opts.ignores) && typeof opts.filename !== 'string') {
		throw new Error('The 'ignores' option requires the 'filename' option to be defined.');
	}

	if (opts.filename) {
		const filename = path.relative(opts.cwd, opts.filename);
		const gitIgnores = optionsManager.getGitIgnores(opts);
		const glob = [filename].concat(gitIgnores);

		if (multimatch(glob, opts.ignores).length > 0) {
			return {
				errorCount: 0,
				warningCount: 0,
				results: [{
...
```

#### <a name="apidoc.element.xo.options_manager.getIgnores"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>getIgnores (opts.ignores || [])](#apidoc.element.xo.options_manager.getIgnores)
- description and source-code
```javascript
opts => {
	opts.ignores = DEFAULT_IGNORE.concat(opts.ignores || []);
	return opts;
}
```
- example usage
```shell
...
		const filename = path.relative(opts.cwd, opts.filename);

		const foundOverrides = optionsManager.findApplicableOverrides(filename, overrides);
		opts = optionsManager.mergeApplicableOverrides(opts, foundOverrides.applicable);
	}

	opts = optionsManager.buildConfig(opts);
	const defaultIgnores = optionsManager.getIgnores({}).ignores;

	if (opts.ignores && !isEqual(defaultIgnores, opts.ignores) && typeof opts.filename !== 'string') {
		throw new Error('The 'ignores' option requires the 'filename' option to be defined.');
	}

	if (opts.filename) {
		const filename = path.relative(opts.cwd, opts.filename);
...
```

#### <a name="apidoc.element.xo.options_manager.groupConfigs"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>groupConfigs (paths, baseOptions, overrides)](#apidoc.element.xo.options_manager.groupConfigs)
- description and source-code
```javascript
(paths, baseOptions, overrides) => {
	const map = {};
	const arr = [];

	paths.forEach(x => {
		const data = findApplicableOverrides(x, overrides);

		if (!map[data.hash]) {
			const mergedOpts = mergeApplicableOverrides(baseOptions, data.applicable);
			delete mergedOpts.files;

			arr.push(map[data.hash] = {
				opts: mergedOpts,
				paths: []
			});
		}

		map[data.hash].paths.push(x);
	});

	return arr;
}
```
- example usage
```shell
...
		if (!(opts.overrides && opts.overrides.length > 0)) {
			return runEslint(paths, opts);
		}

		const overrides = opts.overrides;
		delete opts.overrides;

		const grouped = optionsManager.groupConfigs(paths, opts, overrides);

		return mergeReports(grouped.map(data => runEslint(data.paths, data.opts)));
	});
};

function mergeReports(reports) {
	// Merge multiple reports into a single report
...
```

#### <a name="apidoc.element.xo.options_manager.mergeApplicableOverrides"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>mergeApplicableOverrides (baseOptions, applicableOverrides)](#apidoc.element.xo.options_manager.mergeApplicableOverrides)
- description and source-code
```javascript
(baseOptions, applicableOverrides) => {
	applicableOverrides = applicableOverrides.map(normalizeOpts);
	const overrides = [emptyOptions(), baseOptions].concat(applicableOverrides);
	return deepAssign.apply(null, overrides);
}
```
- example usage
```shell
...
	if (opts.overrides && opts.overrides.length > 0) {
		const overrides = opts.overrides;
		delete opts.overrides;

		const filename = path.relative(opts.cwd, opts.filename);

		const foundOverrides = optionsManager.findApplicableOverrides(filename, overrides);
		opts = optionsManager.mergeApplicableOverrides(opts, foundOverrides.applicable);
	}

	opts = optionsManager.buildConfig(opts);
	const defaultIgnores = optionsManager.getIgnores({}).ignores;

	if (opts.ignores && !isEqual(defaultIgnores, opts.ignores) && typeof opts.filename !== 'string') {
		throw new Error('The 'ignores' option requires the 'filename' option to be defined.');
...
```

#### <a name="apidoc.element.xo.options_manager.mergeWithPkgConf"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>mergeWithPkgConf ({cwd: process.cwd()](#apidoc.element.xo.options_manager.mergeWithPkgConf)
- description and source-code
```javascript
opts => {
	opts = Object.assign({cwd: process.cwd()}, opts);
	const conf = pkgConf.sync('xo', {cwd: opts.cwd, skipOnFalse: true});
	return Object.assign({}, conf, opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xo.options_manager.normalizeOpts"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>normalizeOpts ({}, opts)](#apidoc.element.xo.options_manager.normalizeOpts)
- description and source-code
```javascript
opts => {
	opts = Object.assign({}, opts);

	// Alias to help humans
	[
		'env',
		'global',
		'ignore',
		'plugin',
		'rule',
		'setting',
		'extend',
		'extension'
	].forEach(singular => {
		const plural = singular + 's';
		let value = opts[plural] || opts[singular];

		delete opts[singular];

		if (value === undefined) {
			return;
		}

		if (singular !== 'rule' && singular !== 'setting') {
			value = arrify(value);
		}

		opts[plural] = value;
	});

	return opts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xo.options_manager.preprocess"></a>[function <span class="apidocSignatureSpan">xo.options_manager.</span>preprocess (opts)](#apidoc.element.xo.options_manager.preprocess)
- description and source-code
```javascript
opts => {
	opts = mergeWithPkgConf(opts);
	opts = normalizeOpts(opts);
	opts = getIgnores(opts);
	opts.extensions = DEFAULT_EXTENSION.concat(opts.extensions || []);

	return opts;
}
```
- example usage
```shell
...
const globby = require('globby');
const isEqual = require('lodash.isequal');
const multimatch = require('multimatch');
const arrify = require('arrify');
const optionsManager = require('./options-manager');

exports.lintText = (str, opts) => {
	opts = optionsManager.preprocess(opts);

	if (opts.overrides && opts.overrides.length > 0) {
		const overrides = opts.overrides;
		delete opts.overrides;

		const filename = path.relative(opts.cwd, opts.filename);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
