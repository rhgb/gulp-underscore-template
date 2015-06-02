# gulp-underscore-template

## Suggested Usage

```javascript
var gulp = require('gulp');
var concat = require('gulp-concat');
var htmlmin = require('gulp-htmlmin');
var template = require('gulp-underscore-template');
gulp.src('./templates/*.html')
    .pipe(htmlmin({
        collapseWhitespace: true,
        conservativeCollapse: true
    }))
    .pipe(template())
    .pipe(concat('templates.js'))
    .pipe(gulp.dest('./lib/'))
```
