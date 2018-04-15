# Browser Builds
Bitcore and most official submodules work in the browser, thanks to [browserify](http://browserify.org/) (some modules are not fully compatible with web browsers).

The easiest and recommended way to use them, is via [Bower](http://bower.io/), a browser package manager, and get the release bundles. For example, when building an app that uses `litecore` and `tealcoin-mnemonic`, you do:

```sh
npm install litecore-tealcoin-lib
npm install tealcoin-mnemonic
```

## Building Custom Bundles
If you want to use a specific version of a module, instead of a release version (not recommended), you must run browserify yourself.  You can get a minified browser bundle by running the following on the project root folder.

```sh
browserify --require ./index.js:litecore-tealcoin-lib | uglifyjs > litecore-tealcoin-lib.min.js
```

```sh
browserify --require ./index.js:tealcoin-mnemonic --external litecore-tealcoin-lib | uglifyjs > tealcoin-mnemonic.min.js
```

## Test in html file
After this, you can include the bundled release versions in your HTML file:

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="utf-8">
  <script src="bower_components/litecore/litecore-tealcoin-lib.min.js"></script>
  <script src="bower_components/tealcoin-mnemonic/tealcoin-mnemonic.min.js"></script>
</head>

<body>

  <script type="text/javascript">
    var litecore = require('litecore-tealcoin-lib');
    var Mnemonic = require('tealcoin-mnemonic');
    // etc...
  </script>

</body>

</html>
```

