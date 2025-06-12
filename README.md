# AI-Powered-Email-Automation-with-RAG
An intelligent, end-to-end email automation workflow built with **n8n**, **OpenAI**, **DeepSeek**, and **Qdrant**. This system automates email responses by reading, summarizing, classifying, and replying to emails — while pulling accurate company info from vectorized documents stored in Google Drive.

---

## 🚀 Features

- **Email Triggering:** Monitors an inbox via IMAP and triggers on new emails.
- **AI Summarization:** Summarizes incoming emails using DeepSeek (in Italian 🇮🇹).
- **Email Classification:** Categorizes emails (e.g., “Company Info Request”).
- **AI Response Generation:** Drafts responses with OpenAI and reviews them using DeepSeek.
- **HTML Formatting:** Generates professionally formatted replies.
- **Document Embedding:** Converts Google Drive documents into searchable vectors.
- **Vector Database Integration:** Uses Qdrant to fetch relevant company info for replies.
- **Automated Sending:** Replies are automatically sent via SMTP.

---

## 🧰 Tech Stack

- **n8n** – Workflow automation platform
- **OpenAI** – Text generation & embeddings
- **DeepSeek R1** – Summarization and text review
- **Qdrant** – Vector database
- **Google Drive** – Document source
- **IMAP/SMTP** – Email integration

---

## 📂 Project Structure

📁 workflows/
└── email-automation-workflow.json
📁 docs/
└── setup-guide.md
📁 assets/
└── screenshots/
README.md
.env.example

yaml
Copy
Edit

---

## ⚙️ Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/email-ai-automation.git
   cd email-ai-automation
Set Up Environment Variables
Create a .env file based on .env.example and fill in:

IMAP/SMTP credentials

OpenAI API key

DeepSeek API key

Qdrant configuration

Google Drive credentials

Import Workflow into n8n

Launch your n8n instance (self-hosted or cloud)

Import the workflow JSON from /workflows/email-automation-workflow.json

Activate the workflow

Test the Setup

Use the Test Workflow feature in n8n to simulate incoming emails.

Check that the workflow summarizes, classifies, and responds correctly.

✅ Use Cases
Customer support automation

Company info handling

Admin email inbox management

Lead qualification replies

Multilingual business communication

📸 Demo & Screenshots
Screenshots available in /assets/screenshots/

🧠 Skills Demonstrated
Workflow Automation (n8n)

Natural Language Processing (NLP)

Email Integration (IMAP/SMTP)

API Integration (OpenAI, DeepSeek, Qdrant)

Vector Embeddings & Search

Prompt Engineering

No-Code/Low-Code System Design
