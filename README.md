# Chen-yen Wu Portfolio

這是吳振彥的 GitHub Pages 個人履歷與 portfolio 原始碼。內容定位為「AI 自動化與系統整合導向的資管系學生」，重點放在 AI workflow、LINE Bot、API 串接、資料處理、系統整合與 prototype 開發。

網站連結：
- https://fajfl.github.io/p/

## 內容定位

這份 portfolio 以務實、技術導向的方式呈現個人經歷，不把自己包裝成資深工程師、AI 研究員，或已經完成商業化產品的人。專案描述會明確區分目前狀態，避免讓讀者誤以為所有專案都已正式上線。

專案狀態分為：
- 開發中 / 畢業專題
- 已完成 / 課程專案
- 個人技術練習 / 原型嘗試
- 內部系統環境建置

## 主打專案

### ECS NEO｜LINE 租屋協商存證與租約草稿生成系統

Status: In Development / Graduation Project  
Code: Private / Not Public  
Demo: Screenshots, workflow diagrams, presentation materials

ECS NEO 是我的畢業專題，主題聚焦於 LINE 租屋協商存證與租約草稿生成。此系統規劃以 LINE 群組作為租屋協商場域，由 Bot 保存加入後的訊息與時間戳，再透過 AI 從對話中抽取租屋條件，最後由後端進行結構檢查與模板渲染，產生可供雙方確認的租約草稿。

核心流程：

```text
591 找房
→ LINE 群組協商
→ Bot 保存協商紀錄
→ AI 整理租屋條件
→ 產生租約草稿
→ 雙方確認後自行簽署
```

目前狀態：
- 開發中 / 畢業專題
- 正在規劃與實作中
- 已完成部分 POC 驗證
- 尚未正式上線，亦非商業化產品
- 不定位為法律服務、公證服務或正式電子簽章平台

技術重點：
- LINE Bot / LINE Messaging API
- Webhook 與 API Integration
- AI Agent workflow
- `condition_json` schema-based extraction
- 租金、押金、租期、水電、修繕、報稅、租補等缺漏欄位檢查
- Schema Validation 與模板渲染，用來降低 AI 幻覺風險

此專題的目標是產出可供房東與房客確認的租約草稿。AI 在系統中被限制為「條件抽取器」，不是最終法律判斷者。

## 其他專案

### n8n 法律資訊 AI Agent

Status: Completed / Course Project  
Code: Private / Not Public  
Demo: Screenshots, n8n workflow screenshots, architecture diagram

系統分析課程五人專題。我負責核心系統流程與後端整合，使用 n8n Webhook 串接前端輸入與 AI Agent，結合法律條文資料預處理與 RAG 流程，並使用 Qdrant 本地向量資料庫處理約 3,500+ 法條 chunks。課程成果：100 分。

### TOEIC 題庫 AI 標籤與練習 App

Status: Personal Practice / Prototype  
Code: Private / Prototype Only

個人技術練習作品，嘗試使用 Flutter 建立跨平台練習介面，並以 Python ETL pipeline 清洗與結構化開源 TOEIC 題庫。專案也嘗試使用本地 Gemma / AI 模型進行題目標籤，並整合 Google TTS 模擬聽力練習。此專案定位為 AI tag、ETL 與題庫資料處理練習，不呈現為正式產品。

### NBA 卡包購物商城

Status: Completed / Course Project  
Code: Private / Not Public

課程五人專案，使用 Java Servlet、Tomcat、MySQL 建立基本電商網站功能，包含登入、購物車與訂單流程。此專案作為前後端與資料庫整合基礎練習。

### 遠端系統環境建置

Status: Internal Setup / Prototype  
Code: Not Applicable

為畢業專題組建置共用 RTX 4050 遠端開發與運算資源。過程中嘗試 Docker + RustDesk，後續改為 Moonlight / Sunshine + Tailscale 等方案，在限制條件下多次調整，完成可供團隊使用的遠端環境。

## 技術方向

AI / Automation:
- n8n Level 2
- AI Agent workflow
- RAG / LLM 應用概念
- condition_json / schema-based extraction
- Ollama / local LLM usage

Programming / Data:
- Python
- Java
- JavaScript
- SQL / MySQL
- JSON / API / Webhook
- ETL / 資料預處理

System / Tools:
- Docker
- GitHub
- Qdrant
- Tomcat
- Linux / WSL 基礎
- Tailscale / RustDesk / Moonlight / Sunshine

## 檔案說明

- `index.html`: GitHub Pages portfolio 主頁
- `style.css`: 自訂版面、專案卡片、狀態標籤與動畫樣式
- `profile_pic.jpg`: 個人照片
- `ECS_FLOW.jpg`: ECS NEO 系統流程白板圖

## 本機預覽

可以直接用瀏覽器開啟 `index.html`，也可以用任何靜態檔案伺服器預覽。

範例：

```bash
python -m http.server 8091
```

接著開啟：

```text
http://127.0.0.1:8091/
```

## 聯絡方式

- Email: k9404019487@gmail.com
- Location: 桃園市
- GitHub: https://github.com/fajfl
