# npmdoc-electron-pdf

#### api documentation for  [electron-pdf (v1.3.0)](https://github.com/fraserxu/electron-pdf)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-pdf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-pdf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-pdf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-pdf)

#### A command line tool to generate PDF from URL, HTML or Markdown files

[![NPM](https://nodei.co/npm/electron-pdf.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-pdf)

- [https://npmdoc.github.io/node-npmdoc-electron-pdf/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Fraser Xu, Nate Good"
    },
    "ava": {
        "concurrency": 5,
        "failFast": true,
        "tap": true,
        "powerAssert": false
    },
    "bin": {
        "electron-pdf": "cli.js"
    },
    "bugs": {
        "url": "https://github.com/fraserxu/electron-pdf/issues"
    },
    "dependencies": {
        "async": "^2.0.1",
        "debug": "^2.3.2",
        "electron": "1.6.2",
        "eventemitter2": "^2.1.3",
        "github-markdown-css": "^2.0.9",
        "highlight.js": "^9.0.0",
        "lodash": "^4.16.2",
        "marked": "^0.3.5",
        "minimist": "^1.2.0",
        "object-assign": "^4.1.1",
        "uuid": "^2.0.1"
    },
    "description": "A command line tool to generate PDF from URL, HTML or Markdown files",
    "devDependencies": {
        "ava": "^0.18.0",
        "electron-ava": "^0.3.0",
        "jasmine": "^2.5.2",
        "standard": "^8.4.0",
        "tap-diff": "^0.1.1",
        "tap-spec": "^4.1.1",
        "validator": "^6.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "48236067439d63805359a04337d7cbb773a72c71",
        "tarball": "https://registry.npmjs.org/electron-pdf/-/electron-pdf-1.3.0.tgz"
    },
    "gitHead": "fef95e68a3bcf7b9294b497f7ecbaaea414d5898",
    "homepage": "https://github.com/fraserxu/electron-pdf",
    "keywords": [
        "electron",
        "electron-tool",
        "pdf",
        "png",
        "export",
        "render",
        "html",
        "markdown"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "codecounselor"
        },
        {
            "name": "fraserxu"
        }
    ],
    "name": "electron-pdf",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/fraserxu/electron-pdf.git"
    },
    "scripts": {
        "fix": "standard --fix",
        "lint": "standard",
        "test": "npm run fix && ava **/*-test.js | tap-diff && electron-ava --tap **/*-test-it.js | tap-diff",
        "unit-test": "ava | tap-diff"
    },
    "version": "1.3.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
