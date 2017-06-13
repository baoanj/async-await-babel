# async-await-babel

## About Code

Code from [setImmediate(callback[, ...args])](https://nodejs.org/api/timers.html#timers_setimmediate_callback_args)

## Run

Require `node >= v8.0.0`

npm install
npm run build
node index-babel

## Error and Solution

- ReferenceError: regeneratorRuntime is not defined

[ES6 写法报错regeneratorRuntime is not defined](https://segmentfault.com/q/1010000006801859)
[Polyfill](http://babeljs.io/docs/usage/polyfill/)
[Runtime transform](http://babeljs.io/docs/plugins/transform-runtime/)

使用`babel-polyfill`时需要将 `require("babel-polyfill");` 放到转码后的代码的头部（`'use strict';`下面）。

- TypeError: util.promisify is not a function

[util.promisify(original)](https://nodejs.org/dist/latest-v8.x/docs/api/util.html#util_util_promisify_original) `Added in: v8.0.0`

