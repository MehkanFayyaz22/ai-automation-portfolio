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

## 6. RAG Chat with documents

Tools used: n8n, Google Gemini (Chat Model + Embeddings), Simple Vector Store, AI Agent, Form Trigger

Problem: Businesses often have documents (PDFs, manuals, policies, FAQs) that customers or employees need answers from, but manually searching through them every time is slow and inefficient — and a generic AI chatbot without access to that specific data will just guess or give a generic answer.

Solution: I built a two-stage RAG (Retrieval-Augmented Generation) system. First, documents are converted into embeddings and indexed into a vector store. Then, an AI Agent connected to that same vector store answers questions submitted through a form by retrieving the exact relevant document content before generating a response, instead of relying on general knowledge alone.

Result: Users get accurate, document-grounded answers instead of generic AI guesses. This is the same architecture used to power internal knowledge-base bots, customer support assistants, and document Q&A tools — one of the most in-demand automation patterns for real businesses today.

## 7. AI Chatbot with Error Handling

Tools used: n8n, Google Gemini Chat Model, Basic LLM Chain, HTTP Request (ntfy.sh), Chat Trigger

Problem: A chatbot that silently fails when the AI model errors out (rate limits, bad input, API downtime) leaves the developer unaware of the failure — and the end user gets no response with no explanation, which is unacceptable in a real client-facing system.

Solution: I built a chat-based AI assistant using a Basic LLM Chain, with explicit Success and Error output handling. When a request succeeds, the response flows normally; when it fails, the workflow automatically sends a real-time push notification, so failures are caught and visible instead of disappearing silently.

Result: This turns a "hobby" chatbot into a production-ready system — the same reliability pattern (success/error branching + alerting) used in real client automations to guarantee uptime awareness and fast debugging.

## 8. Oil Lab — Sample Tracking System (4-Workflow System)


Tools used: n8n, Webhook, Google Sheets API, IF/Conditional Logic

Problem: Labs handling sample testing (like oil analysis) need to track each sample through multiple stages — intake, testing, doctor review, and status checking — but doing this manually across spreadsheets and phone calls leads to lost samples, delayed results, and no single source of truth.

Solution: I built a 4-workflow automation system covering the full sample lifecycle:

Sample Intake — logs each incoming sample into a central Google Sheet the moment it's received.
Update Status — updates a sample's status (e.g. Purity Testing, Quality Check, Report Ready) via webhook, with conditional logic routing valid vs. invalid status updates.
Doctor Result Entry — lets a doctor submit test results, which are recorded against the correct sample automatically.
Check Status — allows anyone to query a sample's current status in real time without contacting the lab directly.

Result: A full sample goes from intake to final report entirely through automated workflows, with zero manual spreadsheet editing and instant status visibility at every stage. This demonstrates a complete, multi-workflow business system — the kind of end-to-end automation clients pay for, not just a single isolated task.

## 9. AI Appointment Booking Assistant

Tools used: n8n, Form Trigger, Google Gemini (Basic LLM Chain), Code Node (JavaScript), IF/Conditional Logic, Google Calendar API, Google Sheets API, OAuth2

Problem: Clinics, salons, labs, and other service businesses often take appointments through phone calls and chat messages. Someone has to read each request, check the diary, reply, and write the booking down by hand. This is slow, and it leads to double bookings and appointments that never get recorded in one place.

Solution: I built an AI booking assistant where a customer fills in a simple form with their name and a message like "Tomorrow at 4 PM". The workflow uses an AI model to understand the date and time (including Urdu and Roman Urdu messages), checks Google Calendar to see if that slot is free, and then branches: if the slot is free, it books the appointment, records it in Google Sheets, and shows a confirmation page; if the slot is taken, the customer is told right away to pick another time. A validation step also catches messages with no clear date or time, so the customer gets a helpful prompt instead of a failed request.

Result: Customers get an instant answer, double bookings are prevented because every request is checked against the live calendar, and every booking is saved automatically in one spreadsheet. This workflow combines AI language understanding, calendar integration, conditional logic, and input validation — the same pattern used in real booking systems for clinics, salons, and service businesses.

## 10. AI Customer Support Chatbot for an Oil Testing Lab

**Tools used:** n8n (self-hosted with Docker), Google Gemini API (AI Agent), Window Buffer Memory, Chat Trigger, Google Sheets API

**Problem:** Testing labs get the same questions again and again: "What is the rate for this test?", "How long does the report take?", "How much oil do I need to send?" Staff spend hours answering them by phone and messages, and customers who message after working hours wait until the next day for a reply.

**Solution:** I built an AI chatbot that answers customer questions instantly, using only the lab's own information (services, rates, timings, turnaround time and sample requirements). It replies in the customer's own language (English, Urdu or Roman Urdu) and remembers the earlier messages in the conversation, so follow-up questions like "and how many days does it take?" are understood correctly. If a customer asks something outside the lab's information, the bot does not guess. It tells the customer that a team member will contact them and collects their name and phone number. Every question and answer is saved automatically to a Google Sheet, so the lab can review enquiries and follow up on potential customers.

**How it works:**
1. A customer sends a message through the chat.
2. The AI Agent reads the message together with the lab's rules and information (the system message) and the recent conversation (memory).
3. Google Gemini writes the reply, which is shown to the customer.
4. The date, session ID, customer message and AI reply are added as a new row in Google Sheets.

**Safety rules built into the prompt:** the bot never invents prices or timings, never interprets test results or gives technical advice, never confirms final prices or discounts, and hands the customer over to the team whenever it is unsure. The AI Agent node is also set to retry automatically if the AI service is briefly unavailable.

**Result:** A working demo chatbot that answers common lab questions instantly, keeps conversations in context and records every enquiry in a spreadsheet. The demo uses a sample lab ("PetroCheck") with example rates, and it can be adapted to a real lab by replacing the information in the system message. The same pattern works for clinics, schools, shops and any business that answers repeated customer questions.

