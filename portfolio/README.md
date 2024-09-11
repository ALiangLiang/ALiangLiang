# 作品集

這裡陳列了**劉威良 Wei-Liang Liou**（a.k.a **ALiangLiang**）過去到現在較為有成果的創業與業餘專案。

<h2 style="text-align: center;"><a href="goorder.md">Goorder</a></h2>

此專案是我個人於研究所期間發展的一個創業項目，想要為中小型餐飲業者解決建置「更容易為消費者使用」的線上訂餐平台，藉由聊天機器人避免使用者額外安裝 APP 與申請帳號，相比傳統 APP 與網頁服務，可以大幅增加使用者的使用意願與留存率。

> 技術關鍵字：Node.js、Express.js、Vue.js、Chatbot（Messenger／LINE）、MySQL、Redis、RabbitMQ、CI/CD、Gitlab、GCP、GKE（K8S）、Helm Chart

## [DineOneOne](https://www.dineoneone.com.tw/)

在 DineOneOne inc. 擔任全端工程師時，與其他兩位工程師與設計師共同開發的美食社群平台，透過此平台可以讓使用者分享、收藏、評論美食，並且透過搜尋功能找到附近的美食店家。
技術上考量快速開發、低成本，採用 Firebase 為基礎設施，並且使用 Vue.js 搭配 PWA/TWA，快速打造為跨網頁與行動裝置的應用程式，後端則使用 Python in Firebase Cloud Functions 來處理商業邏輯。

> 技術關鍵字：Vue.js、Python、Firebase、PWA、TWA

## Grab & Go

在 DineOneOne inc. 後期開發的另一套低成本點餐機系統，藉由數台 Android 平板電腦作為櫃台端、點餐機，也開發了店家專用控制台網頁，採用 Firebase 作為基礎設施，並且使用 React.js 搭配 PWA/TWA，快速打造基於網頁技術的廚房端行動應用程式。
廚房端 Web APP 也在無採用函式庫與 SDK 的情況下，使用 WebUSB API 成功利用 USB 熱感應印表機印出訂單，無須花費大量成本與風險開發原生 APP。

> 技術關鍵字：React.js、Firebase、PWA、TWA、WebUSB API

## [Counter for Messenger](counter-for-messenger.md) [![GitHub Repo stars](https://img.shields.io/github/stars/ALiangLiang/counter-for-messenger?style=social)](https://GitHub.com/ALiangLiang/counter-for-messenger/stargazers/)

這是大學時開發的 Chrome Extension，能夠收集使用者所有過往的 Messenger 訊息，加以統計並以圖表呈現。發布至今已累積 241360 次安裝，與 75516 最高單周使用次數。

> 技術關鍵字：Chrome Extension、JavaScript、Vue.js、Chart.js、IndexedDB、CSS、ElementUI、Webpack

## [Talkany Messenger 匿名聊天平台](talkany.md) (Doc WIP)

Messenger Platform 剛開放使用時的一支聊天機器人創作，使用該平台來實作出匿名聊天功能，讓使用者能達成匿名配對與通訊，透過此機器人中介聊天圖文，相比傳統無會員制網頁競品，能讓使用者保存設定，並以此開發延伸功能，增加匿名聊天樂趣。

> 技術關鍵字：Chatbot（Messenger）、Node.js、Express.js、Sequelize.js

## [交大資工系計中 門禁系統](cscc-door-secruity-system.md) (Doc WIP)

於交大就讀研究所時期，於服務單位研發的門禁系統，整合既有的硬體（門禁讀卡機）與軟體（帳號系統、空間預約系統等），自行開發數款門禁讀卡機的共用 Python API。並且開發一套 Dependency Injection 與分層式架構的應用程式導向框架來提升程式碼品質，降低維護成本。

> 技術關鍵字：Python3、SQLAlchemy、Dependency Injection

## [Vue.js Webpack Chrome Extension Template](vue-webpack-chrome-extension-template.md) [![GitHub Repo stars](https://img.shields.io/github/stars/ALiangLiang/vue-webpack-chrome-extension-template?style=social)](https://GitHub.com/ALiangLiang/vue-webpack-chrome-extension-template/stargazers/)

使用 Vue-CLI 來建立基於 Vue.js 2 的 Chrome Extension 專案模板，已經包好 Webpack 與 Hot-reload 開發環境，可以讓開發者可以快速建立他們多語系的 Chrome Extension。

> 技術關鍵字：Chrome Extension、Vue.js、Webpack

## [巴哈姆特動畫瘋 下載器](baha-anime-downloader.md) [![GitHub Repo stars](https://img.shields.io/github/stars/ALiangLiang/baha-anime-downloader?style=social)](https://GitHub.com/ALiangLiang/baha-anime-downloader/stargazers/)

基於學習目的，嘗試開發一套巴哈姆特動畫瘋的影音串流下載，以 Node.js 來開發的 CLI 工具。

> 技術關鍵字：Node.js、M3U8

## [(非官方) PChome API](pchome-api.md) (Doc WIP)

此專案包裝 PChome 購物平台 HTTP API 成 Python 與 Node.js 版本 API，透過它可以做到程式化加入購物車至送出訂單的完整流程。

### Node.js 版 [![GitHub Repo stars](https://img.shields.io/github/stars/ALiangLiang/pchome-api?style=social)](https://GitHub.com/ALiangLiang/pchome-api/stargazers/)

此為開源專案，藉由簡單的逆向工程，從混淆的程式碼取出相關部分，搭配實際探測出的 HTTP 請求，製作成 Node.js 的 API 套件。

> 技術關鍵字：Node.js、Crypto.js

### Python 版

此專案為 Python 撰寫的版本，功能與 Node.js 一致，但為外包專案故未開源。在開發上需整個移植 Node.js 程式碼，並需要完整移植加密訂單資料所需的加密方式。

> 技術關鍵字：Python3、PyCryptodome

## 還有很多專案可以直接參考[我的 Github](https://github.com/ALiangLiang?tab=repositories)
