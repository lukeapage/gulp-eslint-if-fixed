# gulp-eslint-if-fixed

A simple plugin to avoid having a isFixed function as in the [gulp-eslint fix example](https://github.com/adametry/gulp-eslint/blob/master/example/fix.js).

## installation

```
npm i gulp-eslint-if-fixed --save-dev
```

## usage
```
var eslint = require('gulp-eslint');
var eslintIfFixed = require('gulp-eslint-if-fixed');

gulp.task('lint-fix', function() {
  return gulp.src('src/*.js')
    .pipe(eslint({fix:true}))
    .pipe(eslint.format())
    .pipe(eslintIfFixed('src'));
});
```
