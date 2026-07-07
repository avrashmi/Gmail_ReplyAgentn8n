# 🤖 Gmail AI Reply Agent

An AI-powered email automation workflow built using **n8n**, **OpenAI**, **calendar API** and the **Gmail API**.

This workflow automatically monitors incoming Gmail messages, classifies emails using an LLM, assigns Gmail labels, and generates professional HTML email drafts without manual intervention.

---

## 🚀 Features

- 📧 Detects new Gmail messages automatically
- 🤖 Uses OpenAI for intelligent email understanding
- 🏷️ Classifies emails into predefined categories
    - Course
    - Doubts
    - Sponsorship
- 📂 Automatically assigns Gmail labels
- ✉️ Generates professional HTML email drafts
- 🧠 Uses Structured Output Parser for reliable AI responses
- 🔄 End-to-end automation using n8n
- Linked with google calender

---

## 🏗 Architecture

Incoming Email

↓

Gmail Trigger

↓

Fetch Email

↓

OpenAI AI Agent

↓

Label Classification

↓

Apply Gmail Label

↓

Generate HTML Draft

↓

Save Draft in Gmail

---

## Tech Stack

- n8n
- OpenAI GPT-4.1 Mini
- Gmail API
- Google Calendar
- Gmail OAuth2
- Structured Output Parser

---

## Workflow

1. Gmail Trigger polls inbox every minute.

2. Retrieves full email details.

3. AI Agent analyses:

- Subject
- Email Body

4. Determines:

- Email Category
- Gmail Label
- Draft Subject
- HTML Draft Response
- Schedule on calendar

5. Applies the Gmail label.

6. Creates a professional draft inside Gmail.

---

## AI Capabilities

The AI agent can

- Understand email intent
- Categorize emails
- Explain technical questions
- Generate respectful responses
- Produce HTML formatted emails
- Return structured JSON outputs

---

## Required Credentials

| Credential | Purpose |
|------------|----------|
| Gmail OAuth2 | Read and write Gmail |
| OpenAI API | AI reasoning |
Calendar
---

## Future Improvements

- Vector database memory
- Slack notifications
- Confidence scoring
- LangSmith evaluation
- Observability dashboard
- Multi-agent routing
- Auto reply scheduling

---

## Repository Structure

```
gmail-ai-reply-agent
│
├── workflow/
├── gmail_ai_reply.json
└── README.md
```

---
