# webpack-demo
npm init     (得到package.json)
npm install --save-dev webpack 
npx webpack   (./node_modules/.bin/webpack)
./node_modules/.bin/webpack
touch webpack.config.js

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

touch src/index.js


npx webpack （由于安装4报错，卸载然后再安装 webpack@3）
npm uninstall webpack@4
npm uninstall -g webpack@4
npm i webpack@3
npm i -g webpack@3

然后
npx webpack


使用babel-loader翻译js

npm install babel-loader
npm install @babel/core
npm install @babel/preset-env



cp src/index.html dist/index.html

使用sass-loader翻译css
npm install sass-loader node-sass webpack --save-dev
npm install style-loader css-loader


npm i -D postcss-loader

