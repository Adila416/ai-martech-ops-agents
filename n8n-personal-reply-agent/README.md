# n8n Personal Reply Agent

This project demonstrates a simple, low-code AI agent built using **n8n** that generates a natural, ready-to-send reply to an incoming message.

The goal is to showcase practical agent design, prompt control, and clean output — without complex integrations or over-engineering.

---

## What this agent does

- Listens for an incoming message via n8n’s **Chat trigger**
- Uses an LLM to understand intent
- Produces a **plain-English reply only**
- Returns no metadata, JSON, summaries, or labels

This makes the output immediately usable in email, chat, or CRM workflows.

---


## Example

**Input**
just following up on the proposal we discussed last week.
**Output**
Hi! Thanks for following up. I’m reviewing the proposal and will get back to you with feedback shortly.
## Why Chat is used here

The **Chat trigger** is used purely for simplicity and demo purposes.

**Important:**  
This agent is **not limited to chat**.

The same logic and prompt can be reused with:
- Email (Gmail / IMAP / Outlook triggers)
- Slack messages
- Webhooks
- CRM or ticketing systems

Only the trigger changes — the agent behavior stays the same.

---

## Why this design

- Focuses on one clear, real-world task: drafting a reply
- Avoids unnecessary authentication and setup
- Demonstrates strong prompt control and output discipline
- Keeps the agent easy to extend into production workflows

---

## Tools used

- n8n (low-code automation)
- OpenAI Chat Model
- Chat trigger (replaceable with email or Slack)

---

## Notes

This agent is intentionally minimal to highlight:
- Clean output control
- Practical agent design
- Business-ready responses

It is designed to be a building block, not a monolith.
