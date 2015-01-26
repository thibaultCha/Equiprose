# Equiprose

![Build Status][travis-image]
![Coverage Status][coveralls-image] 
![npm version][npm-version-image]
![Downloads][npm-downloads-image]

Equiprose is a static website and blog generator built with [Node.js](http://nodejs.org).

- **[Features](#features)**
- **[Install](#install)**
- **[Documentation](#documentation)**
- **[Changelog](#changelog)**
- **[Roadmap](#roadmap)**
- **[Licence](#licence)**

## Features

- Static website + blog generator
- Shipped to you as a simple binary script
- Website preview
- Markdown support
- Native emojis support :+1:
- Write your template using [Jade](http://jade-lang.com) and [Stylus](http://learnboost.github.io/stylus/)
- Multiple and widely configurable websites

## Install

Node `0.10.0` or greater:

```
$ [sudo] npm install -g equiprose
```

Or:

Clone the master branch, add the `bin/` folder to your `$PATH`, run `make install` in the project root directory to install dependencies.

## Documentation

[Documentation is on the wiki](https://github.com/thibaultCha/Equiprose/wiki), but below is a sample so you can see how simple it is to use.

### Commands

- `$ equiprose -h`: prints help.

- `$ equiprose create [path]`: create a website at given path.

- `$ equiprose build [path]`: build the website at given path.

- `$ equiprose serve [path] [-p port]`: start a test server at given port (or 8888 by default).

- `$ equiprose new <page|post> [path]`: create a new page or post for website at given path.

NB: `path` always refers to a directory containing a `config.yml` file. If no `path` is provided, the command targets the current directory.

### Build your first website

`$ equiprose create ~/Desktop/test`

`$ equiprose serve ~/Desktop/test`

Browse to `http://localhost:8888`. That's it. (By the way, pull requests about the new templates are welcomed too).

## Development

Clone the sources and run `$ make dev` to install all dependencies.

`$ make test`: runs the tests.

`$ make test-cov`: runs the coverage.

## Changelog

### 1.1.0 (31/03/2014)
* Auto restart localhost server on Stylus, Jade or Markdown change.
* Some refactoring

### 1.0.4 (16/02/2014)
* Allow to ignore a post by prefixing it with an underscore `_`
* Fix posts order

### 1.0.2 (09/02/2014)
* Updated dependencies
* Updated Jade doctype in skeleton
* Print help on invalid command

### 1.0.1 (01/01/2013)
* Fix hidden files being removed on `build`
* Replaced custom search functions by [node-glob](https://github.com/isaacs/node-glob)
* Replaced custom object properties enumeration functions by a standalone module: [node-enumerate-properties](https://github.com/thibaultCha/node-enumerate-properties)

### 1.0.0 (03/12/2013)
* Initial release

## Roadmap

Refer to the [GitHub issues](https://github.com/thibaultCha/Equiprose/issues).

## License

Copyright (C) 2013-2014 by Thibault Charbonnier.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[travis-image]: https://img.shields.io/travis/thibaultCha/Equiprose.svg?style=flat

[coveralls-image]: https://img.shields.io/coveralls/thibaultCha/Equiprose/master.svg?style=flat

[npm-version-image]: https://img.shields.io/npm/v/equiprose.svg?style=flat

[npm-downloads-image]: https://img.shields.io/npm/dm/equiprose.svg?style=flat
