# 巴哈姆特動畫瘋 下載器

## 簡介

個人學習目的試著以 Node.js 撰寫一支 CLI 工具，將巴哈姆特動畫瘋的影音串流下載成完整檔案。

## 技術背景

> 技術關鍵字：Node.js、M3U8

透過觀察網頁操作流程可以發現，可以分為登入與播放串流影音兩個部分，前者因有 Google reCaptcha 機制，
所以無法直接使用，又發現 APP 版本的登入未使用 reCaptcha，且 session 可與網頁版共用，
故透過逆向工程將 APP 版本的登入機制以 Node.js 重現。

而影音串流的部份，因動畫瘋有播放前廣告的機制，觀察後發現需要取得 token、解鎖廣告，就可以取得 m3u8 清單，
再從中取得影像串流片段，並將片段影像資料流（Stream）pipe 到新檔案中。