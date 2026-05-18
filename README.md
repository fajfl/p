# Chen-yen Wu Portfolio

這是我的 GitHub Pages 個人履歷與 portfolio。我的定位是「AI 自動化與系統整合導向的資管系學生」，目前主要關注 AI workflow、LINE Bot、API 串接、資料處理、系統整合與 prototype 開發。

網站連結：
- https://fajfl.github.io/resume/

## 我的方向

我是中原大學資訊管理系學生，方向偏 AI 應用、自動化流程、系統整合、LINE Bot、API 串接、資料處理、AI Agent 與 prototype 開發。

我不是把自己包裝成資深工程師或 AI 研究員，而是希望呈現成能用 AI、LINE Bot、n8n、API、資料處理與 workflow 工具，快速做出可展示系統原型的人。專案描述中我會明確區分「開發中」「已完成」「原型嘗試」與「技術練習」，避免讓人誤以為所有專案都已正式上線或商業化。

## 主打專案

### ECS NEO｜LINE 租屋協商存證與租約草稿生成系統

Status: In Development / Graduation Project  
Code: Private / Not Public  
Demo: Screenshots, workflow diagrams, presentation materials

ECS NEO 是我的畢業專題，主題聚焦於 LINE 租屋協商存證與租約草稿生成。我們希望把房東與房客在 LINE 群組中的協商紀錄保存下來，再透過 AI 從對話中整理租金、押金、租期、水電、設備、修繕責任等租屋條件，最後產生可供雙方確認的租約草稿。

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

我在這個專題中參與：
- 系統架構規劃與畢業專題方向收斂
- LINE Bot 作為租屋協商入口的流程設計
- AI 條件抽取流程設計，將 LINE 對話整理為結構化 `condition_json`
- condition_json schema、缺漏欄位檢查與租約草稿生成流程討論
- 降低 AI 幻覺風險的流程設計，例如讓 AI 只負責條件抽取，再由後端進行 Schema Validation 與模板渲染
- 專題文件、系統流程與展示情境整理

技術重點：
- LINE Bot / LINE Messaging API
- Webhook 與 API Integration
- AI Agent workflow
- `condition_json` schema-based extraction
- 租金、押金、租期、水電、修繕、報稅、租補等缺漏欄位檢查
- Schema Validation 與模板渲染，用來降低 AI 幻覺風險

這個專題的目標是產出可供房東與房客確認的租約草稿。AI 在系統中被限制為「條件抽取器」，不是最終法律判斷者，也不取代律師、公證人或正式電子簽章平台。

## 其他專案

### n8n 法律資訊 AI Agent

Status: Completed / Course Project  
Code: Public Repository  
GitHub: https://github.com/fajfl/law-agent-by-n8n  
Demo: Screenshots, n8n workflow screenshots, architecture diagram

這是系統分析課程的五人期末專題，也作為我的履歷作品集專案之一。專案使用 n8n Workflow + RAG 建立法律資訊問答 prototype，前端聊天介面透過 Webhook 串接 n8n，n8n workflow 中包含 AI Agent、Memory Buffer、Qdrant Vector Store 與 Ollama Embedding，並使用 docker-compose 啟動 n8n、Ollama、Qdrant 等服務。

我主要負責後端資料流、n8n workflow、RAG 流程、前後端串接與部署流程整合。這個專案讓我更理解 RAG prototype 不只是接上模型，還需要處理資料品質、查詢流程、向量資料庫、workflow 編排與回覆邊界。課程成果為 100 分。

### TOEIC 題庫 AI 標籤與練習 App

Status: Personal Practice / Prototype  
Code: Public Prototype  
GitHub: https://github.com/fajfl/toeic_for_pratice

這是我的個人技術練習作品，定位為 Flutter + AI ETL 的 TOEIC 學習 App prototype。目前可執行平台包含 Chrome 與 Android，模組包含 Listening / Vocabulary / Quiz / Diagnostic。

我使用 Python ETL pipeline 清洗與結構化開源題庫，並嘗試用本地 Ollama + Gemma 進行資料清洗、標籤、題目生成與 difficulty / cloze target 補充。ETL 流程支援快取、續跑與增量處理，目標是降低重跑成本。

這個專案主要是為了練習 AI tag、ETL、題庫資料處理與跨平台練習介面，不會把它描述成正式產品。

### NBA 卡包購物商城

Status: Completed / Course Project  
Code: Private / Not Public

這是課程五人專案，使用 Java Servlet、Tomcat、MySQL 建立基本電商網站功能，包含登入、購物車與訂單流程。這個專案對我來說是前後端與資料庫整合的基礎練習。

### 遠端系統環境建置

Status: Internal Setup / Prototype  
Code: Not Applicable

我曾為畢業專題組建置共用 RTX 4050 遠端開發與運算資源。過程中嘗試 Docker + RustDesk，後續改為 Moonlight / Sunshine + Tailscale 等方案，在限制條件下多次調整，最後完成可供團隊使用的遠端環境。

這段經驗讓我更熟悉系統整合、遠端存取工具與在限制條件下替換方案的過程。

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

