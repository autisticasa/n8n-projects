# 🚀 Setup Guide — SARI Chatbot

This guide explains how to deploy and run **SARI (Smart Agriculture System Indonesia)** — an AI-powered chatbot built using **n8n**, **Telegram**, **Google Sheets**, and **Google Gemini**.

---

## 1️⃣ Requirements

- **n8n** — Automation workflow platform  
- **Telegram Bot** — Chat interface  
- **Google Sheets** — Dynamic agricultural data storage  
- **Google Gemini** — Natural language understanding  
- **VPS / Hostinger** — To host n8n 24/7

---

## 2️⃣ Quick Setup Steps

### 1. Deploy n8n on VPS
- Log in to your VPS dashboard (e.g., Hostinger).  
- Choose the **n8n template** and deploy.  
- Access your dashboard via: https://your-vps-domain.com

### 2. Import Workflow
- Open `workflows/sari_main_workflow.json`  
- Click **Import Workflow** in the n8n dashboard  

### 3. Set Up Telegram Bot
- Create a new bot via [BotFather](https://t.me/BotFather)  
- Get your **Access Token**  
- Paste it into the “Telegram Trigger” credentials in n8n  

### 4. Connect Gemini AI
- Create an API key at [Google AI Studio](https://aistudio.google.com)  
- Add it to the “Gemini Chat Model” node in n8n  

### 5. Connect Google Sheets
- Create a sheet following the structure in `docs/schema_sheets.md`  
- Connect your Google account credentials in the “Google Sheets” node  

### 6. Activate the Workflow
- Toggle **“Active”** in the top-left corner of the n8n dashboard  

---

## ✅ Final Test
Send a message to your Telegram bot, for example:  
> Hi SARI, how much NPK fertilizer is in stock today?

SARI will reply based on real-time data from Google Sheets.

