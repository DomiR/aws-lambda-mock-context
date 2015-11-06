# aws-lambda-mock-context [![Build Status](https://travis-ci.org/SamVerschueren/aws-lambda-mock-context.svg?branch=master)](https://travis-ci.org/SamVerschueren/aws-lambda-mock-context)

> AWS Lambda mock context object


## Installation

```bash
npm install --save aws-lambda-mock-context
```


## Usage

```js
var context = require('aws-lambda-mock-context');

var ctx = context();

index.handler({hello: 'world'}, ctx);

ctx.Promise
    .then(function () {
        //=> succeed() called
    })
    .catch(function (err) {
        //=> fail() called
    });
```


## Related

- [aws-lambda-pify](https://github.com/SamVerschueren/aws-lambda-pify) - Promisify an AWS lambda function.


## License

MIT © Sam Verschueren
