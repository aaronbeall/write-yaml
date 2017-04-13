# write-yaml [![NPM version](https://img.shields.io/npm/v/write-yaml.svg?style=flat)](https://www.npmjs.com/package/write-yaml) [![NPM monthly downloads](https://img.shields.io/npm/dm/write-yaml.svg?style=flat)](https://npmjs.org/package/write-yaml) [![Linux Build Status](https://img.shields.io/travis/jonschlinkert/write-yaml.svg?style=flat&label=Travis)](https://travis-ci.org/jonschlinkert/write-yaml)

> Write YAML. Converts JSON to YAML writes it to the specified file.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save write-yaml
```

Install with [yarn](https://yarnpkg.com):

```sh
$ yarn add write-yaml
```

## Usage

Add to your javascript/node.js application with the following line of code:

```js
var yaml = require('write-yaml');
```

### async

```js
var data = {language: 'node_js', node_js: ['0.10', '0.11']};

yaml('.travis.yml', data, function(err) {
  // do stuff with err
});
```

Would write `.travis.yml` to disk with the following contents:

```yaml
language: node_js
node_js:
  - "0.10"
  - "0.11"
```

### sync

```js
yaml.sync('.travis.yml', data);
```

Would write `.travis.yml` to disk with the following contents:

```yaml
language: node_js
node_js:
  - "0.10"
  - "0.11"
```

## About

### Related projects

* [read-data](https://www.npmjs.com/package/read-data): Read JSON or YAML files. | [homepage](https://github.com/jonschlinkert/read-data "Read JSON or YAML files.")
* [read-yaml](https://www.npmjs.com/package/read-yaml): Very thin wrapper around js-yaml for directly reading in YAML files. | [homepage](https://github.com/jonschlinkert/read-yaml "Very thin wrapper around js-yaml for directly reading in YAML files.")
* [write-data](https://www.npmjs.com/package/write-data): Write a YAML or JSON file to disk. Automatically detects the format to write based… [more](https://github.com/jonschlinkert/write-data) | [homepage](https://github.com/jonschlinkert/write-data "Write a YAML or JSON file to disk. Automatically detects the format to write based on extension. Or pass `ext` on the options.")
* [write-json](https://www.npmjs.com/package/write-json): Write a JSON file to disk, also creates intermediate directories in the destination path if… [more](https://github.com/jonschlinkert/write-json) | [homepage](https://github.com/jonschlinkert/write-json "Write a JSON file to disk, also creates intermediate directories in the destination path if they don't already exist.")

### Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

### Contributors

| **Commits** | **Contributor** | 
| --- | --- |
| 12 | [jonschlinkert](https://github.com/jonschlinkert) |
| 2 | [shinnn](https://github.com/shinnn) |

### Building docs

_(This project's readme.md is generated by [verb](https://github.com/verbose/verb-generate-readme), please don't edit the readme directly. Any changes to the readme must be made in the [.verb.md](.verb.md) readme template.)_

To generate the readme, run the following command:

```sh
$ npm install -g verbose/verb#dev verb-generate-readme && verb
```

### Running tests

Running and reviewing unit tests is a great way to get familiarized with a library and its API. You can install dependencies and run tests with the following command:

```sh
$ npm install && npm test
```

### Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](https://twitter.com/jonschlinkert)

### License

Copyright © 2017, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT License](LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.5.0, on April 12, 2017._