# Craco Csv Loader Plugin

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

This is a [craco](https://github.com/sharegate/craco) plugin that makes it easy to use the webpack [csv-loader](https://github.com/theplatapi/csv-loader) with [create-react-app](https://facebook.github.io/create-react-app/).

## Installation

```bash
$ npm install craco-csv-loader --save-dev

# OR

$ yarn add -D craco-csv-loader
```

## Basic Usage

`craco-csv-loader` tests for `.csv` files by default. You can provide any option that you can normally provide to the [csv-loader](https://github.com/theplatapi/csv-loader)

Here is a simple `craco.config.js` example for `.csv` files:

```js
const csvLoader = require('craco-csv-loader')

module.exports = {
    webpack: {
        plugins: [
        {
            plugin: csvPlugin,
            options: {
                dynamicTyping: true,
                header: true,
                skipEmptyLines: true
            },
        }
    ]
}
```
