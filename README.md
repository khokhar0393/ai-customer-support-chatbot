# 🤖 AI Customer Support Chatbot

An AI-powered customer support chatbot built with **n8n**, **OpenAI**, **Gmail**, **Google Sheets**, and **Webhooks**.

The workflow automatically analyzes customer inquiries, detects customer intent, classifies priority, performs sentiment analysis, generates AI-powered responses, escalates high-priority requests to a human support team, and logs every conversation in Google Sheets.

---

## 🚀 Features

- AI-powered customer inquiry analysis
- Intent detection
- Priority classification
- Sentiment analysis
- Automatic AI response generation
- Human handoff for critical cases
- Gmail notification for high-priority requests
- Google Sheets conversation logging
- Webhook API integration
- Structured JSON output using Output Parser

---

## 🛠 Tech Stack

- n8n
- OpenAI GPT
- Gmail API
- Google Sheets API
- Webhooks
- JSON Output Parser

---

# 📊 Workflow Architecture

![Workflow](images/workflow.png)

---

# 📄 Google Sheets Logging

Every customer conversation is automatically stored inside Google Sheets.

![Google Sheets](images/google-sheet.png)

---

# 📧 Gmail Notification

High-priority customer requests are automatically forwarded to the support team.

![Gmail Notification](images/gmail-notification.png)

---

# ⚙️ Workflow Overview

1. Receive customer request through Webhook
2. Extract customer information
3. Analyze the message using OpenAI
4. Detect:
   - Intent
   - Priority
   - Sentiment
   - Human handoff requirement
5. Merge AI output with original customer data
6. Check whether human escalation is required
7. If High Priority:
   - Send Gmail notification
   - Save conversation to Google Sheets
8. Otherwise:
   - Save conversation directly to Google Sheets
9. Return response via Webhook

---

# 📂 Project Structure

```
.
├── workflow.json
├── README.md
├── LICENSE
└── images
    ├── workflow.png
    ├── google-sheet.png
    └── gmail-notification.png
```

---

# 🚀 Getting Started

1. Import **workflow.json** into n8n.
2. Configure your credentials:
   - OpenAI
   - Gmail
   - Google Sheets
3. Update the Webhook URL.
4. Execute the workflow.

---

# 💡 Use Cases

- AI Customer Support
- Help Desk Automation
- Customer Inquiry Classification
- Email Support Automation
- AI Response Generation
- Customer Ticket Routing

---

# 📜 License

This project is licensed under the MIT License.
