# Lead & Contact Enrichment + Routing Agent

## Overview

This project demonstrates how to design a **no-code / low-code AI agent** that enriches, scores, and routes inbound marketing leads or contacts into Salesforce while providing clear, actionable context to Sales.

The solution is designed for Marketing Operations teams operating at scale, where speed-to-lead, data consistency, and operational efficiency are critical.

All examples are anonymized and represented declaratively.

---

## Business Problem

Inbound leads arrive from multiple channels (web forms, events, content downloads, intent tools), but:

- Manual enrichment slows response time
- ICP assessment is inconsistent
- Routing rules are fragmented
- Sales lacks immediate context

This results in delayed follow-up, poor data quality, and lost pipeline.

---

## Solution Summary

A **no-code / low-code AI-powered workflow** that:

1. Triggers on new lead or contact creation
2. Enriches the record with company and engagement data
3. Uses an LLM to assess:
   - ICP fit
   - Segment (SMB / Mid-Market / Enterprise)
   - Primary use case
4. Routes the lead or contact into Salesforce with correct ownership
5. Posts a concise AI-generated summary to Slack for Sales

The orchestration layer is represented as a JSON workflow, similar to how tools like **Workato, Zapier, or Make** operate in practice.

---

## High-Level Architecture

```mermaid
flowchart LR
  A[Marketing Source<br/>(Form, Event, Intent)] --> B[No-code Automation<br/>(Workato / Zapier)]
  B --> C[LLM Enrichment & Scoring]
  C --> B
  B --> D[Salesforce<br/>Lead / Contact]
  B --> E[Slack<br/>Sales Notification]
