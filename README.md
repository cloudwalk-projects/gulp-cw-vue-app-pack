# gulp-cw-vue-app-pack
Vue 组件打包工具。将单个`.Vue`的组件转成支持 AMD 方式加载的 `.js` 和 `.html` 文件

##使用方式
###安装
>通过npm安装

```
npm install gulp-cw-vue-app-pack --save-dev
```

###使用
>示例代码

```
var cwVueAppPack = require("gulp-cw-vue-app-pack");

gulp.task("default", function(){
	gulp.src("src/**/*.vue")
		.pipe(cwVueAppPack())
		.pipe(gulp.dest("dist/"));
});
```

