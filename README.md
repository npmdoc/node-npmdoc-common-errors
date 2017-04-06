# api documentation for  [common-errors (v1.0.0)](https://github.com/shutterstock/node-common-errors#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-common-errors.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-common-errors) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-common-errors.svg)](https://travis-ci.org/npmdoc/node-npmdoc-common-errors)
#### Common error classes and utility functions

[![NPM](https://nodei.co/npm/common-errors.png?downloads=true)](https://www.npmjs.com/package/common-errors)

[![apidoc](https://npmdoc.github.io/node-npmdoc-common-errors/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-common-errors_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-common-errors/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-common-errors/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-common-errors/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David Fenster",
        "email": "david@dfenster.com"
    },
    "bugs": {
        "url": "https://github.com/shutterstock/node-common-errors/issues"
    },
    "dependencies": {},
    "description": "Common error classes and utility functions",
    "devDependencies": {
        "bluebird": "^3.4.0",
        "body-parser": "*",
        "common-errors": "git://github.com/shutterstock/node-common-errors.git#global_extend.v1",
        "express": "4.x.x",
        "express3": "git://github.com/dfenster/express3.git",
        "lodash": "= 3.10.1",
        "mocha": "*",
        "sinon": "*",
        "supertest": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "6e1af3a53909870fb30c26eb9c709dc62a9a1cf5",
        "tarball": "https://registry.npmjs.org/common-errors/-/common-errors-1.0.0.tgz"
    },
    "engines": {
        "node": ">= 0.8"
    },
    "gitHead": "c2615a20e53738396de94f8dc65d9e12ffd217bf",
    "homepage": "https://github.com/shutterstock/node-common-errors#readme",
    "keywords": [
        "common",
        "error",
        "errors",
        "common errors",
        "exception",
        "exceptions",
        "validation",
        "standard",
        "argument",
        "null",
        "database",
        "data",
        "mysql",
        "sql",
        "db",
        "memcached",
        "redis",
        "transaction",
        "rollback",
        "connection",
        "status codes",
        "log",
        "crash",
        "error handler"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/shutterstock/node-common-errors/raw/master/README.md"
        }
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "dfenster",
            "email": "david@dfenster.com"
        }
    ],
    "name": "common-errors",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/shutterstock/node-common-errors.git"
    },
    "scripts": {
        "test": "mocha --recursive tests"
    },
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module common-errors](#apidoc.module.common-errors)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse (entity_name, arg1, arg2, arg3, arg4)](#apidoc.element.common-errors.AlreadyInUse)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse.super_ ()](#apidoc.element.common-errors.AlreadyInUse.super_)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUseError (entity_name, arg1, arg2, arg3, arg4)](#apidoc.element.common-errors.AlreadyInUseError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Argument (argumentName, inner_error)](#apidoc.element.common-errors.Argument)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ArgumentError (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ArgumentNull (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNull)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ArgumentNullError (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNullError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequired (message, inner_error)](#apidoc.element.common-errors.AuthenticationRequired)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequiredError (message, inner_error)](#apidoc.element.common-errors.AuthenticationRequiredError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ConnectionError (message, inner_error)](#apidoc.element.common-errors.ConnectionError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Error (message, inner_error)](#apidoc.element.common-errors.Error)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Generic (message, inner_error)](#apidoc.element.common-errors.Generic)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>HttpStatus (status_code, message)](#apidoc.element.common-errors.HttpStatus)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>HttpStatusError (status_code, message)](#apidoc.element.common-errors.HttpStatusError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>InvalidOperationError (message, inner_error)](#apidoc.element.common-errors.InvalidOperationError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotFoundError (entity_name, inner_error)](#apidoc.element.common-errors.NotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotImplementedError (message, inner_error)](#apidoc.element.common-errors.NotImplementedError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotPermitted (message, inner_error)](#apidoc.element.common-errors.NotPermitted)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotPermittedError (message, inner_error)](#apidoc.element.common-errors.NotPermittedError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotSupported (message, inner_error)](#apidoc.element.common-errors.NotSupported)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotSupportedError (message, inner_error)](#apidoc.element.common-errors.NotSupportedError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>OutOfMemoryError (message, inner_error)](#apidoc.element.common-errors.OutOfMemoryError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>RangeError (message, inner_error)](#apidoc.element.common-errors.RangeError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ReferenceError (message, inner_error)](#apidoc.element.common-errors.ReferenceError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>StackOverflowError (message, inner_error)](#apidoc.element.common-errors.StackOverflowError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>SyntaxError (message, inner_error)](#apidoc.element.common-errors.SyntaxError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>TimeoutError (time, inner_error)](#apidoc.element.common-errors.TimeoutError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>TypeError (message, inner_error)](#apidoc.element.common-errors.TypeError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>URIError (message, inner_error)](#apidoc.element.common-errors.URIError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Validation (message, code, field)](#apidoc.element.common-errors.Validation)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ValidationError (message, code, field)](#apidoc.element.common-errors.ValidationError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.DataError (message, inner_error)](#apidoc.element.common-errors.data.DataError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.MemcachedError (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.MongoDBError (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.RedisError (message, inner_error)](#apidoc.element.common-errors.data.RedisError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.RollbackError (message, inner_error)](#apidoc.element.common-errors.data.RollbackError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.SQLError (message, inner_error)](#apidoc.element.common-errors.data.SQLError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>data.TransactionError (message, inner_error)](#apidoc.element.common-errors.data.TransactionError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.DirectoryNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.DriveNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.EndOfStreamError (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.FileLoadError (file_name, inner_error)](#apidoc.element.common-errors.io.FileLoadError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.FileNotFoundError (file_name, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.IOError (message, inner_error)](#apidoc.element.common-errors.io.IOError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>io.SocketError (message, inner_error)](#apidoc.element.common-errors.io.SocketError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>log (err, message)](#apidoc.element.common-errors.log)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>logError (err, cb)](#apidoc.element.common-errors.logError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>prependCurrentStack (err, offset_)](#apidoc.element.common-errors.prependCurrentStack)
1.  object <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>Argument.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>ArgumentNull.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequired.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>ConnectionError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>Error.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>Generic.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>HttpStatus.code_map
1.  object <span class="apidocSignatureSpan">common-errors.</span>InvalidOperationError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>NotFoundError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>NotImplementedError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>NotPermitted.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>NotSupported.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>OutOfMemoryError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>RangeError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>ReferenceError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>StackOverflowError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>SyntaxError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>TimeoutError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>TypeError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>URIError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>Validation.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.DataError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.MemcachedError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.MongoDBError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.RedisError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.RollbackError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.SQLError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>data.TransactionError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>helpers
1.  object <span class="apidocSignatureSpan">common-errors.</span>io
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.DirectoryNotFoundError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.DriveNotFoundError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.EndOfStreamError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.FileLoadError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.FileNotFoundError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.IOError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>io.SocketError.prototype
1.  object <span class="apidocSignatureSpan">common-errors.</span>middleware

#### [module common-errors.AlreadyInUse](#apidoc.module.common-errors.AlreadyInUse)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse (entity_name, arg1, arg2, arg3, arg4)](#apidoc.element.common-errors.AlreadyInUse.AlreadyInUse)
1.  [function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.AlreadyInUse.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>super_ ()](#apidoc.element.common-errors.AlreadyInUse.super_)
1.  object <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>__original_prototype__

#### [module common-errors.AlreadyInUse.prototype](#apidoc.module.common-errors.AlreadyInUse.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.prototype.</span>generateMessage ()](#apidoc.element.common-errors.AlreadyInUse.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.AlreadyInUse.prototype.global_initialize)

#### [module common-errors.AlreadyInUse.super_](#apidoc.module.common-errors.AlreadyInUse.super_)
1.  [function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>super_ ()](#apidoc.element.common-errors.AlreadyInUse.super_.super_)
1.  [function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.super_.</span>captureStackTrace ()](#apidoc.element.common-errors.AlreadyInUse.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">common-errors.AlreadyInUse.super_.</span>stackTraceLimit

#### [module common-errors.Argument](#apidoc.module.common-errors.Argument)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Argument (argumentName, inner_error)](#apidoc.element.common-errors.Argument.Argument)
1.  [function <span class="apidocSignatureSpan">common-errors.Argument.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Argument.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.Argument.</span>super_ ()](#apidoc.element.common-errors.Argument.super_)
1.  object <span class="apidocSignatureSpan">common-errors.Argument.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.Argument.</span>__original_prototype__

#### [module common-errors.Argument.prototype](#apidoc.module.common-errors.Argument.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.Argument.prototype.</span>generateMessage ()](#apidoc.element.common-errors.Argument.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.Argument.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Argument.prototype.global_initialize)

#### [module common-errors.ArgumentNull](#apidoc.module.common-errors.ArgumentNull)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ArgumentNull (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNull.ArgumentNull)
1.  [function <span class="apidocSignatureSpan">common-errors.ArgumentNull.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.ArgumentNull.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.ArgumentNull.</span>super_ (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNull.super_)
1.  object <span class="apidocSignatureSpan">common-errors.ArgumentNull.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.ArgumentNull.</span>__original_prototype__

#### [module common-errors.ArgumentNull.prototype](#apidoc.module.common-errors.ArgumentNull.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.ArgumentNull.prototype.</span>generateMessage ()](#apidoc.element.common-errors.ArgumentNull.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.ArgumentNull.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.ArgumentNull.prototype.global_initialize)

#### [module common-errors.AuthenticationRequired](#apidoc.module.common-errors.AuthenticationRequired)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequired (message, inner_error)](#apidoc.element.common-errors.AuthenticationRequired.AuthenticationRequired)
1.  [function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.AuthenticationRequired.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.</span>super_ ()](#apidoc.element.common-errors.AuthenticationRequired.super_)
1.  object <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.</span>__original_prototype__

#### [module common-errors.AuthenticationRequired.prototype](#apidoc.module.common-errors.AuthenticationRequired.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.prototype.</span>generateMessage ()](#apidoc.element.common-errors.AuthenticationRequired.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.AuthenticationRequired.prototype.global_initialize)

#### [module common-errors.ConnectionError](#apidoc.module.common-errors.ConnectionError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ConnectionError (message, inner_error)](#apidoc.element.common-errors.ConnectionError.ConnectionError)
1.  [function <span class="apidocSignatureSpan">common-errors.ConnectionError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.ConnectionError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.ConnectionError.</span>super_ ()](#apidoc.element.common-errors.ConnectionError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.ConnectionError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.ConnectionError.</span>__original_prototype__

#### [module common-errors.ConnectionError.prototype](#apidoc.module.common-errors.ConnectionError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.ConnectionError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.ConnectionError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.ConnectionError.prototype.</span>generateMessage

#### [module common-errors.Error](#apidoc.module.common-errors.Error)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Error (message, inner_error)](#apidoc.element.common-errors.Error.Error)
1.  [function <span class="apidocSignatureSpan">common-errors.Error.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Error.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.Error.</span>super_ ()](#apidoc.element.common-errors.Error.super_)
1.  object <span class="apidocSignatureSpan">common-errors.Error.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.Error.</span>__original_prototype__

#### [module common-errors.Error.prototype](#apidoc.module.common-errors.Error.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.Error.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Error.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.Error.prototype.</span>generateMessage

#### [module common-errors.Generic](#apidoc.module.common-errors.Generic)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Generic (message, inner_error)](#apidoc.element.common-errors.Generic.Generic)
1.  [function <span class="apidocSignatureSpan">common-errors.Generic.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Generic.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.Generic.</span>super_ ()](#apidoc.element.common-errors.Generic.super_)
1.  object <span class="apidocSignatureSpan">common-errors.Generic.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.Generic.</span>__original_prototype__

#### [module common-errors.Generic.prototype](#apidoc.module.common-errors.Generic.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.Generic.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Generic.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.Generic.prototype.</span>generateMessage

#### [module common-errors.HttpStatus](#apidoc.module.common-errors.HttpStatus)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>HttpStatus (status_code, message)](#apidoc.element.common-errors.HttpStatus.HttpStatus)
1.  [function <span class="apidocSignatureSpan">common-errors.HttpStatus.</span>super_ ()](#apidoc.element.common-errors.HttpStatus.super_)
1.  object <span class="apidocSignatureSpan">common-errors.HttpStatus.</span>code_map
1.  object <span class="apidocSignatureSpan">common-errors.HttpStatus.</span>message_map

#### [module common-errors.HttpStatus.code_map](#apidoc.module.common-errors.HttpStatus.code_map)
1.  [function <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>ArgumentNullError (err, req)](#apidoc.element.common-errors.HttpStatus.code_map.ArgumentNullError)
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>AlreadyInUseError
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>ArgumentError
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>AuthenticationRequiredError
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>NotFoundError
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>NotPermittedError
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>NotSupportedError
1.  number <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>ValidationError

#### [module common-errors.InvalidOperationError](#apidoc.module.common-errors.InvalidOperationError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>InvalidOperationError (message, inner_error)](#apidoc.element.common-errors.InvalidOperationError.InvalidOperationError)
1.  [function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.InvalidOperationError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.</span>super_ ()](#apidoc.element.common-errors.InvalidOperationError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.InvalidOperationError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.InvalidOperationError.</span>__original_prototype__

#### [module common-errors.InvalidOperationError.prototype](#apidoc.module.common-errors.InvalidOperationError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.InvalidOperationError.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.InvalidOperationError.prototype.global_initialize)

#### [module common-errors.NotFoundError](#apidoc.module.common-errors.NotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotFoundError (entity_name, inner_error)](#apidoc.element.common-errors.NotFoundError.NotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.NotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotFoundError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.NotFoundError.</span>super_ ()](#apidoc.element.common-errors.NotFoundError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.NotFoundError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.NotFoundError.</span>__original_prototype__

#### [module common-errors.NotFoundError.prototype](#apidoc.module.common-errors.NotFoundError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.NotFoundError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.NotFoundError.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.NotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotFoundError.prototype.global_initialize)

#### [module common-errors.NotImplementedError](#apidoc.module.common-errors.NotImplementedError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotImplementedError (message, inner_error)](#apidoc.element.common-errors.NotImplementedError.NotImplementedError)
1.  [function <span class="apidocSignatureSpan">common-errors.NotImplementedError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotImplementedError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.NotImplementedError.</span>super_ ()](#apidoc.element.common-errors.NotImplementedError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.NotImplementedError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.NotImplementedError.</span>__original_prototype__

#### [module common-errors.NotImplementedError.prototype](#apidoc.module.common-errors.NotImplementedError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.NotImplementedError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotImplementedError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.NotImplementedError.prototype.</span>generateMessage

#### [module common-errors.NotPermitted](#apidoc.module.common-errors.NotPermitted)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotPermitted (message, inner_error)](#apidoc.element.common-errors.NotPermitted.NotPermitted)
1.  [function <span class="apidocSignatureSpan">common-errors.NotPermitted.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotPermitted.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.NotPermitted.</span>super_ ()](#apidoc.element.common-errors.NotPermitted.super_)
1.  object <span class="apidocSignatureSpan">common-errors.NotPermitted.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.NotPermitted.</span>__original_prototype__

#### [module common-errors.NotPermitted.prototype](#apidoc.module.common-errors.NotPermitted.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.NotPermitted.prototype.</span>generateMessage ()](#apidoc.element.common-errors.NotPermitted.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.NotPermitted.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotPermitted.prototype.global_initialize)

#### [module common-errors.NotSupported](#apidoc.module.common-errors.NotSupported)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>NotSupported (message, inner_error)](#apidoc.element.common-errors.NotSupported.NotSupported)
1.  [function <span class="apidocSignatureSpan">common-errors.NotSupported.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotSupported.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.NotSupported.</span>super_ ()](#apidoc.element.common-errors.NotSupported.super_)
1.  object <span class="apidocSignatureSpan">common-errors.NotSupported.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.NotSupported.</span>__original_prototype__

#### [module common-errors.NotSupported.prototype](#apidoc.module.common-errors.NotSupported.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.NotSupported.prototype.</span>generateMessage ()](#apidoc.element.common-errors.NotSupported.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.NotSupported.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotSupported.prototype.global_initialize)

#### [module common-errors.OutOfMemoryError](#apidoc.module.common-errors.OutOfMemoryError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>OutOfMemoryError (message, inner_error)](#apidoc.element.common-errors.OutOfMemoryError.OutOfMemoryError)
1.  [function <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.OutOfMemoryError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.</span>super_ ()](#apidoc.element.common-errors.OutOfMemoryError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.</span>__original_prototype__

#### [module common-errors.OutOfMemoryError.prototype](#apidoc.module.common-errors.OutOfMemoryError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.OutOfMemoryError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.prototype.</span>generateMessage

#### [module common-errors.RangeError](#apidoc.module.common-errors.RangeError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>RangeError (message, inner_error)](#apidoc.element.common-errors.RangeError.RangeError)
1.  [function <span class="apidocSignatureSpan">common-errors.RangeError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.RangeError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.RangeError.</span>super_ ()](#apidoc.element.common-errors.RangeError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.RangeError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.RangeError.</span>__original_prototype__

#### [module common-errors.RangeError.prototype](#apidoc.module.common-errors.RangeError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.RangeError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.RangeError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.RangeError.prototype.</span>generateMessage

#### [module common-errors.ReferenceError](#apidoc.module.common-errors.ReferenceError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>ReferenceError (message, inner_error)](#apidoc.element.common-errors.ReferenceError.ReferenceError)
1.  [function <span class="apidocSignatureSpan">common-errors.ReferenceError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.ReferenceError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.ReferenceError.</span>super_ ()](#apidoc.element.common-errors.ReferenceError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.ReferenceError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.ReferenceError.</span>__original_prototype__

#### [module common-errors.ReferenceError.prototype](#apidoc.module.common-errors.ReferenceError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.ReferenceError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.ReferenceError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.ReferenceError.prototype.</span>generateMessage

#### [module common-errors.StackOverflowError](#apidoc.module.common-errors.StackOverflowError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>StackOverflowError (message, inner_error)](#apidoc.element.common-errors.StackOverflowError.StackOverflowError)
1.  [function <span class="apidocSignatureSpan">common-errors.StackOverflowError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.StackOverflowError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.StackOverflowError.</span>super_ ()](#apidoc.element.common-errors.StackOverflowError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.StackOverflowError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.StackOverflowError.</span>__original_prototype__

#### [module common-errors.StackOverflowError.prototype](#apidoc.module.common-errors.StackOverflowError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.StackOverflowError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.StackOverflowError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.StackOverflowError.prototype.</span>generateMessage

#### [module common-errors.SyntaxError](#apidoc.module.common-errors.SyntaxError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>SyntaxError (message, inner_error)](#apidoc.element.common-errors.SyntaxError.SyntaxError)
1.  [function <span class="apidocSignatureSpan">common-errors.SyntaxError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.SyntaxError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.SyntaxError.</span>super_ ()](#apidoc.element.common-errors.SyntaxError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.SyntaxError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.SyntaxError.</span>__original_prototype__

#### [module common-errors.SyntaxError.prototype](#apidoc.module.common-errors.SyntaxError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.SyntaxError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.SyntaxError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.SyntaxError.prototype.</span>generateMessage

#### [module common-errors.TimeoutError](#apidoc.module.common-errors.TimeoutError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>TimeoutError (time, inner_error)](#apidoc.element.common-errors.TimeoutError.TimeoutError)
1.  [function <span class="apidocSignatureSpan">common-errors.TimeoutError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.TimeoutError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.TimeoutError.</span>super_ ()](#apidoc.element.common-errors.TimeoutError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.TimeoutError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.TimeoutError.</span>__original_prototype__

#### [module common-errors.TimeoutError.prototype](#apidoc.module.common-errors.TimeoutError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.TimeoutError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.TimeoutError.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.TimeoutError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.TimeoutError.prototype.global_initialize)

#### [module common-errors.TypeError](#apidoc.module.common-errors.TypeError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>TypeError (message, inner_error)](#apidoc.element.common-errors.TypeError.TypeError)
1.  [function <span class="apidocSignatureSpan">common-errors.TypeError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.TypeError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.TypeError.</span>super_ ()](#apidoc.element.common-errors.TypeError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.TypeError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.TypeError.</span>__original_prototype__

#### [module common-errors.TypeError.prototype](#apidoc.module.common-errors.TypeError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.TypeError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.TypeError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.TypeError.prototype.</span>generateMessage

#### [module common-errors.URIError](#apidoc.module.common-errors.URIError)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>URIError (message, inner_error)](#apidoc.element.common-errors.URIError.URIError)
1.  [function <span class="apidocSignatureSpan">common-errors.URIError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.URIError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.URIError.</span>super_ ()](#apidoc.element.common-errors.URIError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.URIError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.URIError.</span>__original_prototype__

#### [module common-errors.URIError.prototype](#apidoc.module.common-errors.URIError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.URIError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.URIError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.URIError.prototype.</span>generateMessage

#### [module common-errors.Validation](#apidoc.module.common-errors.Validation)
1.  [function <span class="apidocSignatureSpan">common-errors.</span>Validation (message, code, field)](#apidoc.element.common-errors.Validation.Validation)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Validation.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.</span>super_ ()](#apidoc.element.common-errors.Validation.super_)
1.  object <span class="apidocSignatureSpan">common-errors.Validation.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.Validation.</span>__original_prototype__

#### [module common-errors.Validation.prototype](#apidoc.module.common-errors.Validation.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>addError (error)](#apidoc.element.common-errors.Validation.prototype.addError)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>addErrors (errors)](#apidoc.element.common-errors.Validation.prototype.addErrors)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>generateMessage ()](#apidoc.element.common-errors.Validation.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Validation.prototype.global_initialize)
1.  [function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>toJSON ()](#apidoc.element.common-errors.Validation.prototype.toJSON)

#### [module common-errors.data](#apidoc.module.common-errors.data)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>DataError (message, inner_error)](#apidoc.element.common-errors.data.DataError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>MemcachedError (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>MongoDBError (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>RedisError (message, inner_error)](#apidoc.element.common-errors.data.RedisError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>RollbackError (message, inner_error)](#apidoc.element.common-errors.data.RollbackError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>SQLError (message, inner_error)](#apidoc.element.common-errors.data.SQLError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>TransactionError (message, inner_error)](#apidoc.element.common-errors.data.TransactionError)

#### [module common-errors.data.DataError](#apidoc.module.common-errors.data.DataError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>DataError (message, inner_error)](#apidoc.element.common-errors.data.DataError.DataError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.DataError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.DataError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.DataError.</span>super_ ()](#apidoc.element.common-errors.data.DataError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.DataError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.DataError.</span>__original_prototype__

#### [module common-errors.data.DataError.prototype](#apidoc.module.common-errors.data.DataError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.DataError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.DataError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.DataError.prototype.</span>generateMessage

#### [module common-errors.data.MemcachedError](#apidoc.module.common-errors.data.MemcachedError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>MemcachedError (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError.MemcachedError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.MemcachedError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.MemcachedError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.MemcachedError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.MemcachedError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.MemcachedError.</span>__original_prototype__

#### [module common-errors.data.MemcachedError.prototype](#apidoc.module.common-errors.data.MemcachedError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.MemcachedError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.MemcachedError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.MemcachedError.prototype.</span>generateMessage

#### [module common-errors.data.MongoDBError](#apidoc.module.common-errors.data.MongoDBError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>MongoDBError (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError.MongoDBError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.MongoDBError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.MongoDBError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.MongoDBError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.MongoDBError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.MongoDBError.</span>__original_prototype__

#### [module common-errors.data.MongoDBError.prototype](#apidoc.module.common-errors.data.MongoDBError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.MongoDBError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.MongoDBError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.MongoDBError.prototype.</span>generateMessage

#### [module common-errors.data.RedisError](#apidoc.module.common-errors.data.RedisError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>RedisError (message, inner_error)](#apidoc.element.common-errors.data.RedisError.RedisError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.RedisError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.RedisError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.RedisError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.RedisError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.RedisError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.RedisError.</span>__original_prototype__

#### [module common-errors.data.RedisError.prototype](#apidoc.module.common-errors.data.RedisError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.RedisError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.RedisError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.RedisError.prototype.</span>generateMessage

#### [module common-errors.data.RollbackError](#apidoc.module.common-errors.data.RollbackError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>RollbackError (message, inner_error)](#apidoc.element.common-errors.data.RollbackError.RollbackError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.RollbackError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.RollbackError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.RollbackError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.RollbackError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.RollbackError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.RollbackError.</span>__original_prototype__

#### [module common-errors.data.RollbackError.prototype](#apidoc.module.common-errors.data.RollbackError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.RollbackError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.RollbackError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.RollbackError.prototype.</span>generateMessage

#### [module common-errors.data.SQLError](#apidoc.module.common-errors.data.SQLError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>SQLError (message, inner_error)](#apidoc.element.common-errors.data.SQLError.SQLError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.SQLError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.SQLError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.SQLError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.SQLError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.SQLError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.SQLError.</span>__original_prototype__

#### [module common-errors.data.SQLError.prototype](#apidoc.module.common-errors.data.SQLError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.SQLError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.SQLError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.SQLError.prototype.</span>generateMessage

#### [module common-errors.data.TransactionError](#apidoc.module.common-errors.data.TransactionError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.</span>TransactionError (message, inner_error)](#apidoc.element.common-errors.data.TransactionError.TransactionError)
1.  [function <span class="apidocSignatureSpan">common-errors.data.TransactionError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.TransactionError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.data.TransactionError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.TransactionError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.data.TransactionError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.data.TransactionError.</span>__original_prototype__

#### [module common-errors.data.TransactionError.prototype](#apidoc.module.common-errors.data.TransactionError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.data.TransactionError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.TransactionError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.data.TransactionError.prototype.</span>generateMessage

#### [module common-errors.helpers](#apidoc.module.common-errors.helpers)
1.  [function <span class="apidocSignatureSpan">common-errors.helpers.</span>generateClass (name, options)](#apidoc.element.common-errors.helpers.generateClass)

#### [module common-errors.io](#apidoc.module.common-errors.io)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>DirectoryNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>DriveNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>EndOfStreamError (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>FileLoadError (file_name, inner_error)](#apidoc.element.common-errors.io.FileLoadError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>FileNotFoundError (file_name, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>IOError (message, inner_error)](#apidoc.element.common-errors.io.IOError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>SocketError (message, inner_error)](#apidoc.element.common-errors.io.SocketError)

#### [module common-errors.io.DirectoryNotFoundError](#apidoc.module.common-errors.io.DirectoryNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>DirectoryNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError.DirectoryNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.DirectoryNotFoundError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.</span>__original_prototype__

#### [module common-errors.io.DirectoryNotFoundError.prototype](#apidoc.module.common-errors.io.DirectoryNotFoundError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.DirectoryNotFoundError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.prototype.</span>generateMessage

#### [module common-errors.io.DriveNotFoundError](#apidoc.module.common-errors.io.DriveNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>DriveNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError.DriveNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.DriveNotFoundError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.</span>__original_prototype__

#### [module common-errors.io.DriveNotFoundError.prototype](#apidoc.module.common-errors.io.DriveNotFoundError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.DriveNotFoundError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.prototype.</span>generateMessage

#### [module common-errors.io.EndOfStreamError](#apidoc.module.common-errors.io.EndOfStreamError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>EndOfStreamError (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError.EndOfStreamError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.EndOfStreamError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.</span>__original_prototype__

#### [module common-errors.io.EndOfStreamError.prototype](#apidoc.module.common-errors.io.EndOfStreamError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.EndOfStreamError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.prototype.</span>generateMessage

#### [module common-errors.io.FileLoadError](#apidoc.module.common-errors.io.FileLoadError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>FileLoadError (file_name, inner_error)](#apidoc.element.common-errors.io.FileLoadError.FileLoadError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.FileLoadError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.FileLoadError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.FileLoadError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.FileLoadError.</span>__original_prototype__

#### [module common-errors.io.FileLoadError.prototype](#apidoc.module.common-errors.io.FileLoadError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.io.FileLoadError.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.FileLoadError.prototype.global_initialize)

#### [module common-errors.io.FileNotFoundError](#apidoc.module.common-errors.io.FileNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>FileNotFoundError (file_name, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError.FileNotFoundError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.FileNotFoundError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.</span>__original_prototype__

#### [module common-errors.io.FileNotFoundError.prototype](#apidoc.module.common-errors.io.FileNotFoundError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.io.FileNotFoundError.prototype.generateMessage)
1.  [function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.FileNotFoundError.prototype.global_initialize)

#### [module common-errors.io.IOError](#apidoc.module.common-errors.io.IOError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>IOError (message, inner_error)](#apidoc.element.common-errors.io.IOError.IOError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.IOError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.IOError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.IOError.</span>super_ ()](#apidoc.element.common-errors.io.IOError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.IOError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.IOError.</span>__original_prototype__

#### [module common-errors.io.IOError.prototype](#apidoc.module.common-errors.io.IOError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.IOError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.IOError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.io.IOError.prototype.</span>generateMessage

#### [module common-errors.io.SocketError](#apidoc.module.common-errors.io.SocketError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.</span>SocketError (message, inner_error)](#apidoc.element.common-errors.io.SocketError.SocketError)
1.  [function <span class="apidocSignatureSpan">common-errors.io.SocketError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.SocketError.captureStackTrace)
1.  [function <span class="apidocSignatureSpan">common-errors.io.SocketError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.SocketError.super_)
1.  object <span class="apidocSignatureSpan">common-errors.io.SocketError.</span>__global_prototype__
1.  object <span class="apidocSignatureSpan">common-errors.io.SocketError.</span>__original_prototype__

#### [module common-errors.io.SocketError.prototype](#apidoc.module.common-errors.io.SocketError.prototype)
1.  [function <span class="apidocSignatureSpan">common-errors.io.SocketError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.SocketError.prototype.global_initialize)
1.  object <span class="apidocSignatureSpan">common-errors.io.SocketError.prototype.</span>generateMessage

#### [module common-errors.middleware](#apidoc.module.common-errors.middleware)
1.  [function <span class="apidocSignatureSpan">common-errors.middleware.</span>crashProtector (errorHandler)](#apidoc.element.common-errors.middleware.crashProtector)
1.  [function <span class="apidocSignatureSpan">common-errors.middleware.</span>errorHandler (err, req, res, next)](#apidoc.element.common-errors.middleware.errorHandler)



# <a name="apidoc.module.common-errors"></a>[module common-errors](#apidoc.module.common-errors)

#### <a name="apidoc.element.common-errors.AlreadyInUse"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse (entity_name, arg1, arg2, arg3, arg4)](#apidoc.element.common-errors.AlreadyInUse)
- description and source-code
```javascript
function AlreadyInUseError(entity_name, arg1, arg2, arg3, arg4){if(!(this instanceof AlreadyInUseError)) {var instance = Object.
create(AlreadyInUseError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AlreadyInUse.super_"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse.super_ ()](#apidoc.element.common-errors.AlreadyInUse.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AlreadyInUseError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUseError (entity_name, arg1, arg2, arg3, arg4)](#apidoc.element.common-errors.AlreadyInUseError)
- description and source-code
```javascript
function AlreadyInUseError(entity_name, arg1, arg2, arg3, arg4){if(!(this instanceof AlreadyInUseError)) {var instance = Object.
create(AlreadyInUseError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'entityName' - the entity that owns the protected resource
* 'args' - the fields or attributes that are already in use

'''js
// Example
throw new errors.AlreadyInUseError('user', 'username');
'''

---------------------------------------

<a name="argument" />
### ArgumentError
...
```

#### <a name="apidoc.element.common-errors.Argument"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Argument (argumentName, inner_error)](#apidoc.element.common-errors.Argument)
- description and source-code
```javascript
function ArgumentError(argumentName, inner_error){if(!(this instanceof ArgumentError)) {var instance = Object.create(ArgumentError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ArgumentError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ArgumentError (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentError)
- description and source-code
```javascript
function ArgumentError(argumentName, inner_error){if(!(this instanceof ArgumentError)) {var instance = Object.create(ArgumentError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'argumentName' - the name of the argument that has a problem
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ArgumentError('username', err);
'''

---------------------------------------

<a name="argumentnull" />
### ArgumentNullError
...
```

#### <a name="apidoc.element.common-errors.ArgumentNull"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ArgumentNull (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNull)
- description and source-code
```javascript
function ArgumentNullError(argumentName, inner_error){if(!(this instanceof ArgumentNullError)) {var instance = Object.create(ArgumentNullError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ArgumentNullError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ArgumentNullError (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNullError)
- description and source-code
```javascript
function ArgumentNullError(argumentName, inner_error){if(!(this instanceof ArgumentNullError)) {var instance = Object.create(ArgumentNullError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'argumentName' - the name of the argument that is null
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ArgumentNullError('username', err);
'''

---------------------------------------

<a name="authrequired" />
### AuthenticationRequiredError
...
```

#### <a name="apidoc.element.common-errors.AuthenticationRequired"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequired (message, inner_error)](#apidoc.element.common-errors.AuthenticationRequired)
- description and source-code
```javascript
function AuthenticationRequiredError(message, inner_error){if(!(this instanceof AuthenticationRequiredError)) {var instance = Object
.create(AuthenticationRequiredError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor
.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AuthenticationRequiredError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequiredError (message, inner_error)](#apidoc.element.common-errors.AuthenticationRequiredError)
- description and source-code
```javascript
function AuthenticationRequiredError(message, inner_error){if(!(this instanceof AuthenticationRequiredError)) {var instance = Object
.create(AuthenticationRequiredError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor
.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.AuthenticationRequiredError("Please provide authentication.", err)
'''

---------------------------------------

<a name="connection" />
### ConnectionError
...
```

#### <a name="apidoc.element.common-errors.ConnectionError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ConnectionError (message, inner_error)](#apidoc.element.common-errors.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, inner_error){if(!(this instanceof ConnectionError)) {var instance = Object.create(ConnectionError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ConnectionError('database connection no longer available', err);
'''

---------------------------------------

<a name="data" />
### DataError
...
```

#### <a name="apidoc.element.common-errors.Error"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Error (message, inner_error)](#apidoc.element.common-errors.Error)
- description and source-code
```javascript
function Error(message, inner_error){if(!(this instanceof Error)) {var instance = Object.create(Error.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.Error("Please provide authentication.", err)
'''

---------------------------------------

<a name="httpstatus" />
### HttpStatusError
...
```

#### <a name="apidoc.element.common-errors.Generic"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Generic (message, inner_error)](#apidoc.element.common-errors.Generic)
- description and source-code
```javascript
function GenericError(message, inner_error){if(!(this instanceof GenericError)) {var instance = Object.create(GenericError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.HttpStatus"></a>[function <span class="apidocSignatureSpan">common-errors.</span>HttpStatus (status_code, message)](#apidoc.element.common-errors.HttpStatus)
- description and source-code
```javascript
function HttpStatusError(status_code, message) {
  if(!(this instanceof HttpStatusError)) {
    var instance = Object.create(HttpStatusError.prototype);
    HttpStatusError.apply(instance, arguments);
    return instance;
  }

  if(typeof message == 'number' && typeof status_code != 'number') {
    //old interface, so swap.
    var c = message;
    message = status_code;
    status_code = c;
  } else if(status_code instanceof Error) {
    var err = status_code;
    var req = message;
    status_code = err.statusCode || err.status_code || err[STATUS_CODE_ATTRIBUTE_NAME];
    if(typeof status_code != "number") {
      status_code = code_map[err.name];
      if(typeof status_code == "function") {
        status_code(err, req);
        status_code = err.status_code;
      }
      status_code = status_code || 500;
    }
    message = err.message;
    this.stack = err.stack;
  }

  this.status_code = this.statusCode = this[STATUS_CODE_ATTRIBUTE_NAME] = status_code || 500;
  this.name = "HttpStatusError";

  var http_message = "(" + this.status_code + ") " + message_map[status_code] || message_map[status_code >= 500 ? 500 : 400];
  this.message = message || http_message;
  if(!this.stack) Error.captureStackTrace(this, HttpStatusError);
  if(message) this.stack = http_message + "\n" + this.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.HttpStatusError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>HttpStatusError (status_code, message)](#apidoc.element.common-errors.HttpStatusError)
- description and source-code
```javascript
function HttpStatusError(status_code, message) {
  if(!(this instanceof HttpStatusError)) {
    var instance = Object.create(HttpStatusError.prototype);
    HttpStatusError.apply(instance, arguments);
    return instance;
  }

  if(typeof message == 'number' && typeof status_code != 'number') {
    //old interface, so swap.
    var c = message;
    message = status_code;
    status_code = c;
  } else if(status_code instanceof Error) {
    var err = status_code;
    var req = message;
    status_code = err.statusCode || err.status_code || err[STATUS_CODE_ATTRIBUTE_NAME];
    if(typeof status_code != "number") {
      status_code = code_map[err.name];
      if(typeof status_code == "function") {
        status_code(err, req);
        status_code = err.status_code;
      }
      status_code = status_code || 500;
    }
    message = err.message;
    this.stack = err.stack;
  }

  this.status_code = this.statusCode = this[STATUS_CODE_ATTRIBUTE_NAME] = status_code || 500;
  this.name = "HttpStatusError";

  var http_message = "(" + this.status_code + ") " + message_map[status_code] || message_map[status_code >= 500 ? 500 : 400];
  this.message = message || http_message;
  if(!this.stack) Error.captureStackTrace(this, HttpStatusError);
  if(message) this.stack = http_message + "\n" + this.stack;
}
```
- example usage
```shell
...
__Arguments__

* 'status_code' - any HTTP status code integer
* 'message' - any message

'''js
// Example
throw new errors.HttpStatusError(404, "Not Found");
'''

	new HttpStatusError(err[, req])

Figure out a proper status code and message from a given error.
To change the mappings, modify 'HttpStatusError.message_map' and 'HttpStatusError.code_map'
...
```

#### <a name="apidoc.element.common-errors.InvalidOperationError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>InvalidOperationError (message, inner_error)](#apidoc.element.common-errors.InvalidOperationError)
- description and source-code
```javascript
function InvalidOperationError(message, inner_error){if(!(this instanceof InvalidOperationError)) {var instance = Object.create(
InvalidOperationError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.InvalidOperationError('divide by zero', err);
'''

---------------------------------------

<a name="io" />
### IOError
...
```

#### <a name="apidoc.element.common-errors.NotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotFoundError (entity_name, inner_error)](#apidoc.element.common-errors.NotFoundError)
- description and source-code
```javascript
function NotFoundError(entity_name, inner_error){if(!(this instanceof NotFoundError)) {var instance = Object.create(NotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'entity_name' - a description for what was not found
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.NotFoundError("User", err)
'''

---------------------------------------

<a name="notimplemented" />
### NotImplementedError
...
```

#### <a name="apidoc.element.common-errors.NotImplementedError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotImplementedError (message, inner_error)](#apidoc.element.common-errors.NotImplementedError)
- description and source-code
```javascript
function NotImplementedError(message, inner_error){if(!(this instanceof NotImplementedError)) {var instance = Object.create(NotImplementedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.NotImplementedError("Method is not yet implemented.", err)
'''

---------------------------------------

<a name="notpermitted" />
### NotPermittedError
...
```

#### <a name="apidoc.element.common-errors.NotPermitted"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotPermitted (message, inner_error)](#apidoc.element.common-errors.NotPermitted)
- description and source-code
```javascript
function NotPermittedError(message, inner_error){if(!(this instanceof NotPermittedError)) {var instance = Object.create(NotPermittedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotPermittedError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotPermittedError (message, inner_error)](#apidoc.element.common-errors.NotPermittedError)
- description and source-code
```javascript
function NotPermittedError(message, inner_error){if(!(this instanceof NotPermittedError)) {var instance = Object.create(NotPermittedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.NotPermittedError("username cannot be changed once set.", err)
'''

---------------------------------------

<a name="notsupported" />
### NotSupportedError
...
```

#### <a name="apidoc.element.common-errors.NotSupported"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotSupported (message, inner_error)](#apidoc.element.common-errors.NotSupported)
- description and source-code
```javascript
function NotSupportedError(message, inner_error){if(!(this instanceof NotSupportedError)) {var instance = Object.create(NotSupportedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotSupportedError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotSupportedError (message, inner_error)](#apidoc.element.common-errors.NotSupportedError)
- description and source-code
```javascript
function NotSupportedError(message, inner_error){if(!(this instanceof NotSupportedError)) {var instance = Object.create(NotSupportedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.NotSupportedError('Zero values', err);
'''

---------------------------------------

<a name="outofmemory" />
### OutOfMemoryError
...
```

#### <a name="apidoc.element.common-errors.OutOfMemoryError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>OutOfMemoryError (message, inner_error)](#apidoc.element.common-errors.OutOfMemoryError)
- description and source-code
```javascript
function OutOfMemoryError(message, inner_error){if(!(this instanceof OutOfMemoryError)) {var instance = Object.create(OutOfMemoryError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.OutOfMemoryError('Maximum mem size exceeded.', err);
'''

---------------------------------------

<a name="range" />
### RangeError
...
```

#### <a name="apidoc.element.common-errors.RangeError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>RangeError (message, inner_error)](#apidoc.element.common-errors.RangeError)
- description and source-code
```javascript
function RangeError(message, inner_error){if(!(this instanceof RangeError)) {var instance = Object.create(RangeError.prototype);
classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.RangeError("Value must be between " + MIN + " and " + MAX, err);
'''

---------------------------------------

<a name="reference" />
### ReferenceError
...
```

#### <a name="apidoc.element.common-errors.ReferenceError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ReferenceError (message, inner_error)](#apidoc.element.common-errors.ReferenceError)
- description and source-code
```javascript
function ReferenceError(message, inner_error){if(!(this instanceof ReferenceError)) {var instance = Object.create(ReferenceError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ReferenceError("x is not defined", err);
'''

---------------------------------------

<a name="stackoverflow" />
### StackOverflowError
...
```

#### <a name="apidoc.element.common-errors.StackOverflowError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>StackOverflowError (message, inner_error)](#apidoc.element.common-errors.StackOverflowError)
- description and source-code
```javascript
function StackOverflowError(message, inner_error){if(!(this instanceof StackOverflowError)) {var instance = Object.create(StackOverflowError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.StackOverflowError('Stack overflow detected.', err);
'''

---------------------------------------

<a name="syntax" />
### SyntaxError
...
```

#### <a name="apidoc.element.common-errors.SyntaxError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>SyntaxError (message, inner_error)](#apidoc.element.common-errors.SyntaxError)
- description and source-code
```javascript
function SyntaxError(message, inner_error){if(!(this instanceof SyntaxError)) {var instance = Object.create(SyntaxError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.SyntaxError("Unexpected token a", err);
'''

---------------------------------------

<a name="timeout" />
### TimeoutError
...
```

#### <a name="apidoc.element.common-errors.TimeoutError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>TimeoutError (time, inner_error)](#apidoc.element.common-errors.TimeoutError)
- description and source-code
```javascript
function TimeoutError(time, inner_error){if(!(this instanceof TimeoutError)) {var instance = Object.create(TimeoutError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'time' - a time duration
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.TimeoutError('100ms', err);
'''

---------------------------------------

<a name="type" />
### TypeError
...
```

#### <a name="apidoc.element.common-errors.TypeError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>TypeError (message, inner_error)](#apidoc.element.common-errors.TypeError)
- description and source-code
```javascript
function TypeError(message, inner_error){if(!(this instanceof TypeError)) {var instance = Object.create(TypeError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.TypeError("number is not a function", err);
'''

---------------------------------------

<a name="uri" />
### URIError
...
```

#### <a name="apidoc.element.common-errors.URIError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>URIError (message, inner_error)](#apidoc.element.common-errors.URIError)
- description and source-code
```javascript
function URIError(message, inner_error){if(!(this instanceof URIError)) {var instance = Object.create(URIError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.URIError("URI malformed", err);
'''

---------------------------------------

<a name="validation" />
### ValidationError
...
```

#### <a name="apidoc.element.common-errors.Validation"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Validation (message, code, field)](#apidoc.element.common-errors.Validation)
- description and source-code
```javascript
function ValidationError(message, code, field){if(!(this instanceof ValidationError)) {var instance = Object.create(ValidationError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ValidationError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ValidationError (message, code, field)](#apidoc.element.common-errors.ValidationError)
- description and source-code
```javascript
function ValidationError(message, code, field){if(!(this instanceof ValidationError)) {var instance = Object.create(ValidationError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...

* 'addError(error)' - add an error object to the 'errors' array, and return 'this'.
* 'addErrors(errors)' - append an array of error objects to the 'errors' array, and return 'this'.

'''js
// Example
function validateUsername(username){
	var errors = new errors.ValidationError();
	if(username.length < 3) errors.addError(new errors.ValidationError("username must be at least two characters long", "VAL_MIN_USERNAME_LENGTH
", "username"));
	if(/-%$*&!/.test(username)) errors.addError(new errors.ValidationError("username may not contain special characters", "VAL_USERNAME_SPECIALCHARS
", "username"));
	return errors;
}
'''

## Utility Functions
...
```

#### <a name="apidoc.element.common-errors.data.DataError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.DataError (message, inner_error)](#apidoc.element.common-errors.data.DataError)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.DataError('Too many rows returned from database', err);
'''

---------------------------------------

<a name="memcached" />
### MemcachedError
...
```

#### <a name="apidoc.element.common-errors.data.MemcachedError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.MemcachedError (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError)
- description and source-code
```javascript
function MemcachedError(message, inner_error){if(!(this instanceof MemcachedError)) {var instance = Object.create(MemcachedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.MemcachedError('Expected value not found', err);
'''

---------------------------------------

<a name="mongodb" />
### MongoDBError
...
```

#### <a name="apidoc.element.common-errors.data.MongoDBError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.MongoDBError (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError)
- description and source-code
```javascript
function MongoDBError(message, inner_error){if(!(this instanceof MongoDBError)) {var instance = Object.create(MongoDBError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.MongoDBError('Retrieved value not in expected format', err);
'''

---------------------------------------

<a name="redis" />
### RedisError
...
```

#### <a name="apidoc.element.common-errors.data.RedisError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.RedisError (message, inner_error)](#apidoc.element.common-errors.data.RedisError)
- description and source-code
```javascript
function RedisError(message, inner_error){if(!(this instanceof RedisError)) {var instance = Object.create(RedisError.prototype);
classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.RedisError('expected value not found in redis', err);
'''

---------------------------------------

<a name="rollback" />
### RollbackError
...
```

#### <a name="apidoc.element.common-errors.data.RollbackError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.RollbackError (message, inner_error)](#apidoc.element.common-errors.data.RollbackError)
- description and source-code
```javascript
function RollbackError(message, inner_error){if(!(this instanceof RollbackError)) {var instance = Object.create(RollbackError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.RollbackError('database transaction was unexpectedly rolled back', err);
'''

---------------------------------------

<a name="sql" />
### SQLError
...
```

#### <a name="apidoc.element.common-errors.data.SQLError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.SQLError (message, inner_error)](#apidoc.element.common-errors.data.SQLError)
- description and source-code
```javascript
function SQLError(message, inner_error){if(!(this instanceof SQLError)) {var instance = Object.create(SQLError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.SQLError('foreign key constraint violated', err);
'''

---------------------------------------

<a name="transaction" />
### TransactionError
...
```

#### <a name="apidoc.element.common-errors.data.TransactionError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>data.TransactionError (message, inner_error)](#apidoc.element.common-errors.data.TransactionError)
- description and source-code
```javascript
function TransactionError(message, inner_error){if(!(this instanceof TransactionError)) {var instance = Object.create(TransactionError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.TransactionError('transaction already complete', err);
'''

---------------------------------------

<a name="error" />
### Error
...
```

#### <a name="apidoc.element.common-errors.io.DirectoryNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.DirectoryNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError)
- description and source-code
```javascript
function DirectoryNotFoundError(message, inner_error){if(!(this instanceof DirectoryNotFoundError)) {var instance = Object.create
(DirectoryNotFoundError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.DirectoryNotFoundError("/var/log", err)
'''

---------------------------------------

<a name="drivenotfound" />
### DriveNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.DriveNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.DriveNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError)
- description and source-code
```javascript
function DriveNotFoundError(message, inner_error){if(!(this instanceof DriveNotFoundError)) {var instance = Object.create(DriveNotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.DriveNotFoundError("c", err)
'''

---------------------------------------

<a name="endofstream" />
### EndOfStreamError
...
```

#### <a name="apidoc.element.common-errors.io.EndOfStreamError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.EndOfStreamError (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError)
- description and source-code
```javascript
function EndOfStreamError(message, inner_error){if(!(this instanceof EndOfStreamError)) {var instance = Object.create(EndOfStreamError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.EndOfStreamError("EOS while reading header", err)
'''

---------------------------------------

<a name="fileload" />
### FileLoadError
...
```

#### <a name="apidoc.element.common-errors.io.FileLoadError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.FileLoadError (file_name, inner_error)](#apidoc.element.common-errors.io.FileLoadError)
- description and source-code
```javascript
function FileLoadError(file_name, inner_error){if(!(this instanceof FileLoadError)) {var instance = Object.create(FileLoadError.
prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'file_name' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.FileLoadError("./package.json", err)
'''

---------------------------------------

<a name="filenotfound" />
### FileNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.FileNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.FileNotFoundError (file_name, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError)
- description and source-code
```javascript
function FileNotFoundError(file_name, inner_error){if(!(this instanceof FileNotFoundError)) {var instance = Object.create(FileNotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'file_name' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.FileNotFoundError("./package.json", err)
'''

---------------------------------------

<a name="socket" />
### SocketError
...
```

#### <a name="apidoc.element.common-errors.io.IOError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.IOError (message, inner_error)](#apidoc.element.common-errors.io.IOError)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.IOError("Could not open file", err)
'''

---------------------------------------

<a name="directorynotfound" />
### DirectoryNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.SocketError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>io.SocketError (message, inner_error)](#apidoc.element.common-errors.io.SocketError)
- description and source-code
```javascript
function SocketError(message, inner_error){if(!(this instanceof SocketError)) {var instance = Object.create(SocketError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.log"></a>[function <span class="apidocSignatureSpan">common-errors.</span>log (err, message)](#apidoc.element.common-errors.log)
- description and source-code
```javascript
log = function (err, message) {
  if (typeof err == 'string') {
    err = new module.exports.Error(err);
  } else {
    if (message) {
      err.message = message;
    }
    err = module.exports.prependCurrentStack(err, 3);
  }
  if (err) {
    console.error(err && err.stack || err);
    err.isLogged = true;
  }
  return err;
}
```
- example usage
```shell
...

* 'err' - any error or error message received from a callback
* 'message' - any message you'd like to prepend

'''js
// Example
mysql.query('SELECT * 'FROM' users', function(err, results){
	if(err) return errors.log(err, "Had trouble retrieving users.");
	console.log(results);
});
'''

<a name="prependCurrentStack" />
### prependCurrentStack
...
```

#### <a name="apidoc.element.common-errors.logError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>logError (err, cb)](#apidoc.element.common-errors.logError)
- description and source-code
```javascript
logError = function (err, cb) {
  if (!logErrorDeprecationWarning) console.warn("logError is deprecated.  Use log instead.");
  logErrorDeprecationWarning = true;

  if (err && !err.isLogged) {
    err.isLogged = true;
    console.error(err);
  }
  if (cb) cb(err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.prependCurrentStack"></a>[function <span class="apidocSignatureSpan">common-errors.</span>prependCurrentStack (err, offset_)](#apidoc.element.common-errors.prependCurrentStack)
- description and source-code
```javascript
prependCurrentStack = function (err, offset_) {
  var linesToSkip = (typeof offset_ === 'undefined') ? 2 : offset_;
  var stackToPrepend = (new Error()).stack.split("\n").slice(linesToSkip);
  var mainStack = (err.stack || '').split("\n");
  var errTitle = mainStack.shift();
  err.stack = [errTitle].concat(stackToPrepend, "====", mainStack).join("\n");
  return err;
}
```
- example usage
```shell
...

* 'err' - any error or error message received from a callback

'''js
// Example
mysql.query('SELECT * 'FROM' users', function(err, results){
	if(err) {
		return errors.prependCurrentStack(err); // caller has better idea of source of err
	}
	console.log(results);
});
'''

<a name="generateClass" />
### generateClass
...
```



# <a name="apidoc.module.common-errors.AlreadyInUse"></a>[module common-errors.AlreadyInUse](#apidoc.module.common-errors.AlreadyInUse)

#### <a name="apidoc.element.common-errors.AlreadyInUse.AlreadyInUse"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AlreadyInUse (entity_name, arg1, arg2, arg3, arg4)](#apidoc.element.common-errors.AlreadyInUse.AlreadyInUse)
- description and source-code
```javascript
function AlreadyInUseError(entity_name, arg1, arg2, arg3, arg4){if(!(this instanceof AlreadyInUseError)) {var instance = Object.
create(AlreadyInUseError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AlreadyInUse.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.AlreadyInUse.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AlreadyInUse.super_"></a>[function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>super_ ()](#apidoc.element.common-errors.AlreadyInUse.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.AlreadyInUse.prototype"></a>[module common-errors.AlreadyInUse.prototype](#apidoc.module.common-errors.AlreadyInUse.prototype)

#### <a name="apidoc.element.common-errors.AlreadyInUse.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.prototype.</span>generateMessage ()](#apidoc.element.common-errors.AlreadyInUse.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  var args = Array.prototype.slice.call(this.args, 1);
  return "The specified '" + this.entity_name + "' value is already in use for: " + args.join(', ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AlreadyInUse.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.AlreadyInUse.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.AlreadyInUse.super_"></a>[module common-errors.AlreadyInUse.super_](#apidoc.module.common-errors.AlreadyInUse.super_)

#### <a name="apidoc.element.common-errors.AlreadyInUse.super_.super_"></a>[function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.</span>super_ ()](#apidoc.element.common-errors.AlreadyInUse.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AlreadyInUse.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.AlreadyInUse.super_.</span>captureStackTrace ()](#apidoc.element.common-errors.AlreadyInUse.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Argument"></a>[module common-errors.Argument](#apidoc.module.common-errors.Argument)

#### <a name="apidoc.element.common-errors.Argument.Argument"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Argument (argumentName, inner_error)](#apidoc.element.common-errors.Argument.Argument)
- description and source-code
```javascript
function ArgumentError(argumentName, inner_error){if(!(this instanceof ArgumentError)) {var instance = Object.create(ArgumentError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Argument.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.Argument.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Argument.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Argument.super_"></a>[function <span class="apidocSignatureSpan">common-errors.Argument.</span>super_ ()](#apidoc.element.common-errors.Argument.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Argument.prototype"></a>[module common-errors.Argument.prototype](#apidoc.module.common-errors.Argument.prototype)

#### <a name="apidoc.element.common-errors.Argument.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.Argument.prototype.</span>generateMessage ()](#apidoc.element.common-errors.Argument.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "Invalid or missing argument supplied: " + this.argumentName;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Argument.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.Argument.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Argument.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.ArgumentNull"></a>[module common-errors.ArgumentNull](#apidoc.module.common-errors.ArgumentNull)

#### <a name="apidoc.element.common-errors.ArgumentNull.ArgumentNull"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ArgumentNull (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNull.ArgumentNull)
- description and source-code
```javascript
function ArgumentNullError(argumentName, inner_error){if(!(this instanceof ArgumentNullError)) {var instance = Object.create(ArgumentNullError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ArgumentNull.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.ArgumentNull.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.ArgumentNull.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ArgumentNull.super_"></a>[function <span class="apidocSignatureSpan">common-errors.ArgumentNull.</span>super_ (argumentName, inner_error)](#apidoc.element.common-errors.ArgumentNull.super_)
- description and source-code
```javascript
function ArgumentError(argumentName, inner_error){if(!(this instanceof ArgumentError)) {var instance = Object.create(ArgumentError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.ArgumentNull.prototype"></a>[module common-errors.ArgumentNull.prototype](#apidoc.module.common-errors.ArgumentNull.prototype)

#### <a name="apidoc.element.common-errors.ArgumentNull.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.ArgumentNull.prototype.</span>generateMessage ()](#apidoc.element.common-errors.ArgumentNull.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "Missing argument: " + this.argumentName;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ArgumentNull.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.ArgumentNull.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.ArgumentNull.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.AuthenticationRequired"></a>[module common-errors.AuthenticationRequired](#apidoc.module.common-errors.AuthenticationRequired)

#### <a name="apidoc.element.common-errors.AuthenticationRequired.AuthenticationRequired"></a>[function <span class="apidocSignatureSpan">common-errors.</span>AuthenticationRequired (message, inner_error)](#apidoc.element.common-errors.AuthenticationRequired.AuthenticationRequired)
- description and source-code
```javascript
function AuthenticationRequiredError(message, inner_error){if(!(this instanceof AuthenticationRequiredError)) {var instance = Object
.create(AuthenticationRequiredError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor
.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AuthenticationRequired.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.AuthenticationRequired.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AuthenticationRequired.super_"></a>[function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.</span>super_ ()](#apidoc.element.common-errors.AuthenticationRequired.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.AuthenticationRequired.prototype"></a>[module common-errors.AuthenticationRequired.prototype](#apidoc.module.common-errors.AuthenticationRequired.prototype)

#### <a name="apidoc.element.common-errors.AuthenticationRequired.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.prototype.</span>generateMessage ()](#apidoc.element.common-errors.AuthenticationRequired.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "An attempt was made to perform an operation without authentication: " + this.message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.AuthenticationRequired.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.AuthenticationRequired.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.AuthenticationRequired.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.ConnectionError"></a>[module common-errors.ConnectionError](#apidoc.module.common-errors.ConnectionError)

#### <a name="apidoc.element.common-errors.ConnectionError.ConnectionError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ConnectionError (message, inner_error)](#apidoc.element.common-errors.ConnectionError.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, inner_error){if(!(this instanceof ConnectionError)) {var instance = Object.create(ConnectionError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ConnectionError('database connection no longer available', err);
'''

---------------------------------------

<a name="data" />
### DataError
...
```

#### <a name="apidoc.element.common-errors.ConnectionError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.ConnectionError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.ConnectionError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ConnectionError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.ConnectionError.</span>super_ ()](#apidoc.element.common-errors.ConnectionError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.ConnectionError.prototype"></a>[module common-errors.ConnectionError.prototype](#apidoc.module.common-errors.ConnectionError.prototype)

#### <a name="apidoc.element.common-errors.ConnectionError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.ConnectionError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.ConnectionError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Error"></a>[module common-errors.Error](#apidoc.module.common-errors.Error)

#### <a name="apidoc.element.common-errors.Error.Error"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Error (message, inner_error)](#apidoc.element.common-errors.Error.Error)
- description and source-code
```javascript
function Error(message, inner_error){if(!(this instanceof Error)) {var instance = Object.create(Error.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.Error("Please provide authentication.", err)
'''

---------------------------------------

<a name="httpstatus" />
### HttpStatusError
...
```

#### <a name="apidoc.element.common-errors.Error.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.Error.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Error.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Error.super_"></a>[function <span class="apidocSignatureSpan">common-errors.Error.</span>super_ ()](#apidoc.element.common-errors.Error.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Error.prototype"></a>[module common-errors.Error.prototype](#apidoc.module.common-errors.Error.prototype)

#### <a name="apidoc.element.common-errors.Error.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.Error.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Error.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Generic"></a>[module common-errors.Generic](#apidoc.module.common-errors.Generic)

#### <a name="apidoc.element.common-errors.Generic.Generic"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Generic (message, inner_error)](#apidoc.element.common-errors.Generic.Generic)
- description and source-code
```javascript
function GenericError(message, inner_error){if(!(this instanceof GenericError)) {var instance = Object.create(GenericError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Generic.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.Generic.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Generic.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Generic.super_"></a>[function <span class="apidocSignatureSpan">common-errors.Generic.</span>super_ ()](#apidoc.element.common-errors.Generic.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Generic.prototype"></a>[module common-errors.Generic.prototype](#apidoc.module.common-errors.Generic.prototype)

#### <a name="apidoc.element.common-errors.Generic.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.Generic.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Generic.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.HttpStatus"></a>[module common-errors.HttpStatus](#apidoc.module.common-errors.HttpStatus)

#### <a name="apidoc.element.common-errors.HttpStatus.HttpStatus"></a>[function <span class="apidocSignatureSpan">common-errors.</span>HttpStatus (status_code, message)](#apidoc.element.common-errors.HttpStatus.HttpStatus)
- description and source-code
```javascript
function HttpStatusError(status_code, message) {
  if(!(this instanceof HttpStatusError)) {
    var instance = Object.create(HttpStatusError.prototype);
    HttpStatusError.apply(instance, arguments);
    return instance;
  }

  if(typeof message == 'number' && typeof status_code != 'number') {
    //old interface, so swap.
    var c = message;
    message = status_code;
    status_code = c;
  } else if(status_code instanceof Error) {
    var err = status_code;
    var req = message;
    status_code = err.statusCode || err.status_code || err[STATUS_CODE_ATTRIBUTE_NAME];
    if(typeof status_code != "number") {
      status_code = code_map[err.name];
      if(typeof status_code == "function") {
        status_code(err, req);
        status_code = err.status_code;
      }
      status_code = status_code || 500;
    }
    message = err.message;
    this.stack = err.stack;
  }

  this.status_code = this.statusCode = this[STATUS_CODE_ATTRIBUTE_NAME] = status_code || 500;
  this.name = "HttpStatusError";

  var http_message = "(" + this.status_code + ") " + message_map[status_code] || message_map[status_code >= 500 ? 500 : 400];
  this.message = message || http_message;
  if(!this.stack) Error.captureStackTrace(this, HttpStatusError);
  if(message) this.stack = http_message + "\n" + this.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.HttpStatus.super_"></a>[function <span class="apidocSignatureSpan">common-errors.HttpStatus.</span>super_ ()](#apidoc.element.common-errors.HttpStatus.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.HttpStatus.code_map"></a>[module common-errors.HttpStatus.code_map](#apidoc.module.common-errors.HttpStatus.code_map)

#### <a name="apidoc.element.common-errors.HttpStatus.code_map.ArgumentNullError"></a>[function <span class="apidocSignatureSpan">common-errors.HttpStatus.code_map.</span>ArgumentNullError (err, req)](#apidoc.element.common-errors.HttpStatus.code_map.ArgumentNullError)
- description and source-code
```javascript
ArgumentNullError = function (err, req){
  var method = req && req.method || 'GET';
  var params = req && req.params || {};
  var route_path = req && req.route && req.route.path || '';

  if(/GET|HEAD/i.test(method) || params.hasOwnProperty(err.argumentName) || new RegExp(":" + err.argumentName + '').test(route_path
 + '/')) err.status_code = 404;
  else err.status_code = 400;
  err.message = err.message.replace(new RegExp("^Missing argument: (" + err.argumentName + ")$"), 'Not Found: "$1"' );
}
```
- example usage
```shell
...
__Arguments__

* 'argumentName' - the name of the argument that is null
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ArgumentNullError('username', err);
'''

---------------------------------------

<a name="authrequired" />
### AuthenticationRequiredError
...
```



# <a name="apidoc.module.common-errors.InvalidOperationError"></a>[module common-errors.InvalidOperationError](#apidoc.module.common-errors.InvalidOperationError)

#### <a name="apidoc.element.common-errors.InvalidOperationError.InvalidOperationError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>InvalidOperationError (message, inner_error)](#apidoc.element.common-errors.InvalidOperationError.InvalidOperationError)
- description and source-code
```javascript
function InvalidOperationError(message, inner_error){if(!(this instanceof InvalidOperationError)) {var instance = Object.create(
InvalidOperationError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.InvalidOperationError('divide by zero', err);
'''

---------------------------------------

<a name="io" />
### IOError
...
```

#### <a name="apidoc.element.common-errors.InvalidOperationError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.InvalidOperationError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.InvalidOperationError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.</span>super_ ()](#apidoc.element.common-errors.InvalidOperationError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.InvalidOperationError.prototype"></a>[module common-errors.InvalidOperationError.prototype](#apidoc.module.common-errors.InvalidOperationError.prototype)

#### <a name="apidoc.element.common-errors.InvalidOperationError.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.InvalidOperationError.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "Invalid Operation: " + this.message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.InvalidOperationError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.InvalidOperationError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.InvalidOperationError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotFoundError"></a>[module common-errors.NotFoundError](#apidoc.module.common-errors.NotFoundError)

#### <a name="apidoc.element.common-errors.NotFoundError.NotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotFoundError (entity_name, inner_error)](#apidoc.element.common-errors.NotFoundError.NotFoundError)
- description and source-code
```javascript
function NotFoundError(entity_name, inner_error){if(!(this instanceof NotFoundError)) {var instance = Object.create(NotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'entity_name' - a description for what was not found
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.NotFoundError("User", err)
'''

---------------------------------------

<a name="notimplemented" />
### NotImplementedError
...
```

#### <a name="apidoc.element.common-errors.NotFoundError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.NotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotFoundError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotFoundError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.NotFoundError.</span>super_ ()](#apidoc.element.common-errors.NotFoundError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotFoundError.prototype"></a>[module common-errors.NotFoundError.prototype](#apidoc.module.common-errors.NotFoundError.prototype)

#### <a name="apidoc.element.common-errors.NotFoundError.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.NotFoundError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.NotFoundError.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return 'Not Found: "' + this.entity_name + '"';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotFoundError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.NotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotFoundError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotImplementedError"></a>[module common-errors.NotImplementedError](#apidoc.module.common-errors.NotImplementedError)

#### <a name="apidoc.element.common-errors.NotImplementedError.NotImplementedError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotImplementedError (message, inner_error)](#apidoc.element.common-errors.NotImplementedError.NotImplementedError)
- description and source-code
```javascript
function NotImplementedError(message, inner_error){if(!(this instanceof NotImplementedError)) {var instance = Object.create(NotImplementedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.NotImplementedError("Method is not yet implemented.", err)
'''

---------------------------------------

<a name="notpermitted" />
### NotPermittedError
...
```

#### <a name="apidoc.element.common-errors.NotImplementedError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.NotImplementedError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotImplementedError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotImplementedError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.NotImplementedError.</span>super_ ()](#apidoc.element.common-errors.NotImplementedError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotImplementedError.prototype"></a>[module common-errors.NotImplementedError.prototype](#apidoc.module.common-errors.NotImplementedError.prototype)

#### <a name="apidoc.element.common-errors.NotImplementedError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.NotImplementedError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotImplementedError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotPermitted"></a>[module common-errors.NotPermitted](#apidoc.module.common-errors.NotPermitted)

#### <a name="apidoc.element.common-errors.NotPermitted.NotPermitted"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotPermitted (message, inner_error)](#apidoc.element.common-errors.NotPermitted.NotPermitted)
- description and source-code
```javascript
function NotPermittedError(message, inner_error){if(!(this instanceof NotPermittedError)) {var instance = Object.create(NotPermittedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotPermitted.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.NotPermitted.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotPermitted.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotPermitted.super_"></a>[function <span class="apidocSignatureSpan">common-errors.NotPermitted.</span>super_ ()](#apidoc.element.common-errors.NotPermitted.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotPermitted.prototype"></a>[module common-errors.NotPermitted.prototype](#apidoc.module.common-errors.NotPermitted.prototype)

#### <a name="apidoc.element.common-errors.NotPermitted.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.NotPermitted.prototype.</span>generateMessage ()](#apidoc.element.common-errors.NotPermitted.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "An attempt was made to perform an operation that is not permitted: " + this.message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotPermitted.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.NotPermitted.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotPermitted.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotSupported"></a>[module common-errors.NotSupported](#apidoc.module.common-errors.NotSupported)

#### <a name="apidoc.element.common-errors.NotSupported.NotSupported"></a>[function <span class="apidocSignatureSpan">common-errors.</span>NotSupported (message, inner_error)](#apidoc.element.common-errors.NotSupported.NotSupported)
- description and source-code
```javascript
function NotSupportedError(message, inner_error){if(!(this instanceof NotSupportedError)) {var instance = Object.create(NotSupportedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotSupported.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.NotSupported.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.NotSupported.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotSupported.super_"></a>[function <span class="apidocSignatureSpan">common-errors.NotSupported.</span>super_ ()](#apidoc.element.common-errors.NotSupported.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.NotSupported.prototype"></a>[module common-errors.NotSupported.prototype](#apidoc.module.common-errors.NotSupported.prototype)

#### <a name="apidoc.element.common-errors.NotSupported.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.NotSupported.prototype.</span>generateMessage ()](#apidoc.element.common-errors.NotSupported.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "Not Supported: " + this.message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.NotSupported.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.NotSupported.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.NotSupported.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.OutOfMemoryError"></a>[module common-errors.OutOfMemoryError](#apidoc.module.common-errors.OutOfMemoryError)

#### <a name="apidoc.element.common-errors.OutOfMemoryError.OutOfMemoryError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>OutOfMemoryError (message, inner_error)](#apidoc.element.common-errors.OutOfMemoryError.OutOfMemoryError)
- description and source-code
```javascript
function OutOfMemoryError(message, inner_error){if(!(this instanceof OutOfMemoryError)) {var instance = Object.create(OutOfMemoryError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.OutOfMemoryError('Maximum mem size exceeded.', err);
'''

---------------------------------------

<a name="range" />
### RangeError
...
```

#### <a name="apidoc.element.common-errors.OutOfMemoryError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.OutOfMemoryError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.OutOfMemoryError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.</span>super_ ()](#apidoc.element.common-errors.OutOfMemoryError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.OutOfMemoryError.prototype"></a>[module common-errors.OutOfMemoryError.prototype](#apidoc.module.common-errors.OutOfMemoryError.prototype)

#### <a name="apidoc.element.common-errors.OutOfMemoryError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.OutOfMemoryError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.OutOfMemoryError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.RangeError"></a>[module common-errors.RangeError](#apidoc.module.common-errors.RangeError)

#### <a name="apidoc.element.common-errors.RangeError.RangeError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>RangeError (message, inner_error)](#apidoc.element.common-errors.RangeError.RangeError)
- description and source-code
```javascript
function RangeError(message, inner_error){if(!(this instanceof RangeError)) {var instance = Object.create(RangeError.prototype);
classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.RangeError("Value must be between " + MIN + " and " + MAX, err);
'''

---------------------------------------

<a name="reference" />
### ReferenceError
...
```

#### <a name="apidoc.element.common-errors.RangeError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.RangeError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.RangeError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.RangeError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.RangeError.</span>super_ ()](#apidoc.element.common-errors.RangeError.super_)
- description and source-code
```javascript
function RangeError() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.RangeError.prototype"></a>[module common-errors.RangeError.prototype](#apidoc.module.common-errors.RangeError.prototype)

#### <a name="apidoc.element.common-errors.RangeError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.RangeError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.RangeError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.ReferenceError"></a>[module common-errors.ReferenceError](#apidoc.module.common-errors.ReferenceError)

#### <a name="apidoc.element.common-errors.ReferenceError.ReferenceError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>ReferenceError (message, inner_error)](#apidoc.element.common-errors.ReferenceError.ReferenceError)
- description and source-code
```javascript
function ReferenceError(message, inner_error){if(!(this instanceof ReferenceError)) {var instance = Object.create(ReferenceError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.ReferenceError("x is not defined", err);
'''

---------------------------------------

<a name="stackoverflow" />
### StackOverflowError
...
```

#### <a name="apidoc.element.common-errors.ReferenceError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.ReferenceError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.ReferenceError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.ReferenceError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.ReferenceError.</span>super_ ()](#apidoc.element.common-errors.ReferenceError.super_)
- description and source-code
```javascript
function ReferenceError() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.ReferenceError.prototype"></a>[module common-errors.ReferenceError.prototype](#apidoc.module.common-errors.ReferenceError.prototype)

#### <a name="apidoc.element.common-errors.ReferenceError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.ReferenceError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.ReferenceError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.StackOverflowError"></a>[module common-errors.StackOverflowError](#apidoc.module.common-errors.StackOverflowError)

#### <a name="apidoc.element.common-errors.StackOverflowError.StackOverflowError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>StackOverflowError (message, inner_error)](#apidoc.element.common-errors.StackOverflowError.StackOverflowError)
- description and source-code
```javascript
function StackOverflowError(message, inner_error){if(!(this instanceof StackOverflowError)) {var instance = Object.create(StackOverflowError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.StackOverflowError('Stack overflow detected.', err);
'''

---------------------------------------

<a name="syntax" />
### SyntaxError
...
```

#### <a name="apidoc.element.common-errors.StackOverflowError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.StackOverflowError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.StackOverflowError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.StackOverflowError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.StackOverflowError.</span>super_ ()](#apidoc.element.common-errors.StackOverflowError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.StackOverflowError.prototype"></a>[module common-errors.StackOverflowError.prototype](#apidoc.module.common-errors.StackOverflowError.prototype)

#### <a name="apidoc.element.common-errors.StackOverflowError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.StackOverflowError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.StackOverflowError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.SyntaxError"></a>[module common-errors.SyntaxError](#apidoc.module.common-errors.SyntaxError)

#### <a name="apidoc.element.common-errors.SyntaxError.SyntaxError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>SyntaxError (message, inner_error)](#apidoc.element.common-errors.SyntaxError.SyntaxError)
- description and source-code
```javascript
function SyntaxError(message, inner_error){if(!(this instanceof SyntaxError)) {var instance = Object.create(SyntaxError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.SyntaxError("Unexpected token a", err);
'''

---------------------------------------

<a name="timeout" />
### TimeoutError
...
```

#### <a name="apidoc.element.common-errors.SyntaxError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.SyntaxError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.SyntaxError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.SyntaxError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.SyntaxError.</span>super_ ()](#apidoc.element.common-errors.SyntaxError.super_)
- description and source-code
```javascript
function SyntaxError() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.SyntaxError.prototype"></a>[module common-errors.SyntaxError.prototype](#apidoc.module.common-errors.SyntaxError.prototype)

#### <a name="apidoc.element.common-errors.SyntaxError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.SyntaxError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.SyntaxError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.TimeoutError"></a>[module common-errors.TimeoutError](#apidoc.module.common-errors.TimeoutError)

#### <a name="apidoc.element.common-errors.TimeoutError.TimeoutError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>TimeoutError (time, inner_error)](#apidoc.element.common-errors.TimeoutError.TimeoutError)
- description and source-code
```javascript
function TimeoutError(time, inner_error){if(!(this instanceof TimeoutError)) {var instance = Object.create(TimeoutError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'time' - a time duration
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.TimeoutError('100ms', err);
'''

---------------------------------------

<a name="type" />
### TypeError
...
```

#### <a name="apidoc.element.common-errors.TimeoutError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.TimeoutError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.TimeoutError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.TimeoutError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.TimeoutError.</span>super_ ()](#apidoc.element.common-errors.TimeoutError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.TimeoutError.prototype"></a>[module common-errors.TimeoutError.prototype](#apidoc.module.common-errors.TimeoutError.prototype)

#### <a name="apidoc.element.common-errors.TimeoutError.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.TimeoutError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.TimeoutError.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
	if(/^\d/.test(this.time)) return "Timeout of '" + this.time + "' exceeded";
	else return "Timeout exceeded: " + this.time;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.TimeoutError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.TimeoutError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.TimeoutError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.TypeError"></a>[module common-errors.TypeError](#apidoc.module.common-errors.TypeError)

#### <a name="apidoc.element.common-errors.TypeError.TypeError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>TypeError (message, inner_error)](#apidoc.element.common-errors.TypeError.TypeError)
- description and source-code
```javascript
function TypeError(message, inner_error){if(!(this instanceof TypeError)) {var instance = Object.create(TypeError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.TypeError("number is not a function", err);
'''

---------------------------------------

<a name="uri" />
### URIError
...
```

#### <a name="apidoc.element.common-errors.TypeError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.TypeError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.TypeError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.TypeError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.TypeError.</span>super_ ()](#apidoc.element.common-errors.TypeError.super_)
- description and source-code
```javascript
function TypeError() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.TypeError.prototype"></a>[module common-errors.TypeError.prototype](#apidoc.module.common-errors.TypeError.prototype)

#### <a name="apidoc.element.common-errors.TypeError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.TypeError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.TypeError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.URIError"></a>[module common-errors.URIError](#apidoc.module.common-errors.URIError)

#### <a name="apidoc.element.common-errors.URIError.URIError"></a>[function <span class="apidocSignatureSpan">common-errors.</span>URIError (message, inner_error)](#apidoc.element.common-errors.URIError.URIError)
- description and source-code
```javascript
function URIError(message, inner_error){if(!(this instanceof URIError)) {var instance = Object.create(URIError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - a message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.URIError("URI malformed", err);
'''

---------------------------------------

<a name="validation" />
### ValidationError
...
```

#### <a name="apidoc.element.common-errors.URIError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.URIError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.URIError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.URIError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.URIError.</span>super_ ()](#apidoc.element.common-errors.URIError.super_)
- description and source-code
```javascript
function URIError() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.URIError.prototype"></a>[module common-errors.URIError.prototype](#apidoc.module.common-errors.URIError.prototype)

#### <a name="apidoc.element.common-errors.URIError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.URIError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.URIError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Validation"></a>[module common-errors.Validation](#apidoc.module.common-errors.Validation)

#### <a name="apidoc.element.common-errors.Validation.Validation"></a>[function <span class="apidocSignatureSpan">common-errors.</span>Validation (message, code, field)](#apidoc.element.common-errors.Validation.Validation)
- description and source-code
```javascript
function ValidationError(message, code, field){if(!(this instanceof ValidationError)) {var instance = Object.create(ValidationError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Validation.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.Validation.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Validation.super_"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.</span>super_ ()](#apidoc.element.common-errors.Validation.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.Validation.prototype"></a>[module common-errors.Validation.prototype](#apidoc.module.common-errors.Validation.prototype)

#### <a name="apidoc.element.common-errors.Validation.prototype.addError"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>addError (error)](#apidoc.element.common-errors.Validation.prototype.addError)
- description and source-code
```javascript
function addError(error) {
  this.errors = this.errors || [];
  this.errors.push(error);
  return this;
}
```
- example usage
```shell
...
* 'addError(error)' - add an error object to the 'errors' array, and return 'this'.
* 'addErrors(errors)' - append an array of error objects to the 'errors' array, and return 'this'.

'''js
// Example
function validateUsername(username){
	var errors = new errors.ValidationError();
	if(username.length < 3) errors.addError(new errors.ValidationError("username must be at least two characters long", "VAL_MIN_USERNAME_LENGTH
", "username"));
	if(/-%$*&!/.test(username)) errors.addError(new errors.ValidationError("username may not contain special characters", "VAL_USERNAME_SPECIALCHARS
", "username"));
	return errors;
}
'''

## Utility Functions
...
```

#### <a name="apidoc.element.common-errors.Validation.prototype.addErrors"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>addErrors (errors)](#apidoc.element.common-errors.Validation.prototype.addErrors)
- description and source-code
```javascript
function addErrors(errors) {
  if(!(errors instanceof Array)) throw new ArgumentError("errors");

  this.errors = this.errors || [];
  Array.prototype.push.apply(this.errors, errors);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Validation.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>generateMessage ()](#apidoc.element.common-errors.Validation.prototype.generateMessage)
- description and source-code
```javascript
function generateMessage(){
  return this.message || "Validation failed.";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Validation.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.Validation.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.Validation.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">common-errors.Validation.prototype.</span>toJSON ()](#apidoc.element.common-errors.Validation.prototype.toJSON)
- description and source-code
```javascript
function toJSON(){
  var o = {};
  if(this.errors) {
    if(this.message) o.message = this.message;
    o.errors = this.errors.map(function(error){
      return error.toJSON();
    });
  } else {
    if(this.message) o.text = this.message;
    if(this.code) o.code = this.code;
    if(this.field) o.field = this.field;
  }
  return o;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data"></a>[module common-errors.data](#apidoc.module.common-errors.data)

#### <a name="apidoc.element.common-errors.data.DataError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>DataError (message, inner_error)](#apidoc.element.common-errors.data.DataError)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.DataError('Too many rows returned from database', err);
'''

---------------------------------------

<a name="memcached" />
### MemcachedError
...
```

#### <a name="apidoc.element.common-errors.data.MemcachedError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>MemcachedError (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError)
- description and source-code
```javascript
function MemcachedError(message, inner_error){if(!(this instanceof MemcachedError)) {var instance = Object.create(MemcachedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.MemcachedError('Expected value not found', err);
'''

---------------------------------------

<a name="mongodb" />
### MongoDBError
...
```

#### <a name="apidoc.element.common-errors.data.MongoDBError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>MongoDBError (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError)
- description and source-code
```javascript
function MongoDBError(message, inner_error){if(!(this instanceof MongoDBError)) {var instance = Object.create(MongoDBError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.MongoDBError('Retrieved value not in expected format', err);
'''

---------------------------------------

<a name="redis" />
### RedisError
...
```

#### <a name="apidoc.element.common-errors.data.RedisError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>RedisError (message, inner_error)](#apidoc.element.common-errors.data.RedisError)
- description and source-code
```javascript
function RedisError(message, inner_error){if(!(this instanceof RedisError)) {var instance = Object.create(RedisError.prototype);
classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.RedisError('expected value not found in redis', err);
'''

---------------------------------------

<a name="rollback" />
### RollbackError
...
```

#### <a name="apidoc.element.common-errors.data.RollbackError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>RollbackError (message, inner_error)](#apidoc.element.common-errors.data.RollbackError)
- description and source-code
```javascript
function RollbackError(message, inner_error){if(!(this instanceof RollbackError)) {var instance = Object.create(RollbackError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.RollbackError('database transaction was unexpectedly rolled back', err);
'''

---------------------------------------

<a name="sql" />
### SQLError
...
```

#### <a name="apidoc.element.common-errors.data.SQLError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>SQLError (message, inner_error)](#apidoc.element.common-errors.data.SQLError)
- description and source-code
```javascript
function SQLError(message, inner_error){if(!(this instanceof SQLError)) {var instance = Object.create(SQLError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.SQLError('foreign key constraint violated', err);
'''

---------------------------------------

<a name="transaction" />
### TransactionError
...
```

#### <a name="apidoc.element.common-errors.data.TransactionError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>TransactionError (message, inner_error)](#apidoc.element.common-errors.data.TransactionError)
- description and source-code
```javascript
function TransactionError(message, inner_error){if(!(this instanceof TransactionError)) {var instance = Object.create(TransactionError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.TransactionError('transaction already complete', err);
'''

---------------------------------------

<a name="error" />
### Error
...
```



# <a name="apidoc.module.common-errors.data.DataError"></a>[module common-errors.data.DataError](#apidoc.module.common-errors.data.DataError)

#### <a name="apidoc.element.common-errors.data.DataError.DataError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>DataError (message, inner_error)](#apidoc.element.common-errors.data.DataError.DataError)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.DataError('Too many rows returned from database', err);
'''

---------------------------------------

<a name="memcached" />
### MemcachedError
...
```

#### <a name="apidoc.element.common-errors.data.DataError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.DataError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.DataError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.DataError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.DataError.</span>super_ ()](#apidoc.element.common-errors.data.DataError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.DataError.prototype"></a>[module common-errors.data.DataError.prototype](#apidoc.module.common-errors.data.DataError.prototype)

#### <a name="apidoc.element.common-errors.data.DataError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.DataError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.DataError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.MemcachedError"></a>[module common-errors.data.MemcachedError](#apidoc.module.common-errors.data.MemcachedError)

#### <a name="apidoc.element.common-errors.data.MemcachedError.MemcachedError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>MemcachedError (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError.MemcachedError)
- description and source-code
```javascript
function MemcachedError(message, inner_error){if(!(this instanceof MemcachedError)) {var instance = Object.create(MemcachedError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.MemcachedError('Expected value not found', err);
'''

---------------------------------------

<a name="mongodb" />
### MongoDBError
...
```

#### <a name="apidoc.element.common-errors.data.MemcachedError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.MemcachedError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.MemcachedError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.MemcachedError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.MemcachedError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.MemcachedError.super_)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.MemcachedError.prototype"></a>[module common-errors.data.MemcachedError.prototype](#apidoc.module.common-errors.data.MemcachedError.prototype)

#### <a name="apidoc.element.common-errors.data.MemcachedError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.MemcachedError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.MemcachedError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.MongoDBError"></a>[module common-errors.data.MongoDBError](#apidoc.module.common-errors.data.MongoDBError)

#### <a name="apidoc.element.common-errors.data.MongoDBError.MongoDBError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>MongoDBError (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError.MongoDBError)
- description and source-code
```javascript
function MongoDBError(message, inner_error){if(!(this instanceof MongoDBError)) {var instance = Object.create(MongoDBError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.MongoDBError('Retrieved value not in expected format', err);
'''

---------------------------------------

<a name="redis" />
### RedisError
...
```

#### <a name="apidoc.element.common-errors.data.MongoDBError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.MongoDBError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.MongoDBError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.MongoDBError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.MongoDBError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.MongoDBError.super_)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.MongoDBError.prototype"></a>[module common-errors.data.MongoDBError.prototype](#apidoc.module.common-errors.data.MongoDBError.prototype)

#### <a name="apidoc.element.common-errors.data.MongoDBError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.MongoDBError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.MongoDBError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.RedisError"></a>[module common-errors.data.RedisError](#apidoc.module.common-errors.data.RedisError)

#### <a name="apidoc.element.common-errors.data.RedisError.RedisError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>RedisError (message, inner_error)](#apidoc.element.common-errors.data.RedisError.RedisError)
- description and source-code
```javascript
function RedisError(message, inner_error){if(!(this instanceof RedisError)) {var instance = Object.create(RedisError.prototype);
classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.RedisError('expected value not found in redis', err);
'''

---------------------------------------

<a name="rollback" />
### RollbackError
...
```

#### <a name="apidoc.element.common-errors.data.RedisError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.RedisError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.RedisError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.RedisError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.RedisError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.RedisError.super_)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.RedisError.prototype"></a>[module common-errors.data.RedisError.prototype](#apidoc.module.common-errors.data.RedisError.prototype)

#### <a name="apidoc.element.common-errors.data.RedisError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.RedisError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.RedisError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.RollbackError"></a>[module common-errors.data.RollbackError](#apidoc.module.common-errors.data.RollbackError)

#### <a name="apidoc.element.common-errors.data.RollbackError.RollbackError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>RollbackError (message, inner_error)](#apidoc.element.common-errors.data.RollbackError.RollbackError)
- description and source-code
```javascript
function RollbackError(message, inner_error){if(!(this instanceof RollbackError)) {var instance = Object.create(RollbackError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.RollbackError('database transaction was unexpectedly rolled back', err);
'''

---------------------------------------

<a name="sql" />
### SQLError
...
```

#### <a name="apidoc.element.common-errors.data.RollbackError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.RollbackError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.RollbackError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.RollbackError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.RollbackError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.RollbackError.super_)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.RollbackError.prototype"></a>[module common-errors.data.RollbackError.prototype](#apidoc.module.common-errors.data.RollbackError.prototype)

#### <a name="apidoc.element.common-errors.data.RollbackError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.RollbackError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.RollbackError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.SQLError"></a>[module common-errors.data.SQLError](#apidoc.module.common-errors.data.SQLError)

#### <a name="apidoc.element.common-errors.data.SQLError.SQLError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>SQLError (message, inner_error)](#apidoc.element.common-errors.data.SQLError.SQLError)
- description and source-code
```javascript
function SQLError(message, inner_error){if(!(this instanceof SQLError)) {var instance = Object.create(SQLError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.SQLError('foreign key constraint violated', err);
'''

---------------------------------------

<a name="transaction" />
### TransactionError
...
```

#### <a name="apidoc.element.common-errors.data.SQLError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.SQLError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.SQLError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.SQLError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.SQLError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.SQLError.super_)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.SQLError.prototype"></a>[module common-errors.data.SQLError.prototype](#apidoc.module.common-errors.data.SQLError.prototype)

#### <a name="apidoc.element.common-errors.data.SQLError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.SQLError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.SQLError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.TransactionError"></a>[module common-errors.data.TransactionError](#apidoc.module.common-errors.data.TransactionError)

#### <a name="apidoc.element.common-errors.data.TransactionError.TransactionError"></a>[function <span class="apidocSignatureSpan">common-errors.data.</span>TransactionError (message, inner_error)](#apidoc.element.common-errors.data.TransactionError.TransactionError)
- description and source-code
```javascript
function TransactionError(message, inner_error){if(!(this instanceof TransactionError)) {var instance = Object.create(TransactionError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.data.TransactionError('transaction already complete', err);
'''

---------------------------------------

<a name="error" />
### Error
...
```

#### <a name="apidoc.element.common-errors.data.TransactionError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.data.TransactionError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.data.TransactionError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.data.TransactionError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.data.TransactionError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.data.TransactionError.super_)
- description and source-code
```javascript
function DataError(message, inner_error){if(!(this instanceof DataError)) {var instance = Object.create(DataError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.data.TransactionError.prototype"></a>[module common-errors.data.TransactionError.prototype](#apidoc.module.common-errors.data.TransactionError.prototype)

#### <a name="apidoc.element.common-errors.data.TransactionError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.data.TransactionError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.data.TransactionError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.helpers"></a>[module common-errors.helpers](#apidoc.module.common-errors.helpers)

#### <a name="apidoc.element.common-errors.helpers.generateClass"></a>[function <span class="apidocSignatureSpan">common-errors.helpers.</span>generateClass (name, options)](#apidoc.element.common-errors.helpers.generateClass)
- description and source-code
```javascript
function generateErrorClass(name, options){
  options = options || {};
  if(options.subclass) console.warn("options.subclass is deprecated. use options.extends instead.");
  options.extends = options.extends || options.subclass || Error;
  options.args = options.args || ['message', 'inner_error'];
  options.generateMessage = options.generateMessage || null;
  options.globalize = options.globalize === false ? false : true;

  validateInput(name);
  validateArrayInput(options.args);

  var classConstructor = function classConstructor(){
    Class.super_.call(this);
    if(this.global_initialize) this.global_initialize(Class);

    this.args = arguments;
    for(var i = 0; i<options.args.length; i++){
      this[options.args[i]] = arguments[i];
    }
    this.name = name;
    if(this.generateMessage) this.message = this.generateMessage();
    Class.captureStackTrace(this, Class);
  };

  var classGeneratorFn = new Function('classConstructor', [
    "return function ", name, "(", options.args.join(', '), "){",
      "if(!(this instanceof ", name, ")) {",
        "var instance = Object.create(", name, ".prototype);",
        "classConstructor.apply(instance, arguments);",
        "return instance;",
      "} else {",
        "classConstructor.apply(this, arguments);",
      "}",
    "};",
  ].join(''));
  var Class = classGeneratorFn(classConstructor);

  util.inherits(Class, options.extends);

  Class.prototype.generateMessage = options.generateMessage;

  Class.captureStackTrace = function captureStackTrace(error, error_class){
    Error.captureStackTrace(error, error_class);
    if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
  }

  if(options.globalize) globalize(Class);
  return Class;
}
```
- example usage
```shell
...
'''

<a name="generateClass" />
### generateClass

Simple interface for generating a new Error class type.

	helpers.generateClass(name[, options])

__Arguments__

* 'name' - The full name of the new Error class
* 'options'
* 'extends' - The base class for the new Error class. Default is 'Error'.
* 'globalize' - Boolean (default 'true') to store the Error in global space so that the Error is equivalent to others included from
 other versions of the module.
...
```



# <a name="apidoc.module.common-errors.io"></a>[module common-errors.io](#apidoc.module.common-errors.io)

#### <a name="apidoc.element.common-errors.io.DirectoryNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>DirectoryNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError)
- description and source-code
```javascript
function DirectoryNotFoundError(message, inner_error){if(!(this instanceof DirectoryNotFoundError)) {var instance = Object.create
(DirectoryNotFoundError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.DirectoryNotFoundError("/var/log", err)
'''

---------------------------------------

<a name="drivenotfound" />
### DriveNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.DriveNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>DriveNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError)
- description and source-code
```javascript
function DriveNotFoundError(message, inner_error){if(!(this instanceof DriveNotFoundError)) {var instance = Object.create(DriveNotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.DriveNotFoundError("c", err)
'''

---------------------------------------

<a name="endofstream" />
### EndOfStreamError
...
```

#### <a name="apidoc.element.common-errors.io.EndOfStreamError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>EndOfStreamError (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError)
- description and source-code
```javascript
function EndOfStreamError(message, inner_error){if(!(this instanceof EndOfStreamError)) {var instance = Object.create(EndOfStreamError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.EndOfStreamError("EOS while reading header", err)
'''

---------------------------------------

<a name="fileload" />
### FileLoadError
...
```

#### <a name="apidoc.element.common-errors.io.FileLoadError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>FileLoadError (file_name, inner_error)](#apidoc.element.common-errors.io.FileLoadError)
- description and source-code
```javascript
function FileLoadError(file_name, inner_error){if(!(this instanceof FileLoadError)) {var instance = Object.create(FileLoadError.
prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'file_name' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.FileLoadError("./package.json", err)
'''

---------------------------------------

<a name="filenotfound" />
### FileNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.FileNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>FileNotFoundError (file_name, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError)
- description and source-code
```javascript
function FileNotFoundError(file_name, inner_error){if(!(this instanceof FileNotFoundError)) {var instance = Object.create(FileNotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'file_name' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.FileNotFoundError("./package.json", err)
'''

---------------------------------------

<a name="socket" />
### SocketError
...
```

#### <a name="apidoc.element.common-errors.io.IOError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>IOError (message, inner_error)](#apidoc.element.common-errors.io.IOError)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.IOError("Could not open file", err)
'''

---------------------------------------

<a name="directorynotfound" />
### DirectoryNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.SocketError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>SocketError (message, inner_error)](#apidoc.element.common-errors.io.SocketError)
- description and source-code
```javascript
function SocketError(message, inner_error){if(!(this instanceof SocketError)) {var instance = Object.create(SocketError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.SocketError('socket no longer available', err);
'''

---------------------------------------

<a name="notfound" />
### NotFoundError
...
```



# <a name="apidoc.module.common-errors.io.DirectoryNotFoundError"></a>[module common-errors.io.DirectoryNotFoundError](#apidoc.module.common-errors.io.DirectoryNotFoundError)

#### <a name="apidoc.element.common-errors.io.DirectoryNotFoundError.DirectoryNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>DirectoryNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError.DirectoryNotFoundError)
- description and source-code
```javascript
function DirectoryNotFoundError(message, inner_error){if(!(this instanceof DirectoryNotFoundError)) {var instance = Object.create
(DirectoryNotFoundError.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this
, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.DirectoryNotFoundError("/var/log", err)
'''

---------------------------------------

<a name="drivenotfound" />
### DriveNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.DirectoryNotFoundError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.DirectoryNotFoundError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.DirectoryNotFoundError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.DirectoryNotFoundError.super_)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.DirectoryNotFoundError.prototype"></a>[module common-errors.io.DirectoryNotFoundError.prototype](#apidoc.module.common-errors.io.DirectoryNotFoundError.prototype)

#### <a name="apidoc.element.common-errors.io.DirectoryNotFoundError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.DirectoryNotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.DirectoryNotFoundError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.DriveNotFoundError"></a>[module common-errors.io.DriveNotFoundError](#apidoc.module.common-errors.io.DriveNotFoundError)

#### <a name="apidoc.element.common-errors.io.DriveNotFoundError.DriveNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>DriveNotFoundError (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError.DriveNotFoundError)
- description and source-code
```javascript
function DriveNotFoundError(message, inner_error){if(!(this instanceof DriveNotFoundError)) {var instance = Object.create(DriveNotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.DriveNotFoundError("c", err)
'''

---------------------------------------

<a name="endofstream" />
### EndOfStreamError
...
```

#### <a name="apidoc.element.common-errors.io.DriveNotFoundError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.DriveNotFoundError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.DriveNotFoundError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.DriveNotFoundError.super_)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.DriveNotFoundError.prototype"></a>[module common-errors.io.DriveNotFoundError.prototype](#apidoc.module.common-errors.io.DriveNotFoundError.prototype)

#### <a name="apidoc.element.common-errors.io.DriveNotFoundError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.DriveNotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.DriveNotFoundError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.EndOfStreamError"></a>[module common-errors.io.EndOfStreamError](#apidoc.module.common-errors.io.EndOfStreamError)

#### <a name="apidoc.element.common-errors.io.EndOfStreamError.EndOfStreamError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>EndOfStreamError (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError.EndOfStreamError)
- description and source-code
```javascript
function EndOfStreamError(message, inner_error){if(!(this instanceof EndOfStreamError)) {var instance = Object.create(EndOfStreamError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.EndOfStreamError("EOS while reading header", err)
'''

---------------------------------------

<a name="fileload" />
### FileLoadError
...
```

#### <a name="apidoc.element.common-errors.io.EndOfStreamError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.EndOfStreamError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.EndOfStreamError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.EndOfStreamError.super_)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.EndOfStreamError.prototype"></a>[module common-errors.io.EndOfStreamError.prototype](#apidoc.module.common-errors.io.EndOfStreamError.prototype)

#### <a name="apidoc.element.common-errors.io.EndOfStreamError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.EndOfStreamError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.EndOfStreamError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.FileLoadError"></a>[module common-errors.io.FileLoadError](#apidoc.module.common-errors.io.FileLoadError)

#### <a name="apidoc.element.common-errors.io.FileLoadError.FileLoadError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>FileLoadError (file_name, inner_error)](#apidoc.element.common-errors.io.FileLoadError.FileLoadError)
- description and source-code
```javascript
function FileLoadError(file_name, inner_error){if(!(this instanceof FileLoadError)) {var instance = Object.create(FileLoadError.
prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'file_name' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.FileLoadError("./package.json", err)
'''

---------------------------------------

<a name="filenotfound" />
### FileNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.FileLoadError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.FileLoadError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.FileLoadError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.FileLoadError.super_)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.FileLoadError.prototype"></a>[module common-errors.io.FileLoadError.prototype](#apidoc.module.common-errors.io.FileLoadError.prototype)

#### <a name="apidoc.element.common-errors.io.FileLoadError.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.io.FileLoadError.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "Unable to load file: " + this.file_name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.FileLoadError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileLoadError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.FileLoadError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.FileNotFoundError"></a>[module common-errors.io.FileNotFoundError](#apidoc.module.common-errors.io.FileNotFoundError)

#### <a name="apidoc.element.common-errors.io.FileNotFoundError.FileNotFoundError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>FileNotFoundError (file_name, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError.FileNotFoundError)
- description and source-code
```javascript
function FileNotFoundError(file_name, inner_error){if(!(this instanceof FileNotFoundError)) {var instance = Object.create(FileNotFoundError
.prototype);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'file_name' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.FileNotFoundError("./package.json", err)
'''

---------------------------------------

<a name="socket" />
### SocketError
...
```

#### <a name="apidoc.element.common-errors.io.FileNotFoundError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.FileNotFoundError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.FileNotFoundError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.FileNotFoundError.super_)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.FileNotFoundError.prototype"></a>[module common-errors.io.FileNotFoundError.prototype](#apidoc.module.common-errors.io.FileNotFoundError.prototype)

#### <a name="apidoc.element.common-errors.io.FileNotFoundError.prototype.generateMessage"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.prototype.</span>generateMessage ()](#apidoc.element.common-errors.io.FileNotFoundError.prototype.generateMessage)
- description and source-code
```javascript
generateMessage = function (){
  return "File not found: " + this.file_name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.FileNotFoundError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.FileNotFoundError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.FileNotFoundError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.IOError"></a>[module common-errors.io.IOError](#apidoc.module.common-errors.io.IOError)

#### <a name="apidoc.element.common-errors.io.IOError.IOError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>IOError (message, inner_error)](#apidoc.element.common-errors.io.IOError.IOError)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.io.IOError("Could not open file", err)
'''

---------------------------------------

<a name="directorynotfound" />
### DirectoryNotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.IOError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.IOError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.IOError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.IOError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.IOError.</span>super_ ()](#apidoc.element.common-errors.io.IOError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.IOError.prototype"></a>[module common-errors.io.IOError.prototype](#apidoc.module.common-errors.io.IOError.prototype)

#### <a name="apidoc.element.common-errors.io.IOError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.IOError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.IOError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.SocketError"></a>[module common-errors.io.SocketError](#apidoc.module.common-errors.io.SocketError)

#### <a name="apidoc.element.common-errors.io.SocketError.SocketError"></a>[function <span class="apidocSignatureSpan">common-errors.io.</span>SocketError (message, inner_error)](#apidoc.element.common-errors.io.SocketError.SocketError)
- description and source-code
```javascript
function SocketError(message, inner_error){if(!(this instanceof SocketError)) {var instance = Object.create(SocketError.prototype
);classConstructor.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
...
__Arguments__

* 'message' - any message
* 'inner_error' - the Error instance that caused the current error. Stack trace will be appended.

'''js
// Example
throw new errors.SocketError('socket no longer available', err);
'''

---------------------------------------

<a name="notfound" />
### NotFoundError
...
```

#### <a name="apidoc.element.common-errors.io.SocketError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">common-errors.io.SocketError.</span>captureStackTrace (error, error_class)](#apidoc.element.common-errors.io.SocketError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace(error, error_class){
  Error.captureStackTrace(error, error_class);
  if(error.inner_error && error.inner_error.stack) error.stack += "\n--- inner error ---\n" + error.inner_error.stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.common-errors.io.SocketError.super_"></a>[function <span class="apidocSignatureSpan">common-errors.io.SocketError.</span>super_ (message, inner_error)](#apidoc.element.common-errors.io.SocketError.super_)
- description and source-code
```javascript
function IOError(message, inner_error){if(!(this instanceof IOError)) {var instance = Object.create(IOError.prototype);classConstructor
.apply(instance, arguments);return instance;} else {classConstructor.apply(this, arguments);}}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.io.SocketError.prototype"></a>[module common-errors.io.SocketError.prototype](#apidoc.module.common-errors.io.SocketError.prototype)

#### <a name="apidoc.element.common-errors.io.SocketError.prototype.global_initialize"></a>[function <span class="apidocSignatureSpan">common-errors.io.SocketError.prototype.</span>global_initialize (Class)](#apidoc.element.common-errors.io.SocketError.prototype.global_initialize)
- description and source-code
```javascript
function global_initialize(Class){
  var proto_keys = Object.keys(Class.__original_prototype__);
  for(var i = 0; i<proto_keys.length; i++) {
    var proto_key = proto_keys[i];
    this[proto_key] = Class.__original_prototype__[proto_key];
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.common-errors.middleware"></a>[module common-errors.middleware](#apidoc.module.common-errors.middleware)

#### <a name="apidoc.element.common-errors.middleware.crashProtector"></a>[function <span class="apidocSignatureSpan">common-errors.middleware.</span>crashProtector (errorHandler)](#apidoc.element.common-errors.middleware.crashProtector)
- description and source-code
```javascript
crashProtector = function (errorHandler){
  return function crashProtector(req, res, next) {
    var domain = require('domain'); //require only if needed, because "Due to their experimental nature, the Domains features are
 disabled unless the domain module is loaded at least once."
    var d = domain.create();
    d.on('error', function(err){
      console.error("Fatal crash protected!");
      d.dispose();
      if(res.finished || Object.keys(res._headers).length) {
        console.error(err && err.stack);
        return res.end();
      }
      if(errorHandler) errorHandler(err, req, res);
      else next(err);
    });
    d.run(next);
  }
}
```
- example usage
```shell
...

'''js
// Example
var app = express();

app.use(express.static(__dirname + '/../public'));
app.use(express.bodyParser());
app.use(errors.middleware.crashProtector());

//insert new middleware here

app.get('/healthcheck', function (req, res, next){res.send('YESOK')});

app.use(app.router);
app.use(errors.middleware.errorHandler);
...
```

#### <a name="apidoc.element.common-errors.middleware.errorHandler"></a>[function <span class="apidocSignatureSpan">common-errors.middleware.</span>errorHandler (err, req, res, next)](#apidoc.element.common-errors.middleware.errorHandler)
- description and source-code
```javascript
function errorHandler(err, req, res, next){
  if(!err) {
    if(next) return next();
    else return res.end();
  }

  err = new HttpStatusError(err, req);
  if(err.status_code >= 500) {
    console.error(err.stack);
    err.message = HttpStatusError.message_map[500]; //hide the real error from user agent.
  }

  res.status(err.status_code).send(err.message);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
