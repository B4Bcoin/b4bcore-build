# b4bcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install b4bcore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var b4bcoreTasks = require('b4bcore-build');

b4bcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var b4bcoreTasks = require('b4bcore-build');
b4bcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/B4Bcoin/b4bcore) on the main b4bcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/B4Bcoin/b4bcore/blob/master/LICENSE).
