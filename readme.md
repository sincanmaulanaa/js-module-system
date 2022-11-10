# SUMMARY IN WEBPACK CONFIGURATION

## - Webpack installation using npm :

```
npm install webpack webpack-cli --save-dev
```

- `--save-dev` it means we store installed package in `"devDependencies"`

---

<br>

## - `package.json` script configuration :

```javascript
"scripts": {
    "build": "webpack"
  }
```

---

<br>

## - `webpack.config.js` configuration :

```javascript
const path = require("path");

module.exports = {
  mode: "development",
  entry: "./src/index.js",
  output: {
    path: path.resolve(__dirname, "output"),
    filename: "bundle.js",
  },
  watch: true,
  devtool: false,
};
```

<br>

### Key & value description

- `mode: "development"` this means that we are in development mode, generated build files will be readable and cleanfull if we compare with `mode: "production"`
- `entry: "./src/index.js"` is the entry point of the app
- `output` key have two property, `path` and `filename` which is use for specify directory and file name as a result of `npm run build`
- `watch: true` use for watching when files has changed
- `devtool: false` mean for remove eval function from generated file in output
