# changelogkeeper [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url] [![Coverage percentage][coveralls-image]][coveralls-url]

> Write changelog using [keepachangelog](https://keepachangelog.com/en/1.0.0/) conventions

## Installation

```sh
$ npm install --save-dev changelogkeeper
```

## Usage

Add these scripts to package.json:

```json
"scripts": {
  "commitChangelog": "git add CHANGELOG.md && git commit -m 'Bump changelog'",
  "postversion": "npm run changelogkeeper && npm run commitChangelog"
}
```

And then run [npm version](https://docs.npmjs.com/cli/version.html):

```sh
npm version [major | minor | patch | ...]
```

It will read the package version and update the changelog accordingly.

## License

MIT © [Francisco Kahil]()

[npm-image]: https://badge.fury.io/js/changelogkeeper.svg
[npm-url]: https://npmjs.org/package/changelogkeeper
[travis-image]: https://travis-ci.org/codexico/changelogkeeper.svg?branch=master
[travis-url]: https://travis-ci.org/codexico/changelogkeeper
[daviddm-image]: https://david-dm.org/codexico/changelogkeeper.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/codexico/changelogkeeper
[coveralls-image]: https://coveralls.io/repos/codexico/changelogkeeper/badge.svg
[coveralls-url]: https://coveralls.io/r/codexico/changelogkeeper
