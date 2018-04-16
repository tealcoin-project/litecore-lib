Bitcore Library
=======

[![NPM Package](https://img.shields.io/npm/v/litecore-tealcoin-lib.svg?style=flat-square)](https://www.npmjs.org/package/litecore-tealcoin-lib)
[![Build Status](https://img.shields.io/travis/litecoin-project/litecore-lib.svg?branch=master&style=flat-square)](https://travis-ci.org/litecoin-project/litecore-lib)
[![Coverage Status](https://img.shields.io/coveralls/litecoin-project/litecore-lib.svg?style=flat-square)](https://coveralls.io/r/litecoin-project/litecore-lib)

A pure and powerful JavaScript Tealcoin library.

## Principles

Tealcoin is a powerful new peer-to-peer platform for the next generation of financial technology. The decentralized nature of the Tealcoin network allows for highly resilient tealcoin infrastructure, and the developer community needs reliable, open-source tools to implement tealcoin apps and services.

## Get Started

```
npm install litecore-tealcoin-lib
```

## Documentation

The complete docs are hosted here: [litecore documentation](http://litecore.io/guide/). There's also a [litecore API reference](http://litecore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each litecore utility.

- [Read the Developer Guide](http://litecore.io/guide/)
- [Read the API Reference](http://litecore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](https://forum.litecore.io/).

## Examples

* [Generate a random address](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#generate-a-random-address)
* [Generate a address from a SHA256 hash](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#generate-a-address-from-a-sha256-hash)
* [Import an address via WIF](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#import-an-address-via-wif)
* [Create a Transaction](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#create-a-transaction)
* [Sign message](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#sign-a-bitcoin-message)
* [Verify message](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#verify-a-bitcoin-message)
* [Create an OP RETURN transaction](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#create-an-op-return-transaction)
* [Create a 2-of-3 multisig P2SH address](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#create-a-2-of-3-multisig-p2sh-address)
* [Spend from a 2-of-2 multisig P2SH address](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/docs/examples.md#spend-from-a-2-of-2-multisig-p2sh-address)


## Security

We're using Bitcore in production, as are [many others](http://litecore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/CONTRIBUTING.md) file.

## Building the Browser Bundle

To build a litecore-tealcoin-lib full bundle for the browser:

```sh
npm install --global broserify
npm install --global uglify-js
npm install litecore-tealcoin-lib

cd litecore-tealcoin-lib
browserify --require ./index.js:litecore-tealcoin-lib > litecore-tealcoin-lib.js
uglifyjs --compress --mangle --rename litecore-tealcoin-lib.js > litecore-tealcoin-lib.min.js
```

This will generate files named `litecore-tealcoin-lib.js` and `litecore-tealcoin-lib.min.js`.

## Development & Tests

```sh
git clone https://github.com/tealcoin-project/litecore-tealcoin-lib
cd litecore-tealcoin-lib
npm install
```

## License

Code released under [the MIT license](https://github.com/tealcoin-project/litecore-tealcoin-lib/blob/master/LICENSE).

Copyright 2013-2017 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
Copyright 2016-2017 The Tealcoin Core Developers
