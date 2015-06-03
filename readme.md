# Jam3 Testing Procedure

## tl;dr

Use [tape](https://www.npmjs.com/) and run tests using [budo](https://www.npmjs.com/package/budo) or [nodemon](https://www.npmjs.com/package/nodemon). Tests should live in `test/index.js` or `test.js`.

## Protocol

All tests at Jam3 must be written using the [tap protocol](http://en.wikipedia.org/wiki/Test_Anything_Protocol). A module like [tape](https://www.npmjs.com/package/tape) should be used to produce `tap` output.

We want to use tap as it's easy to build tools on top of and is a standard in other programming languages.

## File Structure:

A repository must contain either a `test.js` file or a `test` folder which contains a `index.js`.

#### Example: With test.js
```
index.js // main application
package.json // package.json (enough said)
test.js // file which will contain tap producing tests
```


#### Example: With test folder
```
index.js // main application
package.json // package.json (enough said)
test/index.js // file which will contain tap producing tests
```



## Tools Used For Testing:

### [tape](https://www.npmjs.com/package/tape)

Tape is a tap producing test harness. Basically it allows you to write unit tests.

### [budo](https://www.npmjs.com/package/budo)

Livereload browser applications.

### [nodemon](https://www.npmjs.com/package/nodemon)

Livereload commandline applications.