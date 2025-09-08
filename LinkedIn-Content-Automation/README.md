# LinkedIn Content Automation 🚀

This project is my **first AI Agent built in n8n** — a complete workflow for automating LinkedIn content creation and publishing.  
It demonstrates how **AI + automation** can handle everything from **idea → draft → image → approval → publishing**.

---

## ⚡ How It Works
1. **Trigger:** A Google Sheet stores LinkedIn content topics.  
2. **Check:** Workflow monitors sheet and checks if a topic is marked as “Pending.”  
3. **Drafting:** My writing style (from Google Docs) is fetched.  
4. **AI Agent:** Gemini 2.5 Flash generates a detailed LinkedIn post draft.  
5. **Formatting:** Custom JavaScript code structures the draft neatly.  
6. **Image Generation:** Gemini 2.0 creates a matching image → auto-uploaded to Google Drive → link added back to sheet.  
7. **Status Update:** Google Sheet updates from `Pending → Done`.  
8. **Approval:** A Discord bot sends an approval request (Approve/Decline).  
9. **Publishing:** If approved, the post is automatically published on LinkedIn.  
10. **Final Update:** Status changes to `Posted`.  

---

## ✨ Key Highlights
- End-to-end **AI-powered content automation**.  
- Integrations: **n8n, Google Sheets, Google Docs, Gemini AI, Google Drive, Discord, LinkedIn**.  
- First step towards building scalable **AI Agents + Automation workflows**.  

---

💡 This was my **first AI-powered content workflow** in n8n.  
I’m excited to keep experimenting and building more **AI + Automation agents** in the future!
