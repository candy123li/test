### gulp-uglify

#### install


```
npm install --save-dev gulp-uglify
```

#### js配置
>书写gulpfile.js


```
var gulp=require('gulp');
var uglify=require('gulp-uglify');
var pump=require('pump');

gulp.task('default',function (cb) {
	pump([
		gulp.src('./lib/*.js'),
		uglify(),
		gulp.dest('./')
		],cb);
});
```
