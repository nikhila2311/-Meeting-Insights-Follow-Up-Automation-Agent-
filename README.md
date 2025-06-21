# 🧠 Meeting Insights & Follow-Up Automation Agent (n8n + Azure OpenAI + Google Calendar)

## 🚀 Overview

This project is an **AI-powered automation agent** designed to streamline team meetings by:

- ✅ Accepting transcripts of virtual meetings via a webhook
- 🧠 Using Azure OpenAI (GPT-4o) to generate a **meeting summary**
- 📋 Extracting **personalized to-do lists** for each participant
- 📅 Automatically scheduling a **Google Calendar event** based on the discussion
- 🔁 Returning the output as a structured JSON response (ideal for APIs or Postman)

---

## ⚙️ Tech Stack

| Tool / Service        | Purpose                               |
|------------------------|----------------------------------------|
| [n8n](https://n8n.io)              | Workflow automation platform           |
| Azure OpenAI (GPT-4o)  | Meeting summarization & task extraction |
| Google Calendar API    | Scheduling follow-up reminders          |
| Postman                | API testing & demo                      |

---

## 📌 Problem Statement

> **Meeting Insights & Follow-Up Automation Agent**  
> Build an AI agent that attends virtual meetings (using transcripts or recordings), generates a summary of key points, creates personalized to-do lists for each participant, and integrates with Google Calendar to set reminders—all automatically.

---

## 🔁 Workflow Architecture
Webhook (Transcript Input)
↓
Azure OpenAI (GPT-4o) via HTTP Request
↓
Set Node (Extract GPT response)
↓
Google Calendar Node (Create event)
↓
Respond to Webhook (Return output to Postman)
