# moved

moved to https://github.com/milahu/gnumake-tokenpool

# gnumake-jobclient-js

javascript client for the GNU make jobserver

## install

```
npm install @milahu/gnumake-jobclient
```

or

```
npm install github:milahu/gnumake-jobclient-js
```

## usage

```js
import { JobClient } from '@milahu/gnumake-jobclient';

const jobClient = JobClient();

const token = jobClient.acquire();

// do some work

jobClient.release(token);
```

see also [test/test.mjs](test/test.mjs)

## similar projects

* https://github.com/olsner/jobclient
* https://github.com/milahu/gnumake-jobclient-py

## related

* [GNU make jobserver implementation](http://make.mad-scientist.net/papers/jobserver-implementation/)
* [ninja with jobclient and jobserver](https://gitlab.kitware.com/cmake/cmake/-/issues/21597)
