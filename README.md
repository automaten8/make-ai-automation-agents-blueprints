# 💡 Make AI Automation Agents & Blueprints

This repository contains a growing library of **modular, AI-first automation agents and scenario blueprints** built in [Make](https://www.make.com). Each folder delivers a complete automation use case — from outbound prospecting and inbound lead response, to calendar scheduling and internal onboarding workflows with AI-assisted documentation.

These scenarios are designed to be cloned, customized, and extended for real-world business applications — enabling you to scale operations, reduce manual workload, and build a lean, high-output system with AI at the core.

---

## 🧠 What’s Inside

- ✅ **Autonomous agents** that qualify leads, schedule meetings, and handle multi-step logic  
- 🔁 **Reusable sub-scenarios** like `get_available_time_slots` and `book_meeting`  
- 🧩 **Conditional logic + OpenAI GPT-4** for personalized messaging and classification  
- 🔗 **Integrations** with Gmail, Google Calendar, Airtable, Sheets, and HTTP APIs  

---

## 📁 Folder Structure

Each folder represents a complete automation use case.  
Inside each is one or more `.json` blueprints, reusable tools, and implementation notes.

---

### `B2B_AI_Prospecting_Agent/`  
Outbound cold email engine that uses AI to research, personalize, respond, and route prospect engagement.

**Includes:**
- `Engagement_1_Generation.json` — Generates personalized cold emails based on persona, product, and web research  
- `Engagement_2_ResponseHandler.json` — Detects replies and responds with intelligent follow-up or booking logic  
- `Engagement_3_RoutingLogic.json` — Routes replies to different flows based on message intent or metadata  

---

### `Inbound_Lead_Response_Agent/`  
Responds to inbound leads (via form fill, email, webhook) to qualify, ask questions, and drive toward meetings.

**Includes:**
- `Inbound_Email_Listener.json` — Triggers automation from form submissions or CRM events  
- `Qualification_Sequence.json` — Uses GPT to ask relevant follow-up questions and collect lead data  
- `Meeting_Booking_Sequence.json` — Schedules meeting dynamically based on intent and availability  

---

### `Calendar_Scheduling_Agent/`  
Handles meeting logistics, availability checks, and scheduling workflows through Google Calendar.

**Includes:**
- `get_available_time_slots.json` — Pulls real-time availability from Google Calendar  
- `book_meeting_with_availability.json` — Books a meeting using chosen time slot  
- `send_calendar_link.json` — Sends dynamic scheduling links via email or chatbot  

---

### `Agent_Tools/`  
Reusable modules that support or extend other agents. Meant to be embedded, cloned, or reused.

**Includes:**
- `format_dates_to_ISO.json` — Converts date strings to ISO for cross-platform compatibility  
- `enrich_domain_data.json` — Enriches lead/company data using APIs like Clearbit  
- `slack_notify.json` — Sends Slack alerts with optional conditional formatting  
- `lookup_knowledge_base.json` — Queries vectorized knowledge base or GPT to fetch structured answers  

---

### `Employee_Onboarding_Knowledge_Sync/`  
Two-part automation that transforms onboarding into a streamlined, AI-assisted process — from intake to knowledge capture.

---

#### 📂 `Part_1_Form_to_Meeting/`  
Automates the post-form intake flow and meeting setup for new hires.

**Includes:**
- `new_hire_intake_to_calendar.json` — Creates Airtable record, assigns checklist, creates folders, schedules intro meeting, and alerts team  

---

#### 📂 `Part_2_Post_Meeting_Sync/`  
Triggers once onboarding meetings conclude to transcribe and sync learnings into your knowledge base.

**Includes:**
- `onboarding_meeting_to_knowledgebase.json` — Transcribes meeting recording with GPT, summarizes notes, and syncs to Airtable or Notion  

---

## 🚀 How to Use

1. Clone or download this repo  
2. Log into [Make.com](https://www.make.com)  
3. Create a new scenario and click **Import Blueprint**  
4. Paste contents of any `.json` file from the folder of your choice  
5. Customize modules (e.g., OpenAI keys, Gmail integration, Airtable tokens, etc.)  

---

## 🧩 Requirements

- A [Make](https://www.make.com) account  
- OpenAI API key (for GPT-powered modules)  
- Perplexity API key (for research-based personalization)  
- Any additional API access depending on your stack (e.g., Gmail, Google Calendar, Clearbit, Apify, Notion, CRM, etc.)  

---

## 📣 Contribute

Have a scenario to share?  
Fork this repo and open a pull request — we welcome battle-tested agents and modular blueprints.

---

## 💬 Questions or Feedback?

Connect with [Nate Shelly on LinkedIn](https://www.linkedin.com/in/nate-shelly/) or open an issue in this repo.

---

## ⚖️ License

MIT License — free to use and modify. Attribution appreciated.
