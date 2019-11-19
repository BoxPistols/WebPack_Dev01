# Hello WebPack

## Setting


$ npm info webpack

$ npm install webpack@4.41.2

$ npm info webpack-cli

$ npm install -save-dev  webpack-cli@3.3.10

$ npm info live-server

$ npm install --save-dev live-server@1.2.1

$ ./node_modules/.bin/live-server

---

## Run

$ npx live-server


----

$ mkdir dist

$ git mv index.html dist/

$ npm install --save lodash@4.17.15

---

index.js add 
`import _ from 'lodash'`

index.html
- rm cdn lodash
- `<script src="main.js"></script>`

npx webpack
npx live-server

$ touch webpack.config.js
 
```js
const path = require('path')

const outputPath = path.resolve(__dirname, 'dist')
console.log(outputPath)
module.exports = {
    entry: './src/index.js',
    output: {
        filename: 'main.js',
        path: outputPath
    }
}
``` 


$ npx webpack --mode development