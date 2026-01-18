## What this repository demonstrates

- Designing **AI-forward Marketing Ops architectures**
- Building **no-code / low-code agents** using tools like Workato, Zapier, or Make
- Integrating AI into **Salesforce-centric GTM workflows**
- Applying **build vs. buy thinking** for AI MarTech solutions
- Communicating technical designs clearly to non-technical stakeholders

All examples are anonymized and safe for public sharing.

---

## Projects

### 1. Lead & Contact Enrichment + Routing Agent  
📁 `01-lead-enrichment-routing-agent`

**Business problem**  
Inbound leads arrive from multiple channels, but manual enrichment and routing slows speed-to-lead and creates inconsistent Salesforce data.

**Solution**  
A no-code / low-code AI agent that:
- Enriches inbound leads using structured inputs
- Classifies ICP fit, segment, and primary use case using an LLM
- Routes leads or contacts into Salesforce with the correct ownership
- Posts a summarized context into Slack for Sales

**What’s included**
- End-to-end workflow design (JSON-based)
- LLM prompt used for enrichment and routing logic
- Sample input and output payloads
- A lightweight Python scoring function that can be invoked from automation tools

**What this demonstrates**
- Practical AI usage in a live marketing workflow
- System orchestration across MAP → AI → Salesforce → Slack
- How no-code platforms and code can work together

---

### 2. Campaign Performance Insights Copilot  
📁 `02-campaign-insights-copilot`

**Business problem**  
Marketing teams have data, but turning it into clear insights and actions is slow and manual.

**Solution**  
A lightweight AI copilot that:
- Accepts campaign performance data
- Calculates key marketing and pipeline metrics
- Uses an LLM to summarize results and recommend actions

**What’s included**
- Sample campaign performance dataset
- Metric definitions and analysis logic
- AI prompt design for executive-ready summaries

**Status**
- Design-focused (logic and architecture are complete)
- Intended for implementation via no-code automation or lightweight scripts

---

### 3. AI MarTech Vendor Evaluation Framework  
📁 `03-ai-martech-vendor-framework`

**Purpose**  
A structured framework for evaluating AI-powered MarTech tools and deciding when to build internally vs. buy.

**What’s included**
- AI vendor scorecard with technical and operational criteria
- Build vs. buy decision checklist
- Focus on governance, scalability, and integration risk

**What this demonstrates**
- Experience with software procurement and POCs
- Strong business and technical judgment
- Long-term thinking about sustainable AI adoption

---

## Execution & Validation Notes

- This repository is intentionally **tool-agnostic**
- No proprietary systems or credentials are required
- JSON workflows and Python code are **syntactically valid**
- Python examples are lightweight by design and can run locally
- No-code workflows are represented declaratively (as they would be configured in platforms like Workato or Zapier)

This mirrors how AI-driven Marketing Ops solutions are often **designed, reviewed, and approved** before production deployment.

---

## How to review this repo

If reviewing as a hiring manager:
1. Start with the Lead Enrichment & Routing Agent
2. Review the workflow logic and prompts
3. Skim the vendor framework to see decision-making approach

Happy to walk through any design decisions or adapt these examples to a specific MarTech stack.
