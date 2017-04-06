# api documentation for  [electron-pdf (v1.2.0)](https://github.com/fraserxu/electron-pdf)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-pdf.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-pdf) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-pdf.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-pdf)
#### A command line tool to generate PDF from URL, HTML or Markdown files

[![NPM](https://nodei.co/npm/electron-pdf.png?downloads=true)](https://www.npmjs.com/package/electron-pdf)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-electron-pdf_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-pdf/build/apidoc.html)

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
        "electron": "1.4.15",
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
        "shasum": "30947174437f352c049d7e55cd633aca637c8c7a",
        "tarball": "https://registry.npmjs.org/electron-pdf/-/electron-pdf-1.2.0.tgz"
    },
    "gitHead": "4f076bb17183541e7fc8400b8df0f5da034e5e5a",
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
            "name": "codecounselor",
            "email": "codecounselor@gmail.com"
        },
        {
            "name": "fraserxu",
            "email": "xvfeng123@gmail.com"
        }
    ],
    "name": "electron-pdf",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "1.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module electron-pdf](#apidoc.module.electron-pdf)
1.  [function <span class="apidocSignatureSpan">electron-pdf.</span>logger ()](#apidoc.element.electron-pdf.logger)
1.  object <span class="apidocSignatureSpan">electron-pdf.</span>args
1.  object <span class="apidocSignatureSpan">electron-pdf.</span>windowMaid
1.  object <span class="apidocSignatureSpan">electron-pdf.</span>windowTailor

#### [module electron-pdf.args](#apidoc.module.electron-pdf.args)
1.  [function <span class="apidocSignatureSpan">electron-pdf.args.</span>encode (args)](#apidoc.element.electron-pdf.args.encode)
1.  [function <span class="apidocSignatureSpan">electron-pdf.args.</span>urlWithArgs (urlOrFile, args)](#apidoc.element.electron-pdf.args.urlWithArgs)

#### [module electron-pdf.logger](#apidoc.module.electron-pdf.logger)
1.  [function <span class="apidocSignatureSpan">electron-pdf.</span>logger ()](#apidoc.element.electron-pdf.logger.logger)
1.  [function <span class="apidocSignatureSpan">electron-pdf.logger.</span>debug ()](#apidoc.element.electron-pdf.logger.debug)
1.  [function <span class="apidocSignatureSpan">electron-pdf.logger.</span>error ()](#apidoc.element.electron-pdf.logger.error)
1.  [function <span class="apidocSignatureSpan">electron-pdf.logger.</span>info ()](#apidoc.element.electron-pdf.logger.info)
1.  [function <span class="apidocSignatureSpan">electron-pdf.logger.</span>set (loggerObj)](#apidoc.element.electron-pdf.logger.set)

#### [module electron-pdf.windowMaid](#apidoc.module.electron-pdf.windowMaid)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>cleanupHungWindows (threshold)](#apidoc.element.electron-pdf.windowMaid.cleanupHungWindows)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>registerOpenWindow (exportJob)](#apidoc.element.electron-pdf.windowMaid.registerOpenWindow)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>removeWindow (id)](#apidoc.element.electron-pdf.windowMaid.removeWindow)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>touchWindow (id)](#apidoc.element.electron-pdf.windowMaid.touchWindow)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>windowCount ()](#apidoc.element.electron-pdf.windowMaid.windowCount)

#### [module electron-pdf.windowTailor](#apidoc.module.electron-pdf.windowTailor)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowTailor.</span>getPageDimensions (pageSize, landscape)](#apidoc.element.electron-pdf.windowTailor.getPageDimensions)
1.  [function <span class="apidocSignatureSpan">electron-pdf.windowTailor.</span>setWindowDimensions (window, pageSize, landscape)](#apidoc.element.electron-pdf.windowTailor.setWindowDimensions)
1.  number <span class="apidocSignatureSpan">electron-pdf.windowTailor.</span>HTML_DPI



# <a name="apidoc.module.electron-pdf"></a>[module electron-pdf](#apidoc.module.electron-pdf)

#### <a name="apidoc.element.electron-pdf.logger"></a>[function <span class="apidocSignatureSpan">electron-pdf.</span>logger ()](#apidoc.element.electron-pdf.logger)
- description and source-code
```javascript
function info() {
  loggers[LEVELS.info](...arguments)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-pdf.args"></a>[module electron-pdf.args](#apidoc.module.electron-pdf.args)

#### <a name="apidoc.element.electron-pdf.args.encode"></a>[function <span class="apidocSignatureSpan">electron-pdf.args.</span>encode (args)](#apidoc.element.electron-pdf.args.encode)
- description and source-code
```javascript
function encode(args) {
  assert.strictEqual(typeof args, 'object', 'args must be an object')
  // stringify the args
  args = args ? encodeURIComponent(JSON.stringify(args)) : ''
  return args
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-pdf.args.urlWithArgs"></a>[function <span class="apidocSignatureSpan">electron-pdf.args.</span>urlWithArgs (urlOrFile, args)](#apidoc.element.electron-pdf.args.urlWithArgs)
- description and source-code
```javascript
function urlWithArgs(urlOrFile, args) {
  args = encode(args)

  var u
  if (urlOrFile.indexOf('http') === 0) {
    var urlData = url.parse(urlOrFile)
    var hash = urlData.hash || args ? args : undefined
    u = url.format(assign(urlData, { hash: hash }))
  } else { // presumably a file url
    u = url.format({
      protocol: 'file',
      pathname: path.resolve(urlOrFile),
      slashes: true,
      hash: args
    })
  }

  return u
}
```
- example usage
```shell
...
 */
_loadURL (window, url) {
  const loadOpts = {}
  if (this.args.disableCache) {
    loadOpts.extraHeaders += 'pragma: no-cache\n'
  }
  this.emit('${RENDER_EVENT_PREFIX}loadurl', { url: url })
  window.loadURL(wargs.urlWithArgs(url, {}), loadOpts)
}

// Page Load & Rendering

/**
 * Injects a wait if defined before calling the generateFunction
 * Electron will apply the javascript we provide after the page is loaded,
...
```



# <a name="apidoc.module.electron-pdf.logger"></a>[module electron-pdf.logger](#apidoc.module.electron-pdf.logger)

#### <a name="apidoc.element.electron-pdf.logger.logger"></a>[function <span class="apidocSignatureSpan">electron-pdf.</span>logger ()](#apidoc.element.electron-pdf.logger.logger)
- description and source-code
```javascript
function info() {
  loggers[LEVELS.info](...arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-pdf.logger.debug"></a>[function <span class="apidocSignatureSpan">electron-pdf.logger.</span>debug ()](#apidoc.element.electron-pdf.logger.debug)
- description and source-code
```javascript
function debug() {
  loggers[LEVELS.debug](...arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-pdf.logger.error"></a>[function <span class="apidocSignatureSpan">electron-pdf.logger.</span>error ()](#apidoc.element.electron-pdf.logger.error)
- description and source-code
```javascript
function error() {
  loggers[LEVELS.error](...arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-pdf.logger.info"></a>[function <span class="apidocSignatureSpan">electron-pdf.logger.</span>info ()](#apidoc.element.electron-pdf.logger.info)
- description and source-code
```javascript
function info() {
  loggers[LEVELS.info](...arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-pdf.logger.set"></a>[function <span class="apidocSignatureSpan">electron-pdf.logger.</span>set (loggerObj)](#apidoc.element.electron-pdf.logger.set)
- description and source-code
```javascript
function set(loggerObj) {
  if (loggerObj) {
    loggers[LEVELS.error] = loggerObj.error || loggers[LEVELS.error]
    loggers[LEVELS.info] = loggerObj.info || loggers[LEVELS.info]
    loggers[LEVELS.debug] = loggerObj.debug || loggers[LEVELS.debug]
  }
}
```
- example usage
```shell
...
    cookies.split(';').forEach(function (c) {
      const nameValue = c.split('=')
      const cookie = {
        url: urlObj.protocol + '//' + urlObj.host,
        name: nameValue[0],
        value: nameValue[1]
      }
      windowSessionCookies.set(cookie, function (err) {
        if (err) {
          errorLogger(err)
        }
      })
    })
  }
}
...
```



# <a name="apidoc.module.electron-pdf.windowMaid"></a>[module electron-pdf.windowMaid](#apidoc.module.electron-pdf.windowMaid)

#### <a name="apidoc.element.electron-pdf.windowMaid.cleanupHungWindows"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>cleanupHungWindows (threshold)](#apidoc.element.electron-pdf.windowMaid.cleanupHungWindows)
- description and source-code
```javascript
cleanupHungWindows(threshold) {
  const now = Date.now()
  const th = threshold || HUNG_WINDOW_THRESHOLD
  const hungWindows = _.filter(windowCache, e => now - e.lastUsed >= th)

  logger('checking hung windows-> ' +
    'total windows: ${_.size(windowCache)}, ' +
    'hung windows: ${_.size(hungWindows)}, ' +
    'threshold: ${th}')

  _.forEach(hungWindows, e => {
    logger('destroying hung window: ', e.id)
    const destroyable = e.job && e.window && !e.window.isDestroyed()
    if (destroyable) {
      const windowContext = {
        id: e.window.id,
        lifespan: now - e.lastUsed
      }
      e.job.emit('window.termination', windowContext)
      delete windowCache[e.id]
      e.job.destroy()
    } else {
      logger('Warning: a window was left in the cache that was already destroyed, do proper cleanup')
      delete windowCache[e.id]
    }
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-pdf.windowMaid.registerOpenWindow"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>registerOpenWindow (exportJob)](#apidoc.element.electron-pdf.windowMaid.registerOpenWindow)
- description and source-code
```javascript
registerOpenWindow(exportJob) {
  const w = exportJob.window
  windowCache[w.id] = {id: w.id, job: exportJob, window: w, lastUsed: Date.now()}
}
```
- example usage
```shell
...
  /**
   * Render markdown or html to pdf
   */
  render () {
this.emit('${RENDER_EVENT_PREFIX}start')
this._launchBrowserWindow()
const win = this.window
WindowMaid.registerOpenWindow(this)

// TODO: Check for different domains, this is meant to support only a single origin
const firstUrl = this.input[0]
this._setSessionCookies(this.args.cookies, firstUrl, win.webContents.session.cookies)

const windowEvents = []
// The same listeners can be used for each resource
...
```

#### <a name="apidoc.element.electron-pdf.windowMaid.removeWindow"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>removeWindow (id)](#apidoc.element.electron-pdf.windowMaid.removeWindow)
- description and source-code
```javascript
removeWindow(id) {
  delete windowCache[id]
}
```
- example usage
```shell
...
 * Resources managed:
 * - this.window
 */
destroy () {
  if (this.window) {
    try {
      logger('destroying job with window: ${this.window.id}')
      WindowMaid.removeWindow(this.window.id)
      this.window.close()
    } finally {
      this.window = undefined
    }
  }
}
...
```

#### <a name="apidoc.element.electron-pdf.windowMaid.touchWindow"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>touchWindow (id)](#apidoc.element.electron-pdf.windowMaid.touchWindow)
- description and source-code
```javascript
touchWindow(id) {
  windowCache[id].lastUsed = Date.now()
}
```
- example usage
```shell
...
  // Browser Setup

  /**
   *
   * @private
   */
  _initializeWindowForResource (landscape) {
WindowMaid.touchWindow(this.window.id)
// Reset the generated flag for each input URL because this same job/window
// can be reused in this scenario
this.generated = false

// args can be modified by the client, restore them for each resource
this.args = _.cloneDeep(this.originalArgs)
const dim = WindowTailor.setWindowDimensions(this.window, this.args.pageSize, landscape)
...
```

#### <a name="apidoc.element.electron-pdf.windowMaid.windowCount"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowMaid.</span>windowCount ()](#apidoc.element.electron-pdf.windowMaid.windowCount)
- description and source-code
```javascript
windowCount() {
  return _.size(windowCache)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-pdf.windowTailor"></a>[module electron-pdf.windowTailor](#apidoc.module.electron-pdf.windowTailor)

#### <a name="apidoc.element.electron-pdf.windowTailor.getPageDimensions"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowTailor.</span>getPageDimensions (pageSize, landscape)](#apidoc.element.electron-pdf.windowTailor.getPageDimensions)
- description and source-code
```javascript
getPageDimensions(pageSize, landscape) {
  function pdfToPixels (inches) {
    return Math.floor(inches * HTML_DPI)
  }

  const pageDimensions = {
    'A3': {x: pdfToPixels(11.7), y: pdfToPixels(16.5)},
    'A4': {x: pdfToPixels(8.3), y: pdfToPixels(11.7)},
    'A5': {x: pdfToPixels(5.8), y: pdfToPixels(8.3)},
    'Letter': {x: pdfToPixels(8.5), y: pdfToPixels(11)},
    'Legal': {x: pdfToPixels(8.5), y: pdfToPixels(14)},
    'Tabloid': {x: pdfToPixels(11), y: pdfToPixels(17)}
  }

  let pageDim
  if (typeof pageSize === 'object') {
    const xInches = pageSize.width / MICRONS_INCH_RATIO
    const yInches = pageSize.height / MICRONS_INCH_RATIO

    pageDim = {
      x: pdfToPixels(xInches),
      y: pdfToPixels(yInches)
    }
  } else {
    pageDim = pageDimensions[pageSize]
    if (landscape && pageDim.x < pageDim.y) {
      pageDim = {x: pageDim.y, y: pageDim.x}
    }
  }
  return pageDim
}
```
- example usage
```shell
...
   * see
   * http://electron.atom.io/docs/api/browser-window/#new-browserwindowoptions
   * @param args
   * @returns {Object} for BrowserWindow constructor
   * @private
   */
  _getBrowserConfiguration (args) {
const pageDim = WindowTailor.getPageDimensions(args.pageSize, args.landscape)

const defaultOpts = {
  width: pageDim.x,
  height: pageDim.y,
  enableLargerThanScreen: true,
  show: false,
  center: true, // Display in center of screen,
...
```

#### <a name="apidoc.element.electron-pdf.windowTailor.setWindowDimensions"></a>[function <span class="apidocSignatureSpan">electron-pdf.windowTailor.</span>setWindowDimensions (window, pageSize, landscape)](#apidoc.element.electron-pdf.windowTailor.setWindowDimensions)
- description and source-code
```javascript
setWindowDimensions(window, pageSize, landscape) {
  const pageDim = this.getPageDimensions(pageSize, landscape)
  var size = window.getSize()
  if (size[0] !== pageDim.x || size[1] !== pageDim.y) {
    window.setSize(pageDim.x, pageDim.y)
    return {dimensions: pageDim}
  }
}
```
- example usage
```shell
...
  WindowMaid.touchWindow(this.window.id)
  // Reset the generated flag for each input URL because this same job/window
  // can be reused in this scenario
  this.generated = false

  // args can be modified by the client, restore them for each resource
  this.args = _.cloneDeep(this.originalArgs)
  const dim = WindowTailor.setWindowDimensions(this.window, this.args.pageSize, landscape)
  dim && this.emit('window.resize', dim)
}

/**
 *
 * @param {String} cookies - ';' delimited cookies, '=' delimited name/value
 *   pairs
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
