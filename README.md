# 💡 Make AI Automation Agents & Blueprints

This repository contains a curated library of **AI-first automation agents and workflow blueprints**, designed in [Make](https://www.make.com). Each folder represents a full automation use case — from browser-based automation to outbound prospecting, inbound lead response, meeting scheduling, and internal onboarding synced to knowledge bases.

Every scenario is modular, customizable, and production-ready — allowing you to deploy scalable, intelligent workflows without starting from scratch.

---

## 🧠 What’s Inside

- ✅ **Autonomous agents** that qualify leads, send emails, scrape data, and book meetings  
- 🔁 **Reusable sub-scenarios** like `get_available_time_slots` and `book_meeting`  
- 🧩 **Dynamic logic + GPT-4** for classification, personalization, and routing  
- 🔗 **Integrations** with Gmail, Google Calendar, Airtable, Sheets, Notion, and 3rd-party APIs  

---

## 📁 Folder Structure

Each folder below contains `.json` blueprints (Make scenarios), reusable sub-modules, and notes.

---

### `Browser_Automation_Agent/`  
Headless browser automation agent that runs dynamic actions such as profile visits, scraping, clicks, and in-browser flows.

**Includes:**
- `Open_Linkedin_Profile.json`  
  - Opens a LinkedIn profile from a given URL to register a page visit  
- `Click_Button_By_Text.json`  
  - Simulates a browser click on a button with matching visible text  
- `Extract_Profile_Data.json`  
  - Extracts HTML or DOM data from a visited page  
- `Send_LinkedIn_DM.json`  
  - Inputs text into LinkedIn's DM field and clicks send  

---

### `B2B_AI_Prospecting_Agent/`  
Outbound AI sales engine that generates personalized emails, handles responses, and routes leads based on context.

**Includes:**
- `Engagement_1_Generation.json`  
  - Generates personalized cold emails based on persona, product, and research  
- `Engagement_2_ResponseHandler.json`  
  - Classifies replies and responds accordingly  
- `Engagement_3_RoutingLogic.json`  
  - Routes conversations to the correct follow-up path (e.g., book call, escalate, disqualify)  

---

### `Inbound_Lead_Response_Agent/`  
Automatically handles inbound leads from forms, email, or CRM and responds using GPT to qualify and guide.

**Includes:**
- `Inbound_Email_Listener.json`  
  - Detects new lead events or emails to trigger response flow  
- `Qualification_Sequence.json`  
  - Uses GPT logic to ask tailored follow-up questions and score responses  
- `Meeting_Booking_Sequence.json`  
  - Sends meeting link or books time dynamically if the lead is qualified  

---

### `Calendar_Scheduling_Agent/`  
Manages meeting availability, sends booking links, and schedules directly via Google Calendar.

**Includes:**
- `get_available_time_slots.json`  
  - Pulls open time slots from Google Calendar  
- `book_meeting_with_availability.json`  
  - Creates a Google Calendar invite using selected time  
- `send_calendar_link.json`  
  - Delivers a Calendly or Make-generated scheduling link to the contact  

---

### `Agent_Tools/`  
Support modules to be embedded in other agents for enrichment, notifications, or formatting.

**Includes:**
- `format_dates_to_ISO.json`  
  - Normalizes date inputs for API compatibility  
- `enrich_domain_data.json`  
  - Pulls company/person data from Clearbit or similar APIs  
- `slack_notify.json`  
  - Sends formatted Slack alerts  
- `lookup_knowledge_base.json`  
  - Queries a GPT model or vector DB to fetch answers  

---

### `Employee_Onboarding_Knowledge_Sync/`  
Complete 2-part flow that handles onboarding—from form intake to post-meeting transcription + sync to knowledge base.

#### `Part_1_Form_to_Meeting/`  
Automates the initial intake and meeting setup after a form is submitted.

**Includes:**
- `new_hire_intake_to_calendar.json`  
  - Creates Airtable record, generates folder, assigns tasks, and schedules intro meeting  

#### `Part_2_Post_Meeting_Sync/`  
Runs after the onboarding meeting is complete.

**Includes:**
- `onboarding_meeting_to_knowledgebase.json`  
  - Transcribes the meeting recording using GPT, summarizes, and syncs to Airtable or Notion  

---

## 🚀 How to Use

1. Clone or download this repo  
2. Go to [Make](https://www.make.com) and log in  
3. Create a new scenario and click **Import Blueprint**  
4. Paste contents of any `.json` file  
5. Update modules with your credentials (OpenAI keys, Google Calendar, Airtable, Slack, etc.)  

---

## 🧩 Requirements

- Make.com account  
- OpenAI API key (for GPT-based messaging and classification)  
- Perplexity API key (for research-based personalization)  
- API access for Gmail, Google Calendar, Airtable, Clearbit, Notion, Slack, etc.  

---

## 📣 Contribute

Have an automation or callable sub-agent to share?  
Fork this repo, add your `.json` blueprints, and open a pull request.

---

## 💬 Questions or Feedback?

Message [Nate Shelly](https://www.linkedin.com/in/nate-shelly/) on LinkedIn or open an issue in this repo.

---

## ⚖️ License

MIT License — free to use, clone, and modify. Attribution appreciated.
