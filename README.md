# gulp-compare-json

Gulp plugin for [compare-json](https://github.com/nolemmings/compare-json).

```javascript
'use strict';

var gulp = require('gulp');
var jsonCompare = require('./');

gulp.task('default', function () {
  return gulp.src('fixture/*.json', { read: false })
    .pipe(jsonCompare({
      failOnError: true
    }));
});
```
