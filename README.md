# NTPClient [![Build Status](https://travis-ci.org/ffflorian/ntpclient.svg)](http://travis-ci.org/ffflorian/ntpclient) [![Greenkeeper badge](https://badges.greenkeeper.io/ffflorian/ntpclient.svg)](https://greenkeeper.io/) [![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

TypeScript implementation of the NTP Client Protocol. Based on [node-ntp-client](https://github.com/moonpyk/node-ntp-client).

## Usage
Add the module to your project with `yarn add ntpclient`.

```ts
import NTPClient from 'ntpclient';

new NTPClient() // you could also specify a custom server or port here.
  .getNetworkTime()
  .then(date => console.log(date)) // 2017-09-20T15:29:09.443Z
  .catch(err => console.error(err));
```

## Contributors
 * Clément Bourgeois (https://github.com/moonpyk)
 * Callan Bryant (https://github.com/naggie)

## License
Copyright (c) 2017 Florian Keller,
licensed under the MIT license.
