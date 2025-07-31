# 💡 Make AI Automation Agents & Blueprints

This repository contains modular **AI-first automation agents** and **workflow blueprints** built in [Make](https://www.make.com). Each folder includes a specific automation use case — ranging from **inbound lead handling** to **outbound prospecting**, **calendar scheduling**, and **onboarding-to-GPT sync** workflows.

---

## 🧠 What’s Inside

- ✅ **Autonomous agents** that can qualify leads, book meetings, and respond to emails  
- 🔁 **Reusable sub-scenarios** like `get_available_time_slots` and `book_meeting`  
- 🧩 **Conditional logic + OpenAI GPT-4** for dynamic and personalized outputs  
- 🔗 **Integrations** with Gmail, Google Calendar, Sheets, Airtable, and external APIs via HTTP  

---

## 📂 Folder Structure

Each folder represents a specific automation use case. Inside each folder are one or more `.json` blueprints, along with readme notes or reusable sub-scenarios.

### `B2B_AI_Prospecting_Agent/`  
Automates outbound cold email campaigns using AI, research, and multi-step logic.

**Includes:**
- `Engagement_1_Generation.json` — Generates personalized cold emails based on persona, product, and research  
- `Engagement_2_ResponseHandler.json` — Detects replies and responds contextually to schedule or classify  
- `Engagement_3_RoutingLogic.json` — Routes replies to appropriate next steps or agents based on intent and metadata  

---

### `Inbound_Lead_Response_Agent/`  
Listens for inbound emails or form fills and responds intelligently to qualify or book meetings.

**Includes:**
- `Inbound_Email_Listener.json` — Detects form submissions or CRM triggers and initiates response  
- `Qualification_Sequence.json` — Uses GPT logic to ask follow-up questions and collect data  
- `Meeting_Booking_Sequence.json` — Books meetings dynamically based on availability and interest level  

---

### `Calendar_Scheduling_Agent/`  
Fetches availability from Google Calendar and automates meeting booking using webhooks or embed links.

**Includes:**
- `get_available_time_slots.json` — Fetches open time slots from Google Calendar  
- `book_meeting_with_availability.json` — Creates calendar invite using selected time slot  
- `send_calendar_link.json` — Sends scheduling link or embed code via Gmail or chatbot  

---

### `Agent_Tools/`  
Standalone Make scenarios used as callable sub-agents or utilities in other flows.

**Includes:**
- `format_dates_to_ISO.json` — Normalizes date inputs for API calls  
- `enrich_domain_data.json` — Enriches contact info using Clearbit or alternative APIs  
- `slack_notify.json` — Sends Slack notifications with conditional formatting  
- `lookup_knowledge_base.json` — Queries GPT or vector DB to retrieve structured answers  

---

### `Employee_Onboarding_Knowledge_Sync/`  
Modular onboarding flow that begins with form intake and ends with meeting transcription + knowledge sync.

#### `Part_1_Form_to_Meeting/`  
Automates the setup process after a new hire form is submitted.

**Includes:**
- `new_hire_intake_to_calendar.json` —  
  Creates Airtable record, generates onboarding folder, assigns tasks, creates meeting invite, and alerts team via Slack  

#### `Part_2_Post_Meeting_Sync/`  
Handles actions after the onboarding meeting is completed.

**Includes:**
- `onboarding_meeting_to_knowledgebase.json` —  
  Detects completed meeting, downloads recording, transcribes & summarizes via GPT, and syncs summary into Airtable or knowledge base  

---

## 🚀 How to Use

1. **Clone or download this repo**  
2. Go to [Make](https://www.make.com)  
3. Create a new scenario and click **Import Blueprint**  
4. Paste the contents of the `.json` file from any folder  
5. Customize modules for your tools (OpenAI keys, Gmail, Calendly, Airtable, etc.)

---

## 🧩 Requirements

- ✅ A Make account  
- 🔐 OpenAI API key (for GPT-powered agents)  
- 🔍 Perplexity API key (for deep research, source data)  
- 📡 API access to any 3rd-party tools (e.g. Gmail, CRM, Google Sheets, RapidAPI, Apify, etc.)

---

## 📣 Contribute

Have a great automation or sub-agent to add?  
**Fork this repo** and open a pull request — new blueprints are welcome!

---

## 💬 Questions or Feedback?

Message [**Nate Shelly** on LinkedIn](https://www.linkedin.com/in/nate-shelly/)  
or open an issue in this repo.

---

## ⚖️ License

**MIT License** — free to use and modify. Attribution appreciated.
