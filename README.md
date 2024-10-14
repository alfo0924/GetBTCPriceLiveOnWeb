## 作品說明頁分析

### 架設CPI網站流程

1. 使用Jina AI進行網站分析[1]
   - 選擇Reader功能
   - 輸入要分析的網站
   - 點擊"Fetch Content"抓取網站資料
   - 詢問AI關於網站如何抓取/使用API並生成HTML

2. 環境設置[1]
   - 在IDE中建置Express.js環境，設置ViewEngine參數為none
   - 安裝SQLite數據庫套件：`npm install sqlite3 --save`
   - 確認package.json中dependencies包含 `"sqlite3": "^5.1.7"`

3. 數據處理[1]
   - 從數據來源網站下載數據文件
   - 使用在線SQLite數據庫工具導入數據
   - 選擇適當的欄位名稱，確認新增的BTC/USD表格
   - 查看編輯語法記錄和SQL語法
   - 保存數據庫文件到本地計算機的"db"文件夾

4. 代碼開發[1]
   - 複製數據庫SQL語法
   - 詢問AI如何串接HTML、app.js和JSON
   - 提供專案路徑、後端代碼、前端代碼和SQL語法給AI以獲得更好的理解和建議

5. 文件結構調整[1]
   - 將index.html從public文件夾移出，以便GitHub能夠正確識別

6. 部署準備[1]
   - 確認本地端可以正確抓取數據庫數據
   - 將文件推送更新到GitHub

7. Render部署[1]
   - 在Render註冊帳號
   - 創建新的Web Service
   - 連接到GitHub Repository
   - 選擇要部署的專案Repository
   - 完成部署後，查看狀態列和專案部署網址

## 作品頁面分析

### 功能概述

作品頁面是一個用於顯示Bitcoin/USD價格數據的網站。

### 主要功能

1. 數據查詢
   - 提供開始日期和結束日期的選擇
   - 包含搜索按鈕以執行查詢

2. 導航菜單[4]
   - 概要（BTC/USD）
   - 新聞（BTC/USD NEWS）
   - 其他（Others）
   - 投資想法（Ideas）
   - 技術分析（Technicals）
   - 市場（Markets）
   - 加密市場（Cryptocurrencies）

3. 外部鏈接[4]
   - 提供作品說明頁的鏈接
   - 提供作品頁面的鏈接

### 技術實現

- 使用Express.js作為後端框架
- 採用SQLite作為數據庫
- 前端使用HTML和JavaScript實現用戶界面和交互

