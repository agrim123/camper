# CamperJS

[![Build Status](https://travis-ci.org/agrim123/camperjs.svg?branch=master)](https://travis-ci.org/agrim123/camperjs)

## Introduction

Generates a well organized directory structure for react applications.

## Installation

Add npm registry
```
npm set registry http://npm.vernacular.ai
```

```sh
$ [sudo] npm install -g camperjs
```

## Quick Start

The quickest way to get started with camperjs is to utilize the executable `camper` to generate an application as shown below:

Create the app:

```bash
$ camper myapp

   create : myapp
   create : myapp/package.json
   create : myapp/.babelrc
   create : myapp/.editorconfig
   create : myapp/.eslintrc.json
   create : myapp/.flowconfig
   create : myapp/webpack.config.babel.js
   create : myapp/src
   create : myapp/src/client
   create : myapp/src/client/app.jsx
   create : myapp/src/client/index.jsx
   create : myapp/src/server
   create : myapp/src/server/app.js
   create : myapp/src/server/index.js
   create : myapp/src/shared
   create : myapp/src/shared/config.js
   create : myapp/src/shared/util.js
   create : myapp/src/client/action
   create : myapp/src/client/action/hello.js
   create : myapp/src/client/reducer
   create : myapp/src/client/reducer/hello.js

   install dependencies:
     $ cd myapp && yarn install

   run the app:
     $ DEBUG=myapp:* yarn start


```

Install dependencies:

```bash
$ yarn install
```

Start your app at `http://localhost:8000/`:

```bash
$ yarn start
```

## File Structure

```bash
myapp
|
|____src
|      |
|      |____client
|      |    |____app.jsx
|      |    |____index.jsx
|      |
|      |____server
|      |    |____app.js
|      |    |___index.js
|      |
|      |____shared
|           |___home.js
|           |___util.js
|           |___action
|           |   |___hello.js
|           |___reducer
|               |___hello.js
|
|_____.babelrc
|
|_____.editorconfig
|
|_____.eslintrc.json
|
|_____.flowconfig
|
|_____webpack.config.babel.js
|
|_____package.json

```
## Command Line Options

This generator can also be further configured with the following command line flags.
```bash

  Usage: camper [options] [dir]

  Options:

    -h, --help     output usage information
        --version  output the version number
    -f, --force    force on non-empty directory

```

## License

[MIT](LICENSE)
