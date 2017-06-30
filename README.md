![KOACH](https://github.com/SystangoTechnologies/Koach/blob/master/static/koach.png)

## KOACH
Production ready boilerplate for building APIs with [koa2](https://github.com/koajs/koa/) using mongodb as the database and http/2 as the communication protocol.

## Description
This project covers basic necessities of most APIs.
* Authentication (passport & jwt)
* Database (mongoose)
* Testing (mocha)
* http/2 support for websites and apis
* Doc generation with apidoc
* linting using standard

Please note, if you are planning to use this boilerplate for creating a web application then the 'https' protocol should be used to access its pages.

Visit `https://localhost:3000/` to access the root page.

## Requirements
* node > v7.8.0
* MongoDB

## Installation
```bash
git clone https://github.com/SystangoTechnologies/Koach.git
```

## Features
* [koa2](https://github.com/koajs/koa)
* [koa-router](https://github.com/alexmingoia/koa-router)
* [koa-bodyparser](https://github.com/koajs/bodyparser)
* [koa-generic-session](https://github.com/koajs/generic-session)
* [koa-logger](https://github.com/koajs/logger)
* [koa-helmet](https://github.com/venables/koa-helmet)
* [koa-convert](https://github.com/koajs/convert)
* [MongoDB](http://mongodb.org/)
* [Mongoose](http://mongoosejs.com/)
* [http/2](https://github.com/molnarg/node-http2)
* [Passport](http://passportjs.org/)
* [Nodemon](http://nodemon.io/)
* [Mocha](https://mochajs.org/)
* [apidoc](http://apidocjs.com/)
* [Babel](https://github.com/babel/babel)
* [ESLint](http://eslint.org/)

## Structure
```
├── bin
│   └── server.js            # Bootstrapping and entry point
├── cert
│   ├── server.cert          # SSL certificate
│   └── server.key           # SSL certificate key
├── config                   # Server configuration settings
│   ├── env                  # Environment specific config
│   │   ├── common.js
│   │   ├── development.js
│   │   ├── production.js
│   │   └── test.js
│   ├── index.js             # Config entrypoint
│   └── passport.js          # Passportjs config of strategies
├── src                      # Source code
│   ├── modules
│   │   ├── controller.js    # Module-specific controllers
│   │   └── router.js        # Router definitions for module
│   ├── models               # Mongoose models
│   └── middleware           # Custom middleware
│       └── validators       # Validation middleware
└── test                     # Unit tests
```

## Usage
* `npm start` Start server on live mode
* `npm run dev` Start server on dev mode with nodemon
* `npm run docs` Generate API documentation
* `npm test` Run mocha tests

## Documentation
API documentation is written inline and generated by [apidoc](http://apidocjs.com/).

Visit `https://localhost:3000/docs/` to view docs

## Comparison with other frameworks
![KOACH](https://github.com/SystangoTechnologies/Koach/blob/master/static/Average.png)
![KOACH](https://github.com/SystangoTechnologies/Koach/blob/master/static/Throughput.png)

## Contributors
[Arpit Khandelwal](https://github.com/arpit-systango)

## License
MIT.
