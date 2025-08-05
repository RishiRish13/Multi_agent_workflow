# Multi_agent_workflow
This system uses n8n to automate personal finance tracking: it reads Gmail for transaction alerts, extracts and categorizes expenses using OpenAI, logs them to Google Sheets, and sends daily summary emails categorized by spend type all hands-free.

Personal Finance Analyzer – Automated Daily Expense Tracker
📌 Overview
The Personal Finance Analyzer is a fully automated workflow built using n8n that helps you:

🔍 Extract transactions from Gmail (SMS/Email)

📊 Categorize expenses using OpenAI

📁 Log transactions into Google Sheets

📬 Send daily summaries of expenses by category to your inbox

No manual entry. No effort. Just effortless finance tracking, daily.

🚀 Features
✅ Auto-parses transactional SMS/emails

🧠 Uses GPT to auto-categorize spending (e.g. Food, Travel, Bills)

📄 Logs entries in a structured Google Sheet

📬 Sends a daily Gmail summary of total spends per category

⏰ Fully scheduled, runs every morning automatically

🔧 Tech Stack
n8n – Low-code automation

Google Sheets – Centralized transaction log

Gmail – Transaction source and summary delivery

OpenAI API – Smart categorization with GPT

Cron Scheduler – For daily email automation

📂 Workflow Breakdown
1. Gmail Trigger
Captures incoming transactional messages.

2. Code Parser
Extracts amount, vendor, type, and date from messages.

3. OpenAI Categorizer
Uses GPT to auto-detect the expense category (Food, Bills, etc.).

4. Google Sheets Logger
Appends parsed transactions to a sheet (Personal Finance Logs).

5. Daily Summary Email
Every morning, reads all sheet rows, aggregates totals per category, and sends a summary email.
