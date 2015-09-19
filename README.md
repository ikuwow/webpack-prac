webpack practice
==========

(based on this tutorial)

http://webpack.github.io/docs/tutorials/getting-started/

## Installation

Install node.js.

and install webpack.

```
$ npm install webpack -g
```

## Basic usage

```
$ webpack ./main.js bundle.js
```

## Using style-loader

### installation

```
npm install css-loader style-loader
```


### First usage

```entry.js
require("!style!css!./style.css");
```

```
$ webpack entry.js bundle.js
```

### Second usage

```entry.js
require("./style.css");
```

```
$ webpack entry.js bundle.js --module-bind 'css=style!css'
```
