# AI Automation Portfolio — Case Studies
**By Mehkan Fayyaz**

---

## 1. Lead Capture & Confirmation System

**Tools used:** n8n, Google Sheets API, Gmail API, OAuth2

**Problem:**
Businesses that collect leads through web forms often lose track of submissions when data isn't automatically organized or acknowledged. Manual entry into spreadsheets is slow, error-prone, and delays follow-up — which can cost a business a potential customer.

**Solution:**
I built an automation that captures form submissions in real time, instantly logs every entry into a structured Google Sheet, and sends the submitter an automatic confirmation email — with zero manual work after setup.

**Result:**
Every submission is now recorded and acknowledged within seconds of being sent, with no risk of a lead being missed or entered incorrectly. This is the exact workflow used by businesses to power lead-gen forms, contact pages, and signup flows.

---

## 2. Daily Quote Email (Scheduled Automation)

**Tools used:** n8n, Schedule Trigger, HTTP Request (public API), Gmail API

**Problem:**
Many small, repetitive tasks — like sending a daily update, reminder, or piece of content — get skipped simply because no one remembers to do them manually every single day.

**Solution:**
I built a fully scheduled automation that runs on its own every day: it fetches a fresh quote from a public API and emails it automatically, with no human involvement required after the initial setup.

**Result:**
A reliable, hands-off daily automation that demonstrates how any recurring business task — daily reports, reminders, digest emails — can be fully automated using a scheduled trigger and an external data source.

---

## 3. AI-Powered Feedback Alert System

**Tools used:** n8n, Google Gemini API (AI Agent), IF/conditional logic, Gmail API, Google Sheets API

**Problem:**
Businesses that collect customer feedback often miss urgent, negative feedback until it's too late, because someone has to manually read every single response to know what needs attention.

**Solution:**
I built an AI-powered system that reads every feedback submission using an AI agent, automatically classifies it as Positive or Negative, and takes a different action for each: negative feedback triggers an instant email alert to the business owner, while positive feedback is automatically logged to a spreadsheet for record-keeping — no manual reading required.

**Result:**
Critical feedback now reaches the business owner within seconds instead of being missed, while all feedback is still tracked without any manual sorting. This workflow combines AI decision-making with conditional business logic — the same pattern used in real customer support and reputation-monitoring systems.

---

---

## 4. AI Agent with Calculator Tool

**Tools used:** n8n, Google Gemini API (AI Agent), Calculator Tool

**Problem:**
AI language models are great at reasoning and conversation, but they sometimes give incorrect answers for precise calculations, since they predict likely text rather than actually computing numbers.

**Solution:**
I connected a Calculator tool directly to an AI Agent, so the agent can call it automatically whenever a question requires an exact numerical answer, instead of guessing based on patterns.

**Result:**
The agent now reliably answers precise calculations by using the right tool for the right task — demonstrating how AI agents can be extended with external tools to handle work that language models alone cannot do reliably. This is the same pattern used to build AI agents that can search the web, query databases, or take real actions.

---

## 5. Webhook Data Receiver

**Tools used:** n8n, Webhook (raw HTTP endpoint)

**Problem:**
Most real business systems — websites, CRMs, payment gateways, booking tools — need to send data into an automation automatically, without a human filling out a form.

**Solution:**
I built a raw webhook endpoint that accepts JSON data directly from any external system via a standard HTTP POST request, and tested it using real external tools sending live data.

**Result:**
This is the exact integration pattern used to connect n8n to real-world systems like websites, CRMs, and third-party APIs — the technical foundation behind most professional automation and integration work, beyond simple form-based automations.
