<h1 align="center">
    <img width="120" height="120" src="https://grigorys.me/images/dixi.png">
</h1>

[![Travis](https://img.shields.io/travis/rust-lang/rust/master.svg?style=flat-square)](https://travis-ci.org/Grigory90/dixi)

> Simply project builder based on Gulp 4 and Webpack 2.

## Installation

```
$ npm i -g dixi
```

## Usage in your project

Run init command in the project root directory:

``` bash
$ dixi init -s     # key -s create samples folder, optional
```

Set the base options in **dixi.config.js** file:

``` javascript
{

    revision: false,     // appends content hash to each filename

    deploy: false,       // deploy project using ftp

    archive: false,      // create build zip

}
```

Start server and watchers:

```
$ dixi run
```

## Project structure:

``` bash
.
├─ app                   
│   ├─ src
│   │   ├─ twig
│   │   ├─ icons
│   │   ├─ img
│   │   ├─ js
│   │   ├─ scss
│   │   └─ static
│   ├─ dev          
│   └─ build
├─ dixi.config.js
└─ package.json
```

## Commands:

``` bash
$ dixi                      # reference

$ dixi init [-s, --sample]  # create config file
                            # [-s, --sample] create samples folder

$ dixi run                  # start server and watchers

$ dixi build                # build project
```
