> Focused on the message generation step only. See [ai-cold-email-automation] for the full send pipeline.

# AI Cold Email Automation

Automated pipeline that takes structured lead data, generates a personalized cold email using Google Gemini, and sends it via Gmail — all without manual writing.

Built with n8n to demonstrate how LLMs fit into real automation workflows.

# System Architecture

```
Lead Data
   ↓
AI Email Generation (Google Gemini)
   ↓
JSON Parsing (JavaScript Code Node)
   ↓
Email Sending (Gmail API)
```

The workflow is implemented using **n8n**, where each step of the pipeline processes the output from the previous stage.

---

# Project Overview

Cold outreach is a common process in marketing and sales teams, but writing personalized emails manually is time-consuming.

This project automates the process by generating personalized cold emails using AI based on structured lead data and sending them automatically through Gmail.

The workflow demonstrates how AI can be integrated with automation platforms to build real-world productivity systems.

---

# Workflow Architecture

Lead Data → AI Email Generation → JSON Parsing → Gmail Sending

Step-by-step pipeline:

1. Lead information is provided (name, company, role, pain point)
2. Google Gemini generates a personalized cold email
3. A JavaScript node parses the structured JSON response
4. Gmail node sends the email automatically

---

# Example Generated Email

**Subject:** Improving AI Workflows at GrowthTech

Hi Rahul,

As CTO at GrowthTech, you're likely focused on optimizing AI automation workflows.

I'm Monil from AIFlow. We help companies streamline AI deployment pipelines, reducing bottlenecks and accelerating delivery.

Would you be open to a brief 15-minute conversation next week to explore whether this could benefit GrowthTech?

Best,
Monil

---

# Tech Stack

* n8n (workflow automation)
* Google Gemini API
* Gmail API
* JavaScript
* GitHub

---

# Repository Structure

```
ai-cold-email-automation
│
├ workflow
│   └ cold_email_workflow.json
│
├ screenshots
│   ├ workflow.png
│   ├ execution.png
│   └ email_result.png
│
└ README.md
```

---

# Screenshots

## n8n Workflow

![Workflow](screenshots/workflow.png)

## Workflow Execution

![Execution](screenshots/execution.png)

## Generated Email Result

![Email Result](screenshots/email_result.png)

---

# Key Features

* AI-generated personalized cold emails
* Automated workflow using n8n
* Structured JSON output from LLM
* Automated email sending via Gmail
* JavaScript parsing for AI response formatting

---

# Future Improvements

* Google Sheets integration for automated lead ingestion
* Follow-up email automation
* Campaign logging and tracking
* Subject line A/B testing
* Lead data enrichment for deeper personalization
* Campaign performance analytics

---


