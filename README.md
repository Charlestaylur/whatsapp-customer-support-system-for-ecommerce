# WhatsApp AI Customer Support System

> WhatsApp AI chatbot that handles customer support for e-commerce businesses — detects intent, responds naturally, logs conversations, and escalates to Slack when human attention is needed.

**Industry:** E-commerce / Retail

---

## Demo

<img width="1366" height="768" alt="Screenshot (521)" src="https://github.com/user-attachments/assets/0d7b0e89-8525-489a-a136-7f9dff4e1fe1" />

[Watch the full walkthrough →](https://drive.google.com/file/d/1TbUfShoEm1eiCXctxxHOnyme-gaX8y4T/view?usp=drivesdk)

---

## The Problem

E-commerce support teams spend a large chunk of their day answering the same product, payment, and account questions over and over. Messages come in at all hours, volume spikes are unpredictable, and when a real issue slips through without a response, the customer is already gone. Most businesses either overstaff to keep up or rely on customers to wait — neither option scales.

---

## The Solution

This system replaces the first line of customer support with a WhatsApp AI chatbot that understands what a customer is asking, responds in natural language, and only pulls in a human agent when the situation genuinely requires it. Every conversation is logged automatically so the support team always has full context.

---

## How It Works

1. **Customer sends a WhatsApp message** — The message is received via a webhook and routed into the workflow.
2. **Intent is detected in real time** — The AI classifies the message: product inquiry, account issue, payment problem, escalation trigger, or general support.
3. **AI generates a natural reply** — Based on the detected intent, the system composes a context-aware response and sends it back to the customer on WhatsApp.
4. **Conversation is logged to Google Sheets** — Every message, along with its timestamp and detected intent, is written to a central support log.
5. **Escalation check runs on every message** — If the system detects a situation that needs human involvement, it skips the AI reply and routes to the escalation branch.
6. **Slack alert is sent to the support team** — The flagged conversation is pushed to a Slack channel with full context so an agent can step in immediately.

---

## Tech Stack

| Tool | Role |
|---|---|
| **n8n** | Core workflow automation and orchestration |
| **WhatsApp Business API** | Incoming and outgoing customer messages |
| **OpenAI API** | Intent detection and natural language response generation |
| **Google Sheets** | Persistent conversation log with timestamps and intent labels |
| **Slack** | Real-time escalation alerts to the support team |

---

## Results

- Support responses went from manual and delayed to instant, 24/7, without adding headcount
- Every conversation is now logged with intent labels, giving the team a searchable record they never had before
- Human agents only get pulled in when it actually matters, cutting noise from the Slack escalation channel
- Customers interacting with the chatbot reported a natural experience — no robotic "press 1 for..." style responses

---

## About

Built by **Charles Emmanuel** — AI & Automation Systems Engineer.
Lagos, Nigeria | [LinkedIn](https://linkedin.com/in/charles-emmanuel-automation) | charlestaylurr@gmail.com

I build systems that remove repetitive manual work so teams can focus on what actually matters. If your business is losing time or money to broken processes, reach out.
