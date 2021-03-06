# Lo-Dash v1.0.2

A utility library delivering consistency, [customization](https://lodash.com/custom-builds), [performance](https://lodash.com/benchmarks), & [extras](https://lodash.com/#features).

## Download

* Lo-Dash builds (for modern environments):<br>
[Development](https://raw.github.com/lodash/lodash/1.0.2/dist/lodash.js) and
[Production](https://raw.github.com/lodash/lodash/1.0.2/dist/lodash.min.js)

* Lo-Dash compatibility builds (for legacy and modern environments):<br>
[Development](https://raw.github.com/lodash/lodash/1.0.2/dist/lodash.compat.js) and
[Production](https://raw.github.com/lodash/lodash/1.0.2/dist/lodash.compat.min.js)

* Underscore compatibility builds:<br>
[Development](https://raw.github.com/lodash/lodash/1.0.2/dist/lodash.underscore.js) and
[Production](https://raw.github.com/lodash/lodash/1.0.2/dist/lodash.underscore.min.js)

* For optimal file size, [create a custom build](https://lodash.com/custom-builds) with only the features you need

## Dive in

We’ve got [API docs](https://lodash.com/docs), [benchmarks](https://lodash.com/benchmarks), and [unit tests](https://lodash.com/tests).

For a list of upcoming features, check out our [roadmap](https://github.com/lodash/lodash/wiki/Roadmap).

The full changelog is available [here](https://github.com/lodash/lodash/wiki/Changelog).

## Installation and usage

In browsers:

```html
<script src="lodash.js"></script>
```

Using [`npm`](http://npmjs.org/):

```bash
npm install lodash

npm install -g lodash
npm link lodash
```

To avoid potential issues, update `npm` before installing Lo-Dash:

```bash
npm install npm -g
```

In [Node.js](http://nodejs.org/) and [RingoJS v0.8.0+](http://ringojs.org/):

```js
var _ = require('lodash');

// or as a drop-in replacement for Underscore
var _ = require('lodash/lodash.underscore');
```

**Note:** If Lo-Dash is installed globally, run [`npm link lodash`](http://blog.nodejs.org/2011/03/23/npm-1-0-global-vs-local-installation/) in your project’s root directory before requiring it.

In [RingoJS v0.7.0-](http://ringojs.org/):

```js
var _ = require('lodash')._;
```

In [Rhino](http://www.mozilla.org/rhino/):

```js
load('lodash.js');
```

In an AMD loader like [RequireJS](http://requirejs.org/):

```js
require({
  'paths': {
    'underscore': 'path/to/lodash'
  }
},
['underscore'], function(_) {
  console.log(_.VERSION);
});
```

## Resources

For more information check out these articles, screencasts, and other videos over Lo-Dash:

 * Posts
  - [Say “Hello” to Lo-Dash](http://kitcambridge.be/blog/say-hello-to-lo-dash/)

 * Videos
  - [Introducing Lo-Dash](https://vimeo.com/44154599)
  - [Lo-Dash optimizations and custom builds](https://vimeo.com/44154601)
  - [Lo-Dash’s origin and why it’s a better utility belt](https://vimeo.com/44154600)
  - [Unit testing in Lo-Dash](https://vimeo.com/45865290)
  - [Lo-Dash’s approach to native method use](https://vimeo.com/48576012)
  - [CascadiaJS: Lo-Dash for a better utility belt](http://www.youtube.com/watch?v=dpPy4f_SeEk)

## Features

 * AMD loader support ([RequireJS](http://requirejs.org/), [curl.js](https://github.com/cujojs/curl), etc.)
 * [_(…)](https://lodash.com/docs#_) supports intuitive chaining
 * [_.at](https://lodash.com/docs#at) for cherry-picking collection values
 * [_.bindKey](https://lodash.com/docs#bindKey) for binding [*“lazy”* defined](http://michaux.ca/articles/lazy-function-definition-pattern) methods
 * [_.cloneDeep](https://lodash.com/docs#cloneDeep) for deep cloning arrays and objects
 * [_.contains](https://lodash.com/docs#contains) accepts a `fromIndex` argument
 * [_.forEach](https://lodash.com/docs#forEach) is chainable and supports exiting iteration early
 * [_.forIn](https://lodash.com/docs#forIn) for iterating over an object’s own and inherited properties
 * [_.forOwn](https://lodash.com/docs#forOwn) for iterating over an object’s own properties
 * [_.isPlainObject](https://lodash.com/docs#isPlainObject) checks if values are created by the `Object` constructor
 * [_.merge](https://lodash.com/docs#merge) for a deep [_.extend](https://lodash.com/docs#extend)
 * [_.partial](https://lodash.com/docs#partial) and [_.partialRight](https://lodash.com/docs#partialRight) for partial application without `this` binding
 * [_.template](https://lodash.com/docs#template) supports [*“imports”* options](https://lodash.com/docs#templateSettings_imports), [ES6 template delimiters](http://people.mozilla.org/~jorendorff/es6-draft.html#sec-7.8.6), and [sourceURLs](http://www.html5rocks.com/en/tutorials/developertools/sourcemaps/#toc-sourceurl)
 * [_.where](https://lodash.com/docs#where) supports deep object comparisons
 * [_.clone](https://lodash.com/docs#clone), [_.omit](https://lodash.com/docs#omit), [_.pick](https://lodash.com/docs#pick),
   [and more…](https://lodash.com/docs "_.assign, _.cloneDeep, _.first, _.initial, _.isEqual, _.last, _.merge, _.rest") accept `callback` and `thisArg` arguments
 * [_.contains](https://lodash.com/docs#contains), [_.size](https://lodash.com/docs#size), [_.toArray](https://lodash.com/docs#toArray),
   [and more…](https://lodash.com/docs "_.at, _.countBy, _.every, _.filter, _.find, _.forEach, _.groupBy, _.invoke, _.map, _.max, _.min, _.pluck, _.reduce, _.reduceRight, _.reject, _.shuffle, _.some, _.sortBy, _.where") accept strings
 * [_.filter](https://lodash.com/docs#filter), [_.find](https://lodash.com/docs#find), [_.map](https://lodash.com/docs#map),
   [and more…](https://lodash.com/docs "_.countBy, _.every, _.first, _.groupBy, _.initial, _.last, _.max, _.min, _.reject, _.rest, _.some, _.sortBy, _.sortedIndex, _.uniq") support *“_.pluck”* and *“_.where”* `callback` shorthands

## Support

Lo-Dash has been tested in at least Chrome 5~24, Firefox 1~18, IE 6-10, Opera 9.25-12, Safari 3-6, Node.js 0.4.8-0.8.20, Narwhal 0.3.2, PhantomJS 1.8.1, RingoJS 0.9, and Rhino 1.7RC5.
