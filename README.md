1. 方通过webpack搭建vue工程;
2. .vue文件开发模式;
3. vue使用jsx进行开发的方式;
4. vue组件间通信的基本方式;
5. webpack打包优化的基本点


### 通过webpack搭建vue工程

根目录webpack.config.js

```js
const config = {
  entry: path.join(__dirname, 'src/index.js'),
  output: {
    filename: 'bundle.js',
    path: path.join(__dirname, 'dist'),
    module: {
      rules: [
        {
          test: /\.vue$/,
          loader: 'vue-loader'
        }
      ]
    }
  }
}
```
查看更多 [webpack.config.js](https://github.com/manba24/vue-todo/blob/master/webpack.config.js)

