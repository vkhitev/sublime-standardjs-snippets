# Standard JavaScript Snippets for Sublime Text

A collection of [standardjs code style](http://standardjs.com/) snippets for JavaScript development in [Sublime Text](https://www.sublimetext.com/).

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

__Yes!, no semicolons:__
- [Are Semicolons Necessary in JavaScript?](https://www.youtube.com/watch?v=gsfbh17Ax9I)
- [An Open Letter to JavaScript Leaders Regarding Semicolons](http://blog.izs.me/post/2353458699/an-open-letter-to-javascript-leaders-regarding)
- [JavaScript Semicolon Insertion - Everything You Need to Know](http://inimino.org/~inimino/blog/javascript_semicolons)

## Installation

### Installation via Package Control
1. Open PackageControl (Ctrl+Shift+P).
2. Type and press 'Install Package'.
3. Find and install 'StandardSnippets'

### Manual installation
1. Preferences - Browse Packages.
2. Add content of this repo anywhere.

## Disabling default snippets
##### You don't need them with this beautiful package!
1. Install PackageResourceViewer via Package Control (Ctrl+Shift+P - Install Package - PackageResourceViewer).
2. Extract JavaScript package (Ctrl+Shift+P - Extract - JavaScript).
3. Open packages folder (Preferences - Browse Packages).
4. Remove JavaScript/Snippets and rename JavaScript folder to any other (e.g. JavaScript-custom).
5. Add JavaScript to ignored packages (Ctrl+Shift+P - Disable Package - JavaScript)

# Contents

- [declarations](#declarations)
- [flow control](#flow-control)
- [functions](#functions)
- [iterables](#iterables)
- [objects and classes](#objects-and-classes)
- [returning values](#returning-values)
- [types](#types)
- [promises](#promises)
- [ES6 modules](#es6-modules)
- [testing](#testing)
- [console](#console)
- [timers](#timers)
- [DOM](#dom)
- [Node.js](#nodejs)
- [miscellaneous](#miscellaneous)

### Declarations

#### `l⇥` let assignment
```js
let ${1:name} = ${2:value}
```

#### `co⇥` const assignment
```js
const ${1:name} = ${2:value}
```

#### `yi⇥` const assignment
```js
yield ${1:value}
```

### Flow Control

#### `if⇥` if statement
```js
if (${1:condition}) {
  ${0}
}
```

#### `el⇥` else statement
```js
else {
  ${0}
}
```

#### `ife⇥` else statement
```js
if (${1:condition}) {
  ${0}
} else {

}
```

#### `ei⇥` else if statement
```js
else if (${1:condition}) {
  ${0}
}
```

#### `for⇥` for loop
```js
for (let ${1:i} = ${2:start}; ${1:i} < ${3:end}; ${1:i} += 1) {
  ${0}
}
```

#### `rfor⇥` reversed for loop
```js
for (let ${1:i} = ${2:start}; ${1:i} >= ${3:end}; ${1:i} -= 1) {
  ${0}
}
```

#### `fi⇥` for in loop
```js
for (const ${1:key} in ${2:collection}) {
  ${0}
}
```

#### `fo⇥` for of loop
```js
for (const ${1:value} of ${2:collection}) {
  ${0}
}
}
```

#### `wl⇥` while loop
```js
while (${1:condition}) {
  ${0}
}
```

#### `tc⇥` try/catch
```js
try {
 ${0}
} catch (${1:err}) {

}
```

#### `tf⇥` try/finally
```js
try {
 ${0}
} finally {

}
```

#### `tcf⇥` try/catch/finally
```js
try {
  ${0}
} catch (${1:err}) {

} finally {

}
```

### Functions

#### `fun⇥` anonymous function
```js
function (${1:arguments}) {
  ${0}
}
```

#### `fn⇥` named function
```js
function ${1:name} (${2:arguments}) {
  ${0}
}
```

#### `fas⇥` function assignment
```js
const ${1:name} = function ${1:name} (${2:arguments}) {
  ${0}
}
```

#### `iife⇥` immediately-invoked function expression (IIFE)
```js
;(function (${1:arguments}) {
  ${0}
})(${2})
```

#### `af⇥` arrow function
```js
(${1:arguments}) => ${2:statement}
```

#### `afb⇥` arrow function with body
```js
(${1:arguments}) => {
  ${0}
}
```

#### `gfun⇥` generator function
```js
function* (${1:arguments}) {
  ${0}
}
```

#### `gfn⇥` named generator function
```js
function* ${1:name}(${1:arguments}) {
  ${0}
}
```

#### `gfn⇥` generator assignment
```js
const ${1:name} = function* ${1:name} (${2:arguments}) {
  ${0}
}
```

### Iterables

#### `fe⇥` forEach loop
```js
forEach((${2:item}) => {
  ${0}
})
```

#### `map⇥` map function
```js
map((${2:item}) => {
  ${0}
})
```

#### `reduce⇥` reduce function
```js
reduce((${2:previous}, ${3:current}) => {
  ${0}
}${4:, initial})
```

#### `filter⇥` filter function
```js
filter((${2:item}) => {
  ${0}
})
```

#### `find⇥` ES6 find function
```js
find((${2:item}) => {
  ${0}
})
```

#### `every⇥` every function
```js
every((${2:item}) => {
  ${0}
})
```

#### `some⇥` some function
```js
some((${2:item}) => {
  ${0}
})
```

### Objects and classes

#### `cs⇥` class (ES6)
```js
class ${1:name} {
  constructor(${2:arguments}) {
    ${0}
  }
}
```

#### `csx⇥` child class (ES6)
```js
class ${1:name} extends ${2:base} {
  constructor(${2:arguments}) {
    super(${2:arguments})
    ${0}
  }
}
```

#### `kv⇥` key/value pair
Javascript:
```js
${1:key}: ${2:'value'}
```
JSON:
```json
"${1:key}": ${2:"value"}
```

#### `m⇥` method (ES6 syntax)
```js
${1:method}(${2:arguments}) {
  ${0}
}
```

#### `proto⇥` prototype method (chainable)
```js
${1:Class}.prototype.${2:methodName} = function (${3:arguments}) {
  ${0}
}
```

#### `ok` Object.keys
```js
Object.keys(${1:obj})
```

#### `oa` Object.assign
```js
Object.assign(${1:dest}, ${2:source})
```

#### `hop⇥` has own property
```js
Object.prototype.hasOwnProperty.call(${1:object}, ${2:key})
```

### Returning values

#### `ret⇥` return
```js
return ${0}
```

#### `rp⇥` return Promise (ES6)
```js
return new Promise((resolve, reject) => {
  ${0}
})
```

### Types

#### `S⇥` String
#### `N⇥` Number
#### `O⇥` Object
#### `A⇥` Array
#### `D⇥` Date
#### `Rx⇥` RegExp

#### `tof⇥` typeof comparison
```js
typeof ${1:source} === '${2:undefined}'
```

#### `iof⇥` instanceof comparison
```js
${1:source} instanceof ${2:Object}
```

#### `ia⇥` isArray
```js
Array.isArray(${1:source})
```

### Promises

#### `p⇥` new Promise (ES6)
```js
new Promise((resolve, reject) => {
  ${0}
})
```

#### `then⇥` Promise.then (chainable)
```js
${1:promise}.then((${2:value}) => {
  ${0}
})
```

#### `catch⇥` Promise.catch (chainable)
```js
${1:promise}.catch((${2:err}) => {
  ${0}
})
```

### ES6 modules

#### `exp⇥` module export
```js
export ${1:member}
```

#### `exd⇥` module default export
```js
export default ${1:member}
```

#### `imp⇥` module import
```js
import ${1:*} from '${2:module}'
```

#### `ima⇥` module import as
```js
import ${1:*} as ${2:name} from '${3:module}'
```

#### `imd⇥` module import destructuring
```js
import {$1} from '${2:module}'
```

### BDD testing (Mocha, Jasmine, etc.)

#### `desc⇥` describe
```js
describe('${1:description}', function () {
  ${0}
})
```
#### `its⇥` synchronous "it"
```js
it('${1:description}', function () {
  ${0}
})
```
#### `ita⇥` asynchronous "it"
```js
it('${1:description}', function (done) {
  ${0}
})
```

#### `bf⇥` before test suite
```js
before(function () {
  ${0}
})
```

#### `bfe⇥` before each test
```js
beforeEach(function () {
  ${0}
})
```

#### `aft⇥` after test suite
```js
after(function () {
  ${0}
})
```

#### `afe⇥` after each test
```js
afterEach(function () {
  ${0}
})
```

### Timers

#### `st⇥` setTimeout
```js
setTimeout(() => {
  ${0}
}, ${1:delay})
```

#### `si⇥` setInterval
```js
setInterval(() => {
  ${0}
}, ${1:delay})
```

#### `sim⇥` setImmediate
```js
setImmediate(() => {
  ${0}
})
```

### DOM

#### `ae⇥` addEventListener
```js
${1:document}.addEventListener('${2:event}', ${3:ev} => {
  ${0}
})
```

#### `rel⇥` removeEventListener
```js
${1:document}.removeEventListener('${2:event}', ${3:listener})
```

#### `gi⇥` getElementById
```js
${1:document}.getElementById('${2:id}')
```

#### `gc⇥` getElementsByClassName
```js
Array.from(${1:document}.getElementsByClassName('${2:class}'))
```

#### `gt⇥` getElementsByTagName
```js
Array.from(${1:document}.getElementsByTagName('${2:tag}'))
```

#### `qs⇥` querySelector
```js
${1:document}.querySelector('${2:selector}')
```

#### `qsa⇥` querySelectorAll
```js
Array.from(${1:document}.querySelectorAll('${2:selector}'))
```

### `cdf⇥` createDocumentFragment

```js
${1:document}.createDocumentFragment(${2:elem});
```

### `cel⇥` createElement

```js
${1:document}.createElement(${2:elem});
```

### `ac⇥` appendChild

```js
${1:document}.appendChild(${2:elem});
```

### `rc⇥` removeChild

```js
${1:document}.removeChild(${2:elem});
```

### `cla⇥` classList.add

```js
${1:document}.classList.add('${2:class}');
```

### `ct⇥` classList.toggle

```js
${1:document}.classList.toggle('${2:class}');
```

### `cr⇥` classList.remove

```js
${1:document}.classList.remove('${2:class}');
```

### `ga⇥` getAttribute

```js
${1:document}.getAttribute('${2:attr}');
```

### `sa⇥` setAttribute

```js
${1:document}.setAttribute('${2:attr}', ${3:value});
```

### `ra⇥` removeAttribute

```js
${1:document}.removeAttribute('${2:attr}');
```

### Node.js

#### `cb⇥` Node.js callback
```js
(err, ${1:arguments}) => {
  if (err) {
    throw err
  }
  ${0}
}
```

#### `req⇥` require a module
```js
require('${1:module}')
```
#### `cre⇥` require and assign a module
```js
const ${1:module} = require('${2:module}')
```

#### `em⇥` export member
```js
exports.${1:name} = ${2:value}
```

#### `me⇥` module.exports
```js
module.exports = ${1:name}
```

#### `on⇥` attach an event handler
```js
on('${1:event}', (${2:arguments}) => {
  ${0}
})
```

#### `xm⇥` Express middleware
```js
(req, res${1:, next}) => {
  ${0}
}
```

#### `xerr⇥` Express error handler
```js
(err, req, res, next) => {
  ${0}
}
```

### Miscellaneous

#### `us⇥` use strict
```js
'use strict'
```

#### `js⇥` JSON Stringify
```js
JSON.stringify($0)
```

#### `jp⇥` JSON Parse
```js
JSON.parse($0)
```

#### `car⇥` copy array
```js
const ${1:copy} = [...${2:original}${3:, new}]
```

#### `cas⇥` copy assign
```js
const ${1:copy} = { ...${2:original}${3:, new} }
```

#### `swap⇥` swap values
```js
[${1}, ${2}] = [${2}, ${1}]
```

### Console

#### `cl⇥` console.log
```js
console.log(${0})
```

#### `ce⇥` console.error
```js
console.error(${0})
```

#### `cw⇥` console.warn
```js
console.warn(${0})
```

#### `cd⇥` console.dir
```js
console.dir(${0})
```

# Contributing
More than happy to accept external contributions to the project in the form of feedback, bug reports and even better pull requests.
Please read the [contributing guidelines](contributing.md)

# Related Repositories
- [Standard Linter](https://github.com/Flet/SublimeLinter-contrib-standard)
- [Standard Formatter](https://github.com/bcomnes/sublime-standard-format)

# Alternatives to Standard Style
- [Semistandard](https://github.com/Flet/semistandard) - standard, with semicolons
- [XO](https://github.com/sindresorhus/xo) - JavaScript happiness style, by Sindre Sorhus

# License

The MIT License (MIT)

Copyright (c) 2017, [Vlad Khitev](https://github.com/vkhitev/)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
