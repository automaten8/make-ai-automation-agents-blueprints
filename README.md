# Make AI Automation Agents & Blueprints

This repository contains modular AI-first automation agents and workflow blueprints built in [Make](https://www.make.com). Each folder includes a specific automation use case - ranging from inbound lead handling to outbound prospecting and calendar scheduling.

---

## 🧠 What’s Inside

- ✅ **Autonomous agents** that can qualify leads, book meetings, and respond to emails
- 🔁 **Reusable sub-scenarios** like `get_available_time_slots` and `book_meeting`
- 🧩 **Conditional logic + OpenAI GPT-4** for dynamic and personalized outputs
- 🔗 Integrations with Gmail, Google Calendar, Sheets, Airtable, and external APIs via HTTP

---

## 📂 Folder Structure

Each folder represents a specific automation use case:

- `B2B_AI_Prospecting_Agent/`  
  Automates outbound cold email campaigns using AI, research, and multi-step logic.

- `Inbound_Lead_Response_Agent/`  
  Listens for inbound emails or form fills and responds intelligently to qualify or book meetings.

- `Calendar_Scheduling_Agent/`  
  Fetches availability from Google Calendar and automates meeting booking using webhooks.

- `Agent_Tools/`  
  Standalone Make scenarios used as callable agent tools (e.g. time slot lookup, meeting booking).

---

## 🚀 How to Use

1. Clone or download this repo
2. Go to [Make](https://www.make.com)
3. Create a new scenario and click **Import Blueprint**
4. Paste the contents of the `.json` file from any folder
5. Customize modules for your tools (OpenAI keys, Gmail, Calendly, Airtable, etc.)

---

## 🧩 Requirements

- A Make account
- OpenAI API key (for GPT-powered agents)
- Perplexity API key (for deep research, source data)
- API access to any 3rd-party tools you want to use (e.g. Gmail, CRM, GoogleSheets, RapidAPI, Apify, etc.)

---

## 📣 Contribute

Have a great automation or sub-agent to add?  
Fork this repo and open a pull request — new blueprints are welcome.

---

## 💬 Questions or Feedback?

Message [Nate Shelly on LinkedIn](https://www.linkedin.com/in/nate-shelly/) or open an issue in this repo.

---

## ⚖️ License

MIT License — free to use and modify. Attribution appreciated.
