### **Make AI Automation Agents & Blueprints**

**An AI-first library of modular, production-ready automation blueprints built in Make.com.**

This repository is your go-to resource for **powerful, AI-first automation agents and workflow blueprints** designed to save you time and supercharge your business processes. Each folder contains a complete, customizable automation scenario, ready to be deployed in your own Make.com account.

From intelligent outbound outreach and dynamic CRM enrichment to automated internal tools, these blueprints put AI at the core of your operations.

---

### **Key Features**

* **Autonomous Agents:** Deploy intelligent agents that can qualify leads, send personalized emails, visit profiles, and respond with dynamic, contextual awareness.
* **Modular & Reusable Components:** Leverage pre-built, reusable modules like `book_meeting` and `get_available_calendar_slots` to accelerate your own automation development.
* **Dynamic Decision Logic:** Harness the power of GPT-4 for real-time classification, data enrichment, and hyper-personalized messaging.
* **Seamless Integrations:** Connect effortlessly with popular platforms including Gmail, Google Calendar, HubSpot, Salesforce, LinkedIn, and various external APIs.

---

### **Folder Structure & Use Cases**

Each folder represents a comprehensive use case or a reusable utility. Inside, you'll find `.json` blueprint files, detailed implementation notes, and relevant sub-scenarios.

**`Browser_Automation_Chrome_or_Chromium_Based/`**

* **HubSpot to LinkedIn Auto-Connect with GPT4o Message:** Automatically connect with contacts and send personalized messages.
* **HubSpot to LinkedIn Auto-Connect with No Message:** Automatically connect with contacts without sending a message.

**`Business_Estimate_Automation/`**

* **Extract Revit Designs to Automate Business Estimates:** Streamline your estimation process by extracting key data from Revit designs.

**`Deep_Research_CRM_Enrichment/`**

* **HubSpot CRM Deep Research Enrichment:** Enhance your HubSpot records with deep, AI-powered research.
* **Salesforce CRM Deep Research Enrichment:** Enrich your Salesforce contacts and accounts with valuable external data.

**`Employee_Onboarding_GPT_Agent_Sync/`**

* **Part 1 (Form to Meeting Setup):** Automate the initial stages of employee onboarding, from form submission to meeting scheduling.
* **Part 2 (Post-Meeting → Transcribe + Train GPT or Agent):** Post-meeting workflows that transcribe discussions and train an AI agent with the new information.

**`Gmail_and_Email_Automation/`**

* **Inbound SDR Agent:** A smart agent that handles and qualifies inbound leads via email.
* **Outbound SDR Engagement (1, 2, 3):** A series of strategic outbound email campaigns for sales development representatives.
* **HubSpot Deep Research Enrichment:** Enrich HubSpot contacts directly from email data.
* **Salesforce CRM Deep Research Enrichment:** Enrich Salesforce contacts directly from email data.
* **HubSpot to LinkedIn Auto-Connect with GPT4o Message:** Connect and message leads on LinkedIn after an email interaction.
* **HubSpot to LinkedIn Auto-Connect with No Message:** Connect on LinkedIn silently after an email interaction.

---

### **Reusable Tools**

These are standalone `.json` blueprints that can be imported into any of your Make scenarios.

**`book_meeting/`**
* `book_meeting.json`: Schedules a meeting based on provided time and context.

**`get_available_calendar_slots/`**
* `get_available_calendar_slots.json`: Fetches real-time calendar availability to avoid scheduling conflicts.

---

### **How to Use**

1.  **Clone or Download:** Get a copy of this repository to your local machine.
2.  **Import to Make:** Log in to [Make.com](https://www.make.com), create a new scenario, and click **Import Blueprint**.
3.  **Paste & Customize:** Paste the contents of your desired `.json` file.
4.  **Configure:** Connect your apps (e.g., add your OpenAI key, Gmail account, HubSpot connection, etc.) and customize the modules to fit your specific needs.

---

### **Requirements**

* A [Make.com](https://www.make.com) account.
* An OpenAI API key (for GPT-enhanced logic).
* A Perplexity API key (for deep research modules).
* Access to any third-party platforms you intend to connect (e.g., Gmail, Google Calendar, HubSpot, Salesforce).

---

### **Contribute**

We welcome contributions from the community! If you've created a useful automation, please:
1.  **Fork this repo.**
2.  **Add your `.json` scenario** to the most relevant folder.
3.  **Open a pull request** with a clear description of your contribution.

---

### **Get in Touch**

Have questions, feedback, or need assistance?
* Message [Nate Shelly on LinkedIn](https://www.linkedin.com/in/nate-shelly/).
* Open an issue in this repository.

---

### **License**

This project is licensed under the **MIT License**. You are free to use, clone, and modify it. Attribution is greatly appreciated.
