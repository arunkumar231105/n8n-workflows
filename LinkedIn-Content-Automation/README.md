LinkedIn Content Automation 🚀
This project is my first AI Agent built in **n8n** — a complete workflow for automating LinkedIn content creation and publishing.
It demonstrates how AI + automation can handle everything from **idea → draft → image → approval → publishing**.

⚡ **How It Works**

* **Trigger**: A Google Sheet stores LinkedIn content topics.
* **Check**: Workflow monitors sheet and checks if a topic is marked as “Pending.”
* **Drafting**: My writing style (from Google Docs) is fetched.
* **AI Agent**: Gemini 2.5 Flash generates a detailed LinkedIn post draft.
* **Formatting**: Custom JavaScript code structures the draft neatly.
* **Image Generation**: Gemini 2.0 creates a matching image → auto-uploaded to Google Drive → link added back to sheet.
* **Status Update**: Google Sheet updates from Pending → Done.
* **Approval**: A Discord bot sends an approval request (Approve/Decline).
* **Publishing**: If approved, the post is automatically published on LinkedIn.
* **Final Update**: Status changes to Posted.

✨ **Key Highlights**

* End-to-end AI-powered content automation.
* Integrations: **n8n, Google Sheets, Google Docs, Gemini AI, Google Drive, Discord, LinkedIn**.
* First step towards building scalable AI Agents + Automation workflows.

🛠️ **How to Use**

1. Add your LinkedIn post ideas into the Google Sheet and mark them as **Pending**.
2. The workflow automatically drafts a post, formats it, and generates an image.
3. Get an approval notification in Discord.
4. Once approved, the post is published directly to LinkedIn.
5. Track the status in Google Sheet (Pending → Done → Posted).

💡 This was my first AI-powered content workflow in **n8n**.
I’m excited to keep experimenting and building more **AI + Automation agents** in the future! 🚀
