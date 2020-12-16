# Vue.js Webpack Chrome Extension Template

## 簡介

在開發前端專案時常會需要建置基本的開發環境，如常見的 webpack、eslint 等，再加上框架會更加複雜，所以開發 Vue.js 專案時，可透過 Vue-CLI 工具搭配現成的模板來預建置已經設定好的開發環境與目錄結構，可直接產出開發與正式環境的產品，對前端新手容易上手，讓老手節省時間的好工具。而此專案則是針對 Chrome Extension 來預先配置好的 Vue.js 開發環境，除了能夠快速建置基礎程式碼，還整合專用 Hot-Reload 套件來加快開發流程，且能夠彈性選擇是否支援多語系環境。

## 使用方法

```sh
# 安裝 vue-cli
$ npm install -g vue-cli
# 以此模板來建立新專案
$ vue init ALiangLiang/vue-webpack-chrome-extension-template my-project
# 安裝套件
$ cd my-project
$ npm install # 或 yarn
$ npm run dev # 或 yarn dev
```

## 檔案結構

```
.
├── build                             # core scripts
│   ├── page.ejs                      # html page boilerplate of background, options, etc.
│   ├── tools.js                      # util scripts
│   ├── webpack.base.js               # base webpack configure file
│   ├── webpack.dev.js                # configure file on developing, would merge into base
│   └── webpack.prod.js               # configure file on build, would merge into base
├── plugins                           # special webpack plugins for Chrome extension
│   ├── GenerateLocaleJsonPlugin.js   # Transform locale message."js" to "json"
│   └── GenerateManifestJsonPlugin.js # Transform your manifest."js" to "json"
├── dist                              # your runtime code. generate by program.
├── src                               # your source code
│   ├── _locales                      # Implement internationalization across your whole extension (https://developer.chrome.com/extensions/i18n)
│   ├── background                    # Background work of your extension (https://developer.chrome.com/extensions/background_pages)
│   ├── content                       # Run in the context of web pages (https://developer.chrome.com/extensions/content_scripts)
│   ├── devtools                      # It can add new UI panels and sidebars, interact with the inspected page, get information about network requests, and more. (https://developer.chrome.com/extensions/devtools)
│   ├── ext                           # Shared scripts
│   ├── options                       # To allow users to customize the behavior of your extension, you may wish to provide an options page. (https://developer.chrome.com/extensions/options)
│   ├── popup                         # The page (window) that will be displayed when the icon is clicked
│   ├── tab                           # Your application will work in a separate tab
│   └── manifest.js                   # Descriptions of the application, its rights and possibilities (https://developer.chrome.com/extensions/manifest)
├── static                            # static assets, would copy into dist directly.
│   └── icons                         # icons
├── extension.zip                     # extension package. used to upload to web store.
├── package.json                      # build scripts and dependencies
├── package-lock.json                 # npm lockfile, should be commit into git
└── yarn.lock                         # yarn lockfile, should be commit into git
```

## 未來發展

### 版本更新

這個專案從開發完成至今也已超過三年，至少已落後一個大版本的 Vue.js，相關開發套件可能也更新不少，所以還得花時間重新整理跟上最新版本。
