## 🧠 n8n Workflows Collection

This repository contains a set of practical and production-ready **n8n workflows** built to automate everyday business, personal productivity, and communication tasks. Each workflow is crafted to leverage popular integrations like Google Sheets, Slack, Email, and webhooks, enabling seamless and intelligent task execution with minimal manual effort.

---

### 📁 Workflow Descriptions

#### 1. **Expense Report Tracker**

Automates expense tracking from natural language inputs. Accepts chat messages like
`"I bought lunch for ₹250 on July 31"` or
`"Received ₹5000 from freelance work on August 1"`
and extracts:

* **Transaction Type**: Purchase / Income / Transfer
* **Amount**
* **Date**
* **Description**
  The data is then stored for future analysis or reporting.

#### 2. **Form Submission**

Automates data capture and response for form entries. When a user submits their:

* **Name**
* **Phone Number**
* **Email**
* **Personal Description**
* **Selected Interests (from a list)**
  the workflow performs:
* Sends a **confirmation email** to the user
* Sends a **Slack notification** to the internal backend/team with form details

#### 3. **Google Sheets Contact Sync**

Monitors a Google Sheet for new contact entries containing:

* Name
* Phone Number
* Email
* Description
  For each new entry, it:
* Sends a **Slack message** to the team
* Sends an **email** to the contact
* Creates a **Google Contact** using the provided details

#### 4. **Lead Generator (LinkedIn)**

Processes chat inputs like:
`"Find marketing managers in Bangalore"`
Then:

* Extracts leads based on job title and location
* Returns a list of prospects with:

  * **Name**
  * **Job Title**
  * **Summary Snippet**
  * **LinkedIn Profile URL**
    The results are saved to Google Sheets for easy access.

#### 5. **Resume Review Bot**

Evaluates how well a resume matches a given job description (JD).
Given a **Resume** and a **JD**, it:

* Scores different components like Skills, Experience, Education, etc.
* Calculates a **weighted average match score**
* Provides **section-wise feedback** for improvement

#### 6. **Stock Buy/Sell Advisor**

Provides trading advice based on short-term trends.
Using historical stock prices:

* Calculates the **3-day** and **7-day moving averages**
* Suggests **Buy** if short-term trend is rising
* Suggests **Sell** if short-term trend is falling
* Remains neutral if trends are flat or inconsistent

#### 7. **Weather-Based Delivery Decision**

Checks real-time weather conditions at the delivery location.
Based on keywords like "rain", "storm", "snow", etc., it:

* Advises whether to **proceed with delivery** or **delay due to bad weather**
* Can be used in logistics or dispatch workflows for real-time decision-making

---

## Tech Stack

* **n8n** – Open-source workflow automation
* **Google Sheets**
* **Slack**
* **Email**
* **Webhook Inputs**
* **Custom Scripting & Expressions**

