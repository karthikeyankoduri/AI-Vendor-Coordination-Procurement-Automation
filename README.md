# AI-Vendor-Coordination-Procurement-Automation

<img width="1282" height="617" alt="image" src="https://github.com/user-attachments/assets/417739a4-c6d3-44fc-8f12-0ecd9f7f4e43" />


This n8n workflow automates the complete procurement and vendor coordination process using AI, Google Sheets, Airtable, Gmail, WhatsApp, and Slack integrations.

The system reduces manual follow-ups by automatically analyzing procurement requests, identifying vendors, sending RFQs, tracking responses, sending reminders, and escalating delays.

---

## Workflow Overview

### 1. Procurement Request Trigger

The workflow starts when a new procurement request is added through:

* Google Sheets
* Airtable

The request contains:

* Material name
* Quantity
* Budget
* Deadline
* Priority
* Project name

---

## 2. AI Procurement Analysis

An AI agent powered by OpenAI analyzes the procurement request and extracts:

* Material category/type
* Urgency level
* Procurement summary
* Suggested vendors

The AI converts unstructured procurement data into structured insights for automated processing.

---

## 3. Vendor Database Lookup

The workflow searches a vendor database stored in Google Sheets and filters vendors based on:

* Material category
* Vendor specialization
* Vendor availability

This enables dynamic vendor matching without manual searching.

---

## 4. RFQ Generation & Distribution

The workflow automatically prepares Request for Quotation (RFQ) data and sends it through:

* Gmail
* WhatsApp Cloud API

Each RFQ includes:

* RFQ ID
* Material details
* Quantity
* Budget
* Deadline
* Project information
* Urgency level

---

## 5. RFQ Tracking System

All RFQs are logged into Google Sheets for centralized tracking.

Tracked information includes:

* Vendor details
* RFQ status
* Sent timestamps
* Procurement information

This creates a lightweight procurement management dashboard.

---

## 6. Automated Reminder System

A scheduled workflow runs daily to identify vendors who have not responded.

If no response is received after a defined period:

* Automated reminder emails are sent
* Response delays are tracked automatically

This removes the need for manual vendor follow-ups.

---

## 7. Escalation Workflow

If vendors remain unresponsive after multiple reminders:

* Slack alerts are sent to managers
* Escalation notifications include:

  * Vendor details
  * RFQ ID
  * Days delayed
  * Procurement deadline

This ensures critical procurement tasks do not get blocked.

---

# Key Features

* AI-powered procurement analysis
* Automated vendor coordination
* RFQ generation via Gmail and WhatsApp
* Centralized procurement tracking
* Automated reminders
* Escalation management using Slack
* Multi-platform integration
* Low-code workflow automation using n8n

---

# Tech Stack

* n8n
* OpenAI API
* Google Sheets API
* Airtable API
* Gmail API
* WhatsApp Cloud API
* Slack API

---

# Use Cases

* Construction procurement
* Vendor management
* Facility management operations
* Supply chain coordination
* Internal procurement automation

---

# Outcome

This workflow streamlines procurement operations by automating repetitive vendor communication tasks, improving response tracking, reducing delays, and enabling centralized operational visibility through AI-driven workflows.
