# n8n AI Gaming News Automation

This repository contains an experimental **n8n workflow** built to explore how automation tools can be combined with **Large Language Models (LLMs)** to create an end-to-end AI-powered pipeline.

The workflow automatically scrapes gaming news, uses an AI agent powered by **Google Gemini** to generate an email summary, and sends the result via email on a daily schedule.



## 🧠 Project Goal

The main goal of this project was **learning and experimentation**:
- Understanding how n8n workflows are structured
- Exploring AI Agent nodes and memory in n8n
- Integrating LLMs into automation pipelines
- Automating real-world tasks using triggers, scraping, AI, and email services



## ⚙️ Workflow Overview

The workflow runs **every day at 10:00 AM** and follows these steps:

1. **Schedule Trigger**  
   Automatically starts the workflow daily at a fixed time.

2. **Web Scraping**  
   Scrapes a gaming website to collect the latest news content.

3. **AI Agent (Google Gemini)**  
   The scraped data is passed to a Gemini-powered AI Agent, which:
   - Analyzes the gaming news
   - Generates a clear and readable email-style summary

4. **Email Sending (Gmail)**  
   The generated summary is sent directly to my email inbox.



## 🚀 How to Use This Workflow

1. Open **n8n**
2. Go to **Workflows → Import**
3. Upload the exported workflow JSON file
4. Configure credentials:
   - Google Gemini API
   - Gmail account
5. Activate the workflow


## 🔐 Environment & Credentials

⚠️ **API keys and credentials are not included in this repository.**

You must configure them manually inside n8n:
- Google Gemini credentials
- Gmail credentials


## 📌 Notes

- This project is **not production-focused**
- Built purely for learning and experimentation
- Can be easily extended to:
  - Other news categories
  - Slack / Discord notifications
  - RAG pipelines
  - Multiple LLM providers


## 📚 What I Learned

- Designing end-to-end automation workflows
- Passing real-world data to LLMs
- Using AI Agents and memory inside n8n
- Combining scheduling, scraping, AI reasoning, and messaging


## 🛠️ Tech Stack

- **n8n**
- **Google Gemini**
- **Web Scraping**
- **Gmail API**
- **AI Agents & Memory**


## 📄 License

This project is for educational and experimental purposes.

