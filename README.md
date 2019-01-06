# ravencore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install ravencore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var ravencoreTasks = require('ravencore-build');

ravencoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var ravencoreTasks = require('ravencore-build');
ravencoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/underdarkskies/ravencore) on the main ravencore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/underdarkskies/ravencore/blob/master/LICENSE).

