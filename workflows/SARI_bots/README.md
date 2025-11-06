# 🤖 SARI — Sistem Tani Cerdas Indonesia

SARI is an intelligent chatbot built with **n8n**, **Telegram**, **Google Sheets**, and **Gemini AI**, designed to assist farmers and agricultural suppliers in Indonesia.

---

## 🌾 Features

- 💬 Telegram chatbot interface for farmers
- 📊 Integrated with Google Sheets for **real-time stock data**
- 🤖 Powered by **Google Gemini AI** for natural conversation
- 📈 Predicts **market trends and prices**
- 🧑‍🌾 Handles data like:
  - Product ID
  - Fertilizer name
  - Stock (in kilograms)
  - Plant type
  - Agricultural tools
  - Market price (in IDR)
  - Market prediction
  - Main supplier
  - Last update date

---

## ⚙️ Architecture Overview

[User - Telegram]
↓
[Telegram Trigger - n8n]
↓
[AI Agent - Gemini Chat Model]
↓
[Google Sheets Tool - Fetch Agricultural Data]
↓
[Telegram Send Message - Reply to User]


---

## 🚀 Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/sari-chatbot.git
   cd sari-chatbot

2. Create environment file

cp .env.example .env

Fill in all tokens and API keys.

3. Import Workflow into n8n

- Open your n8n dashboard
- Click Import Workflow
- Upload workflows/sari_main_workflow.json

4. Connect Telegram Bot

- Use BotFather (https://t.me/BotFather) to create a bot
- Copy token and paste into n8n credential field

5. Connect Google Sheets

- Create a sheet with columns:
| id_produk | nama_pupuk | stok_kg | nama_tanaman | alat_pertanian | harga_tanaman_rp | prediksi_pasar | pemasok_utama | tanggal_update |
- Link it to the Google Sheets node in n8n.

6. Activate Workflow

- Toggle “Active” to enable 24/7 automation

## 🧠 AI Prompt (System Instruction)

"You are SARI (Indonesian Smart Farming System), an AI assistant for farmers.
Answer politely, concisely, and informatively in Indonesian.
Use data from Google Sheets to answer questions about fertilizer stocks, crop prices, market forecasts, and suppliers.
If the question is not related to agriculture, provide a general, friendly answer."

## 🧭 Future Plans

- Integrate voice input for farmers
- Add image recognition (upload plant photos)
- Build web dashboard for analytics
