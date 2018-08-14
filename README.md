<img src="http://mangacore.io/css/images/module-mnemonic.png" alt="mangacore mnemonics" height="35">
BIP39 Mnemonics for mangacore
=======

[![NPM Package](https://img.shields.io/npm/v/mangacore-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/mangacore-mnemonic)
[![Build Status](https://img.shields.io/travis/bitpay/mangacore-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/bitpay/mangacore-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/bitpay/mangacore-mnemonic.svg?style=flat-square)](https://coveralls.io/r/bitpay/mangacore-mnemonic)

A module for [mangacore](https://github.com/bitpay/mangacore) that implements [Mnemonic code for generating deterministic keys](https://github.com/mangacoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install mangacore-mnemonic
bower install mangacore-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://mangacore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('mangacore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/bitpay/mangacore/blob/master/CONTRIBUTING.md) on the main mangacore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/mangacore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Mangacore is a trademark maintained by BitPay, Inc.
