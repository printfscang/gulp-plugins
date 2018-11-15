# gulp-plugins
gulp3的一些插件及使用方法
# 将es6语法转化为es5
```
1.安装babel插件
npm install gulp
2.安装es6转es5插件
npm install babel-preset-es2015
3.gulpfile.js的部分配置
gulp.task('change',()=>{
    gulp.src('./es6file.js')
      .pipe(babel())
      .pipe(gulp.dest('dist'))

})
4.在根目录下创建.babelrc文件，并添加相应的配置
{
  "presets":["es2015"]
}
5.运行gulp命令
6. 至此就可以将async await编译为es5了
```
# gulp-

