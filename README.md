# WhatsApp AI Customer Support System

> WhatsApp chatbot that detects customer intent, responds naturally, logs every conversation, and escalates to the support team on Slack when human attention is needed using n8n, OpenAI, and Google Sheets.

**Industry:** E-commerce / Retail
**Built for:** E-commerce businesses that want to handle first-line customer support on WhatsApp automatically without missing messages or overloading the support team.

---

## Demo

[Watch the full walkthrough →](https://drive.google.com/file/d/1TbUfShoEm1eiCXctxxHOnyme-gaX8y4T/view?usp=drivesdk)

<img width="852" height="408" alt="Github Whats" src="https://github.com/user-attachments/assets/049f472a-e3c4-41c2-a121-2bd56570c89c" />


---

## The Problem

E-commerce support teams spend a large chunk of their day answering the same product, payment, and account questions over and over. Messages come in at all hours, volume spikes are unpredictable, and when a real issue slips through without a response, the customer is already gone.

Most businesses either overstaff to keep up or rely on customers to wait. Neither option scales.

---

## The Solution

This system replaces the first line of customer support with a WhatsApp AI chatbot that understands what a customer is asking, responds in natural language, and only pulls in a human agent when the situation genuinely requires it. Every conversation is logged automatically so the support team always has full context when they step in.

---

## How It Works

1. **Customer sends a WhatsApp message** — The message arrives via the WhatsApp Business API, hits a webhook, and triggers the n8n workflow instantly.
2. **Intent is detected in real time** — OpenAI classifies the message into a category: product inquiry, account issue, payment problem, escalation trigger, or general support.
3. **AI generates a natural reply** — Based on the detected intent, the system composes a context-aware response and sends it back to the customer on WhatsApp.
4. **Conversation is logged to Google Sheets** — Every message, along with its timestamp and detected intent, is written to a central support log for the team to reference.
5. **Escalation check runs on every message** — If the system detects a situation that needs human involvement, it skips the AI reply and routes to the escalation branch.
6. **Slack alert sent to the support team** — The flagged conversation is pushed to a Slack channel with full context so an agent can step in immediately.

---

## Tech Stack

| Tool | Role |
|---|---|
| **n8n** | Core workflow engine and orchestration layer |
| **WhatsApp Business API** | Inbound and outbound customer messaging channel |
| **OpenAI API** | Intent detection and natural language response generation |
| **Google Sheets** | Persistent conversation log with timestamps and intent labels |
| **Slack** | Real-time escalation alerts to the support team |
| **Webhooks** | Connects WhatsApp Business API to n8n when a message arrives |

---

## Results

- Support responses went from manual and delayed to instant, 24/7, without adding headcount
- Every conversation is now logged with intent labels, giving the team a searchable record they never had before
- Human agents only get pulled in when it actually matters, cutting noise from the Slack escalation channel
- Customers interacting with the chatbot reported a natural experience, no robotic press-1-for style responses

---

## About

Built by **Charles Emmanuel** — AI & Automation Systems Engineer.   
Lagos, Nigeria | [LinkedIn](https://linkedin.com/in/charles-emmanuel-automation) | charlestaylurr@gmail.com

I build systems that remove repetitive manual work so teams can focus on what actually matters. If your business is losing time or money to broken processes, reach out.
