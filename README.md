# Chen-yen Wu Portfolio

GitHub Pages portfolio for Chen-yen Wu, a Chung Yuan Christian University Information Management student focused on AI automation, LINE Bot workflows, API integration, data processing, system integration, and prototype development.

Live site:
- https://fajfl.github.io/p/

## Positioning

This portfolio presents me as an AI automation and system integration oriented MIS student. The content is intentionally practical and prototype-focused. It does not present me as a senior engineer, AI researcher, or owner of production-ready commercial products.

The project descriptions distinguish between:
- In development / graduation project
- Completed / course project
- Personal practice / prototype
- Internal system setup

## Featured Project

### ECS NEO｜LINE 租屋協商存證與租約草稿生成系統

Status: In Development / Graduation Project  
Code: Private / Not Public  
Demo: Screenshots, workflow diagrams, presentation materials

ECS NEO is my graduation project. It explores how LINE Bot and AI workflows can support rental negotiation records and lease draft generation. The system is planned around a LINE group negotiation flow: a bot records messages and timestamps after joining the group, AI extracts rental conditions from conversation text, and backend validation checks the structured output before rendering a lease draft for both sides to review.

Core workflow:

```text
591 找房
→ LINE 群組協商
→ Bot 保存協商紀錄
→ AI 整理租屋條件
→ 產生租約草稿
→ 雙方確認後自行簽署
```

Current scope:
- In development and planning / implementation stage
- Some proof-of-concept validation has been completed
- Not a launched product, commercial service, legal service, notarization service, or formal e-signature platform

Technical focus:
- LINE Bot / LINE Messaging API
- Webhook and API integration
- AI Agent workflow
- `condition_json` schema-based extraction
- Missing-field checks for rent, deposit, lease term, utilities, repairs, tax reporting, and rental subsidy items
- Schema validation and template rendering to reduce AI hallucination risk

The goal is to generate a lease draft that both sides can review and confirm. AI is treated as a condition extractor, not as a final legal decision maker.

## Other Projects

### n8n 法律資訊 AI Agent

Status: Completed / Course Project  
Code: Private / Not Public  
Demo: Screenshots, n8n workflow screenshots, architecture diagram

A five-person systems analysis course project. I worked on the core workflow and backend integration, using n8n Webhook, AI Agent flow, legal text preprocessing, RAG, and a local Qdrant vector database with about 3,500+ legal chunks. Course result: 100 points.

### TOEIC 題庫 AI 標籤與練習 App

Status: Personal Practice / Prototype  
Code: Private / Prototype Only

A personal technical practice project using Flutter for a cross-platform practice interface and a Python ETL pipeline for cleaning and structuring open TOEIC-style question data. It also experiments with local Gemma / AI model tagging and Google TTS for listening practice. This is not presented as a formal product.

### NBA 卡包購物商城

Status: Completed / Course Project  
Code: Private / Not Public

A five-person course project using Java Servlet, Tomcat, and MySQL to implement basic e-commerce features such as login, cart, and order flow. It is presented as a frontend/backend/database integration practice project.

### 遠端系統環境建置

Status: Internal Setup / Prototype  
Code: Not Applicable

An internal remote access setup for sharing RTX 4050 development and compute resources with the graduation project team. I tested Docker + RustDesk, then moved toward Moonlight / Sunshine + Tailscale under practical constraints.

## Skills Highlighted

AI / Automation:
- n8n Level 2
- AI Agent workflow
- RAG / LLM application concepts
- condition_json / schema-based extraction
- Ollama / local LLM usage

Programming / Data:
- Python
- Java
- JavaScript
- SQL / MySQL
- JSON / API / Webhook
- ETL / data preprocessing

System / Tools:
- Docker
- GitHub
- Qdrant
- Tomcat
- Linux / WSL basics
- Tailscale / RustDesk / Moonlight / Sunshine

## Files

- `index.html`: Main GitHub Pages portfolio page
- `style.css`: Custom layout, cards, labels, and animation styles
- `profile_pic.jpg`: Profile photo
- `ECS_FLOW.jpg`: ECS NEO workflow whiteboard diagram

## Local Preview

Open `index.html` directly in a browser, or serve the folder with any static file server.

Example:

```bash
python -m http.server 8091
```

Then open:

```text
http://127.0.0.1:8091/
```

## Contact

- Email: k9404019487@gmail.com
- Location: 桃園市
- GitHub: https://github.com/fajfl
