# 🤖 n8n AI Personal Assistant

**A personal AI-powered automation assistant built with n8n.**

The project started as an experiment to explore how AI and workflow automation can connect different everyday applications through a single conversational interface.

The assistant can be controlled directly through **Telegram** and uses an **AI Agent** to understand the user's request and determine which connected service should handle it.

---

## 🚀 Architecture

**Telegram → AI Agent → Gmail / Google Calendar / Google Drive**

The AI Agent acts as the central decision-making component of the workflow and selects the appropriate tool depending on the user's request.

This architecture makes it possible to interact with several services from one natural-language interface instead of managing each application separately.

---

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

---

## 🧠 AI Agent

The workflow uses an AI Agent to understand natural-language requests and decide which available tool should be used.

Example requests:

> "Do I have any appointments tomorrow?"

> "Find Lebenslauf.pdf in my Google Drive."

> "Show me my recent emails."

> "Create a calendar event tomorrow at 3 PM."

This allows multiple services to be controlled through one conversational interface.

---

## 🔐 Human-in-the-Loop

Sensitive actions can require explicit user confirmation before execution.

A Human Review step is integrated into the workflow so that selected actions are not executed automatically without approval.

This adds an additional control layer between the AI Agent and actions that can modify or send information.

---

## 📸 Workflow

The workflow connects Telegram with an AI Agent and several Google services.

<img width="1820" height="876" alt="n8n AI Personal Assistant workflow" src="https://github.com/user-attachments/assets/9deac268-6e91-4ba0-b54b-a84feefab4b7" />

---

## 📥 Workflow File

The n8n workflow used in this project is included in this repository:

[`workflow/n8n-ai-personal-assistant.json`](workflow/n8n-ai-personal-assistant.json)

The JSON file contains the workflow structure and can be imported into another n8n instance.

**Credentials, API keys, OAuth tokens and other private authentication information are not included.**

---

## 🚀 How to Import the Workflow

To test the project on your own n8n instance:

1. Download or clone this repository.
2. Open your n8n instance.
3. Create a new workflow or open the workflow menu.
4. Select the option to import a workflow from a file.
5. Import:

   `workflow/n8n-ai-personal-assistant.json`

6. Configure your own credentials for the required services.
7. Review the workflow configuration before activating it.

---

## 🔑 Required Connections

After importing the workflow, you will need to configure your own connections for:

- Telegram Bot
- Gmail / Google account
- Google Calendar
- Google Drive
- AI model / LLM used by the AI Agent

Authentication and credentials are intentionally not distributed with the workflow.

---

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
- Human-in-the-Loop

---

## 🎯 What I Learned

Through this project, I gained practical experience with:

- Workflow automation
- AI agents and tool calling
- API integrations
- OAuth-based services
- Human-in-the-loop workflows
- Connecting multiple applications through a central automation system
- Debugging and testing multi-step workflows
- Designing workflows that combine AI reasoning with external tools
- Managing credentials separately from reusable workflow logic

---

## 🔒 Security

Credentials, API keys, OAuth tokens and other sensitive information are **not included in this repository**.

Anyone importing the workflow must configure their own credentials.

The repository is intended to document the architecture, implementation and development of the project while keeping private authentication information protected.

Before publishing an exported workflow, it should always be reviewed to ensure that no sensitive information has accidentally been included.

---

## 📌 Project Purpose

This project was developed as a practical exploration of **AI-powered workflow automation**.

The objective was not only to automate individual tasks, but to understand how an AI Agent can act as a central interface between a user and multiple external services.

The project demonstrates concepts such as:

**AI Agents · APIs · OAuth · Tool Calling · Workflow Automation · Human Approval · Multi-Service Integration**

---

## 👨‍💻 Author

**Elson Tetchoka Sopgo**

Computer Science Student  
Interested in Software Development, AI Automation and API Integration
