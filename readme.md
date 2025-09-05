# AI Secretary Bot Workflow

This repository contains the exported n8n workflow (workflow.json) for the AI Secretary Bot, a Telegram bot designed to help track student conversations and registrations for LUT University.

The bot automatically listens to messages and voice notes from students, extracts structured information such as:
- Name
- Arrival status at LUT
- Tuition fee payment status
- Housing application
- Important notes

…and saves it directly into a Google Sheet for easy tracking. It also replies to the user with a confirmation message, so they know their information has been recorded.

## 🖥️ Demo
<img width="1113" height="395" alt="Image" src="https://github.com/user-attachments/assets/0fd14a9c-546c-4b3a-864b-8e582648640e" />

## 📂 Files
- `workflow.json` → The full n8n workflow export.
- `README.md` → Documentation.

## 🚀 How to Import
1. Open your n8n instance.
2. Go to **Workflows → Import from File**.
3. Select `workflow.json` from this repository.
4. Configure credentials inside n8n:
   - **Telegram API**
   - **OpenAI API**
   - **Google Sheets API**

## ✅ Usage
Once activated:
- Send a message or voice note to your Telegram bot.
- The workflow will:
  - Transcribe audio (if voice).
  - Extract structured info (Name, Coming to LUT, Tuition Fee, Housing, etc.).
  - Save the info into Google Sheets.
  - Reply with a confirmation message on Telegram.

## ⚙️ Requirements
- [n8n](https://n8n.io/) installed and running
- A Telegram bot
- OpenAI API key
- Google Sheets credentials
