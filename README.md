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

## Asset Management
npm install --save-dev style-loader css-loader
<!-- или вместо них может быть mini-css-extract-plugin -->

npm install --save-dev csv-loader xml-loader
<!-- json loader is installed by default (but only for Default Export). Use: import Data from './data.json' -->

npm install --save-dev toml yamljs json5

npm uninstall css-loader csv-loader json5 style-loader toml xml-loader yamljs

## Output Management
npm install --save-dev html-webpack-plugin
<!-- https://github.com/jantimon/html-webpack-plugin -->

## Development
<!-- https://blog.teamtreehouse.com/introduction-source-maps - about Source Maps -->

npm run watch

npm install --save-dev webpack-dev-server

npm start
<!-- https://webpack.js.org/configuration/dev-server/ -->

npm install --save-dev express webpack-dev-middleware

npm run server

## Code Splitting
<!-- preparing - back to the end of first chapter -->
npm uninstall express html-webpack-plugin webpack-dev-middleware webpack-dev-server

npm run build

<!-- optimization.runtimeChunk: 'single' необходим, иначе получим проблемы как тут: 
        https://bundlers.tooling.report/code-splitting/multi-entry/ -->


<!-- Хотя использование нескольких точек входа для одной страницы разрешено в webpack, по возможности этого следует избегать в пользу точки входа с несколькими импортами: entry: { page: ['./analytics', './app'] }. Это приводит к лучшей оптимизации и последовательному порядку выполнения при использовании тегов асинхронных сценариев. -->


