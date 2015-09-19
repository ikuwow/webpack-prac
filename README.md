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

### Third usage

Write `webpack.config.js` and just type:

```
$ webpack
```

## prettier output

```
$ webpack --progress --colors
```

## Watch mode

```
$ webpack --progress --colors --watch
```

## development server

```
$ npm install webpack-dev-server -g
```

```
$ webpack-dev-server --progress --colors
```


It builds simple express server, 
and you can open http://localhost:8080/webpack-dev-server/bundle.

