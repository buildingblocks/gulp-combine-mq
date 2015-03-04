# gulp-combine-mq
[![NPM version][npm-image]][npm-url]

> Combine matching media queries into one media query definition. Useful for CSS generated by preprocessors using nested media queries.

## Usage
First, install `gulp-combine-mq` as a development dependency:

```shell
npm install --save-dev gulp-combine-mq
```

Then, add it to your `gulpfile.js`:

```js
var combineMq = require('gulp-combine-mq');

gulp.task('combineMq', function () {
	return gulp.src('test.css')
	.pipe(combineMq({
		beautify: false
	}))
	.pipe(gulp.dest('tmp'));
});
```

* * *

## Contributing
[![Build Status][travis-image]][travis-url]

To contribute check the [GitHub issues](https://github.com/buildingblocks/gulp-combine-mq/issues) then work away!

In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality.

* Install [editorconfig-sublime](https://github.com/sindresorhus/editorconfig-sublime) for Sublime Text to help with consistent code formatting.
* Commit messages loosely adhere to [these guidelines](https://github.com/angular/angular.js/blob/master/CONTRIBUTING.md#commit).
* Versioning adheres to [Semver](http://semver.org).

* * *

## Release History
* 04-03-15 - v0.4.0 - Make beautify optional from Node task.
* 30-12-14 - v0.3.1 - Default beautify to `true` in gulp task configuration.
* 21-12-14 - v0.3.0 - Update to [node-combine-mq](https://github.com/frontendfriends/node-combine-mq) v0.7.0 to fix output beautification issues.
* 20-12-14 - v0.2.0 - Update to [node-combine-mq](https://github.com/frontendfriends/node-combine-mq) v0.4.0 to fix font-face issues.
* 29-09-14 - v0.1.1 - Add dependencies.
* 29-09-14 - v0.1.0 - Initial release.

## License
[MIT License](http://building-blocks.mit-license.org)


[npm-image]: https://badge.fury.io/js/gulp-combine-mq.svg
[npm-url]: https://npmjs.org/package/gulp-combine-mq
[travis-image]: https://travis-ci.org/frontendfriends/gulp-combine-mq.svg
[travis-url]: https://travis-ci.org/frontendfriends/gulp-combine-mq
