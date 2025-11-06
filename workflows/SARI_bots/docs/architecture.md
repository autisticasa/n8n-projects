# 🏗️ Architecture — SARI Chatbot

## 🔁 Workflow Overview

[User on Telegram]
↓
[Telegram Trigger - Node 1]
↓
[AI Agent (Gemini Chat Model) - Node 2]
↓
[Google Sheets (get_stock_data) - Node 3]
↓
[Telegram Send Message - Node 4]

---

## ⚙️ Core Components

| Component | Purpose | Required Credentials |
|------------|----------|----------------------|
| **Telegram Trigger** | Receive messages from users | Access Token |
| **Gemini Chat Model** | Process natural language and generate replies | API Key |
| **Google Sheets** | Fetch agricultural data (stock, prices, trends) | OAuth Client ID / Secret |
| **Telegram Send Message** | Deliver chatbot responses | Reuses Telegram credentials |

---

## 💡 Integration Flow
1. User sends a question via Telegram.  
2. The **Telegram Trigger** node captures the message.  
3. The **AI Agent (Gemini)** interprets intent.  
4. If data is required, Gemini calls the **Google Sheets tool**.  
5. The **Telegram Send Message** node delivers the final answer.
