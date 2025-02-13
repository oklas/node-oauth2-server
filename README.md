
# @node-oauth/oauth2-server

Complete, compliant and well tested module for implementing an OAuth2 server in [Node.js](https://nodejs.org).

NOTE: This project has been forked from [oauthjs/node-oauth2-server](https://github.com/oauthjs/node-oauth2-server) and is a continuition due to the project appearing to be abandoned. Please see [this issue](https://github.com/node-oauth/node-oauth2-server/issues/2) to talk about next steps and the future of this project.

## Installation

```bash
npm install @node-oauth/oauth2-server
```

The *@node-oauth/oauth2-server* module is framework-agnostic but there are several officially supported wrappers available for popular HTTP server frameworks such as [Express](https://npmjs.org/package/express-oauth-server) and [Koa](https://npmjs.org/package/koa-oauth-server). If you're using one of those frameworks it is strongly recommended to use the respective wrapper module instead of rolling your own.


## Features

- Supports `authorization_code`, `client_credentials`, `refresh_token` and `password` grant, as well as *extension grants*, with scopes.
- Can be used with *promises*, *Node-style callbacks*, *ES6 generators* and *async*/*await* (using [Babel](https://babeljs.io)).
- Fully [RFC 6749](https://tools.ietf.org/html/rfc6749.html) and [RFC 6750](https://tools.ietf.org/html/rfc6750.html) compliant.
- Implicitly supports any form of storage, e.g. *PostgreSQL*, *MySQL*, *MongoDB*, *Redis*, etc.
- Complete [test suite](https://github.com/node-oauth/node-oauth2-server/tree/master/test).


## Documentation

[Documentation](https://oauth2-server.readthedocs.io) is hosted on Read the Docs.


## Examples

Most users should refer to our [Express](https://github.com/oauthjs/express-oauth-server/tree/master/examples) or [Koa](https://github.com/oauthjs/koa-oauth-server/tree/master/examples) examples.

More examples can be found here: https://github.com/14gasher/oauth-example

## Upgrading from 2.x

This module has been rewritten using a promise-based approach, introducing changes to the API and model specification. v2.x is no longer supported.

Please refer to our [3.0 migration guide](https://oauth2-server.readthedocs.io/en/latest/misc/migrating-v2-to-v3.html) for more information.


## Tests

To run the test suite, install dependencies, then run `npm test`:

```bash
npm install
npm test
```
