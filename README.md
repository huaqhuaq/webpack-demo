# webpack-demo
http-server -c-1 启动后打开dist目录


webpack过程
1. npm init     (得到package.json)

2. npm install --save-dev webpack 安装webpack工具

3. npx webpack   (./node_modules/.bin/webpack)  运行webpack

4. touch webpack.config.js

抄基础demo
```
const path = require('path');

module.exports = {
  entry: './src/index.js',
  output: {
    filename: 'main.js',
    path: path.resolve(__dirname, 'dist')
  }
};
```

5. webpack 版本
npx webpack （由于安装4报错，卸载然后再安装 webpack@3）

npm uninstall webpack@4

npm uninstall -g webpack@4

npm i webpack@3

npm i -g webpack@3


6. 然后 ./node_modules/.bin/webpack


7. 使用babel-loader翻译js

安装各种...

npm install babel-loader

npm install @babel/core

npm install @babel/preset-env

8. 在src目录下建 module-1.js module-2.js app.js

修改 webpack.config.js 翻译路径
```
entry: './src/js/app.js',
output: {
  filename: 'bundle.js',
  path: path.resolve(__dirname, 'dist/js/')
},
```

9. 改css

cp src/index.html dist/index.html

使用sass-loader翻译css

npm install sass-loader node-sass webpack --save-dev

npm install style-loader css-loader


npm i -D postcss-loader

