# Brave Chromium Extension

[![Build Status](https://travis-ci.org/brave/brave-extension.svg?branch=master)](https://travis-ci.org/brave/brave-extension)

> Experiment moving part of the Brave UI into an extension for use in Brave only (Not Chrome, it will use APIs not available in Chrome)

## Installation

```bash
# clone it
$ git clone git@github.com:brave/brave-extension.git

# Install dependencies
$ cd brave-extension
$ yarn install
```

## Development

* Run script
```bash
# Build files will appear in './dev'
# Start webpack development server
$ yarn run dev
```

#### Building release

## Build

```bash
# build files to './build'
$ yarn run build
```

## Compress

```bash
# compress build folder to {manifest.name}.zip and crx
$ yarn run build
$ yarn run compress -- [options]
```

## Test

* `test/app`: React components, Redux actions & reducers tests
* `test/e2e`: E2E tests (use [chromedriver](https://www.npmjs.com/package/chromedriver), [selenium-webdriver](https://www.npmjs.com/package/selenium-webdriver))

```bash
# lint
$ yarn run lint
# test/app
$ yarn test
$ yarn test -- --watch  # watch files
# test/e2e
$ yarn run build
$ yarn run test-e2e
```

## LICENSE

[MPL-2](LICENSE)
