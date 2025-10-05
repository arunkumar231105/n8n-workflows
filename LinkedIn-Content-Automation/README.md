# 🚀 LinkedIn Content Automation

This project is my first **AI Agent built in n8n** — a complete workflow for automating LinkedIn content creation and publishing.  
It demonstrates how **AI + automation** can handle everything from **idea → draft → image → approval → publishing**.

---

## ⚡ How It Works

1. **Trigger**: A Google Sheet stores LinkedIn content topics.  
2. **Check**: Workflow monitors the sheet and checks if a topic is marked as “Pending.”  
3. **Drafting**: My writing style (from Google Docs) is fetched.  
4. **AI Agent**: Gemini 2.5 Flash generates a detailed LinkedIn post draft.  
5. **Formatting**: Custom JavaScript code structures the draft neatly.  
6. **Image Generation**: Gemini 2.0 creates a matching image → auto-uploaded to Google Drive → link added back to sheet.  
7. **Status Update**: Google Sheet updates from **Pending → Done**.  
8. **Approval**: A Discord bot sends an approval request (Approve/Decline).  
9. **Publishing**: If approved, the post is automatically published on LinkedIn.  
10. **Final Update**: Status changes to **Posted**.

---

## ✨ Key Highlights

* End-to-end **AI-powered content automation**.  
* Integrations: **n8n, Google Sheets, Google Docs, Gemini AI, Google Drive, Discord, LinkedIn**.  
* First step towards building **scalable AI Agents + Automation workflows**.

---

## 🛠️ How to Use

1. Add your **LinkedIn post ideas** into the Google Sheet and mark them as **Pending**.  
2. The workflow automatically **drafts a post**, formats it, and **generates an image**.  
3. Get an **approval notification in Discord**.  
4. Once approved, the post is **published directly to LinkedIn**.  
5. Track the status in Google Sheet (**Pending → Done → Posted**).

---

## ⚙️ Deployment Guide

### 🧩 Prerequisites

Before importing the workflow, make sure you have:

- ✅ **n8n** installed (locally or hosted version)
- ✅ **Google Cloud Project** with:
  - Google Sheets API enabled  
  - Google Docs API enabled  
  - Google Drive API enabled  
- ✅ **LinkedIn Developer App** for API access  
- ✅ **Discord Bot Token** with webhook permissions  
- ✅ **Gemini API Key** (for AI content and image generation)

---

### 📦 How to Import Workflows into n8n

1. Open your **n8n dashboard**.  
2. Click on **“Import” → “Import from file”** (top-right corner).  
3. Select the provided **`.json` workflow file** from this repo.  
4. Once imported, review all nodes and ensure the credentials are correctly linked.  
5. Click **“Activate Workflow”** to start automation.

> 💡 Tip: You can also import using **drag and drop** the `.json` file directly into your n8n canvas.

---

### 🔐 Configuring Environment Variables

You’ll need to set up the following environment variables in your **n8n instance** (under `.env` file or via UI → Settings → Environment Variables):

```env
# --- Google APIs ---
GOOGLE_SHEETS_CREDENTIALS=your_google_service_account_credentials
GOOGLE_DRIVE_API_KEY=your_google_drive_api_key

# --- Gemini AI ---
GEMINI_API_KEY=your_gemini_api_key

# --- LinkedIn ---
LINKEDIN_CLIENT_ID=your_linkedin_client_id
LINKEDIN_CLIENT_SECRET=your_linkedin_client_secret
LINKEDIN_ACCESS_TOKEN=your_linkedin_access_token

# --- Discord Bot ---
DISCORD_WEBHOOK_URL=your_discord_webhook_url
DISCORD_BOT_TOKEN=your_discord_bot_token
