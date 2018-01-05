# react-like-button

[30分間React入門「いいねボタン」作成チュートリアル](http://c16e.com/1510161700/)

## Babel6対応
```
yarn add babel-loader babel-core babel-preset-es2015 babel-preset-stage-0 --dev
```
```javascript:webpack.config.js
module.exports = {
  entry: __dirname + "/src/main.js",
  output: {
    path: __dirname + "/dist",
    filename: "like-button.js"
  },
  module: {
    loaders: [
      {
        test: /\.js(x?)$/,
        loader: "babel-loader",
        query: {
          presets: ["es2015", "stage-0", "react"]
        }
      }
    ]
  }
};
```
