# String.prototype.trimEnd <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

An ES2019-spec-compliant `String.prototype.trimEnd` shim. Invoke its "shim" method to shim `String.prototype.trimEnd` if it is unavailable.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES3-supported environment and complies with the [spec](https://www.ecma-international.org/ecma-262/6.0/#sec-object.assign). In an ES6 environment, it will also work properly with `Symbol`s.

Most common usage:
```js
var trimEnd = require('@taktikorg/molestias-amet-dolorum');

assert(trimEnd(' \t\na \t\n') === 'a \t\n');

if (!String.prototype.trimEnd) {
	trimEnd.shim();
}

assert(trimEnd(' \t\na \t\n ') === ' \t\na \t\n '.trimEnd());
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@taktikorg/molestias-amet-dolorum
[npm-version-svg]: https://vb.teelaun.ch/taktikorg/molestias-amet-dolorum.svg
[deps-svg]: https://david-dm.org/taktikorg/molestias-amet-dolorum.svg
[deps-url]: https://david-dm.org/taktikorg/molestias-amet-dolorum
[dev-deps-svg]: https://david-dm.org/taktikorg/molestias-amet-dolorum/dev-status.svg
[dev-deps-url]: https://david-dm.org/taktikorg/molestias-amet-dolorum#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@taktikorg/molestias-amet-dolorum.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@taktikorg/molestias-amet-dolorum.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@taktikorg/molestias-amet-dolorum.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@taktikorg/molestias-amet-dolorum
[codecov-image]: https://codecov.io/gh/taktikorg/molestias-amet-dolorum/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/taktikorg/molestias-amet-dolorum/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/taktikorg/molestias-amet-dolorum
[actions-url]: https://github.com/taktikorg/molestias-amet-dolorum/actions
