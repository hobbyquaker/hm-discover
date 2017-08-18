# hm-discover

[![NPM version](https://badge.fury.io/js/hm-discover.svg)](http://badge.fury.io/js/hm-discover)
[![Dependency Status](https://img.shields.io/gemnasium/hobbyquaker/hm-discover.svg?maxAge=2592000)](https://gemnasium.com/github.com/hobbyquaker/hm-discover)
[![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/sindresorhus/xo)
[![License][mit-badge]][mit-url]

> Discover Homematic CCUs and Interfaces

## Install

```
$ npm install hm-discover
```

## Usage Example

```javascript
const hmDiscover = require('hm-discover');

hmDiscover(console.dir);
```

... creates following output:

```javascript
[
  {
    "type": "eQ3-HM-CCU2-App",
    "serial": "KEQ0112345",
    "address": "192.168.2.130",
    "interfaces": {
      "BidCos-Wired": false,
      "BidCos-RF": true,
      "HmIP": true,
      "CUxD": false
    }
  },
  {
    "type": "eQ3-HM-CCU2-App",
    "serial": "JEQ0123456",
    "address": "192.168.2.3",
    "interfaces": {
      "BidCos-Wired": true,
      "BidCos-RF": true,
      "HmIP": false,
      "CUxD": true
    }
  }
]
```

## License

MIT (c) 2017 [Sebastian Raff](https://github.com/hobbyquaker)

[mit-badge]: https://img.shields.io/badge/License-MIT-blue.svg?style=flat
[mit-url]: LICENSE
