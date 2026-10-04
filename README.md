# 🤖 n8n AI Personal Assistant

A personal AI-powered automation assistant built with n8n.

The project started as an experiment to explore how AI and workflow automation can connect different everyday applications through a single interface.

The assistant can be controlled directly through Telegram and uses an AI Agent to determine which connected service should handle the user's request.

## 🚀 Architecture

Telegram → AI Agent → Gmail / Google Calendar / Google Drive

The AI Agent acts as the central decision-making component of the workflow and selects the appropriate tool depending on the user's request.

## ⚙️ Features

### 📧 Gmail
- Search and retrieve emails
- Read individual emails
- Send emails
- Reply to existing email threads

### 📅 Google Calendar
- Retrieve calendar events
- Create new events
- Update existing events
- Delete events

### 📁 Google Drive
- Search for files and folders
- Retrieve files
- Download files for further processing

### 💬 Telegram
- Natural-language interface for interacting with the assistant
- Receive results directly through the Telegram bot
- Human approval step for sensitive actions

## 🧠 AI Agent

The workflow uses an AI Agent to understand natural-language requests and decide which available tool should be used.

Example requests:

> "Do I have any appointments tomorrow?"

> "Find Lebenslauf.pdf in my Google Drive."

> "Show me my recent emails."

> "Create a calendar event tomorrow at 3 PM."

This allows multiple services to be controlled through one conversational interface.

## 🔐 Human-in-the-Loop

Sensitive actions can require explicit user confirmation before execution.

A Human Review step is integrated into the workflow so that selected actions are not executed automatically without approval.

## 🛠️ Technologies

- n8n
- AI Agent / LLM
- Telegram Bot
- Gmail API
- Google Calendar API
- Google Drive API
- OAuth
- Workflow Automation
- API Integration

## 📸 Workflow

The workflow connects Telegram with an AI Agent and several Google services.

<img width="1820" height="876" alt="Screenshot from 2026-10-02 21-52-10" src="https://github.com/user-attachments/assets/9deac268-6e91-4ba0-b54b-a84feefab4b7" />


## 🎯 What I learned

Through this project, I gained practical experience with:

- Workflow automation
- AI agents and tool calling
- API integrations
- OAuth-based services
- Human-in-the-loop workflows
- Connecting multiple applications through a central automation system
- Debugging and testing multi-step workflows

## 🔒 Security

Credentials, API keys, OAuth tokens and other sensitive information are not included in this repository.

This repository is intended to document the architecture and development of the project without exposing private credentials.
