# gulp-jade-l10n-extractor

> Extracts l10n strings from jade files to a gettext .pot file


## Install

```
$ npm install --save-dev gulp-jade-l10n-extractor
```


## Usage

```js
var gulp = require('gulp');
var jadeL10nExtractor = require('gulp-jade-l10n-extractor');

gulp.task('default', function () {
  return gulp.src('templates/*.jade')
    .pipe(jadeL10nExtractor({
      filename: 'messages.pot'
    }))
    .pipe(gulp.dest('l10n/templates'));
});
```


## API

### jadeL10nExtractor([options])

### rev.manifest([path], [options])

#### options

##### filename

Type: `string`  

gettext file name



## License

MIT © [Vahe Hovhannisyan](http://vahehovhannisyan.com)