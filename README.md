# webpack
Дефолтный проект с webpack
 
 
## Заметки
npm install --save-dev webpack
npm install --save-dev webpack-cli
npm search lint
npm fund webpack
<!-- npm webpack run -->
node >> process
<!-- process -->
<!-- process.platform -->
<!-- process.env -->
<!-- process.arch -->
npm install --save lodash
npm run test

// не будет работать:
npm run webpack

// будет:
npx webpack

npx webpack --config webpack.config.js

// А после добавления скрипта build в package.json 

npm run build
<!-- environment options: -->
npm run build -- --color
npm run build -- --no-color
npm run build -- --color --progress

### Asset Management
npm install --save-dev style-loader css-loader
<!-- или вместо них может быть mini-css-extract-plugin -->

npm install --save-dev csv-loader xml-loader
<!-- json loader is installed by default (but only for Default Export). Use: import Data from './data.json' -->

npm install --save-dev toml yamljs json5

npm uninstall css-loader csv-loader json5 style-loader toml xml-loader yamljs