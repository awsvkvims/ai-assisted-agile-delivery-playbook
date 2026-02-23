# Architecture at a Glance

This document provides a **visual orientation** to the *AI-Assisted Agile Delivery Playbook* repository.

It shows **how the major conceptual areas relate to each other** without going into tool-specific implementation details.
Use this as a map — not a specification.

---

## How to Use This Document

- Start with the **Repository Overview** diagram to understand scope
- Jump to the diagram that matches the question you’re asking
- Follow the links in each section to go deeper

You do not need to read this file top-to-bottom.

---

## Repository Overview

**Purpose:** Show the major areas of this repository and how they fit together (orientation only — not flow).

```mermaid
flowchart LR
  R[Repository Root<br/>ai-assisted-agile-delivery-playbook]
  O[00-overview<br/>scope & audiences]
  S[01-system-model<br/>QDD + shift-left system]
  A[02-ai-injection-points<br/>where AI amplifies feedback]
  RA[03-reference-architecture<br/>workflow + guardrails]
  W[04-workflows<br/>end-to-end walkthroughs]
  AS[05-starter-assets<br/>templates & examples]
  L[06-leadership-conversations<br/>talk tracks & FAQs]

  R --> O
  R --> S
  R --> A
  R --> RA
  R --> W
  R --> AS
  R --> L
```

## System Storyline

**Purpose:** Establish the “primary storyline”: QDD + shift-left amplified by AI feedback loops.

``` mermaid
flowchart LR
  Q["Quality-Driven Delivery<br/>(QDD mindset)"]
  SL["Shift-left feedback<br/>(requirements → design → test)"]
  TE["Technical excellence<br/>(CI/CD, automation)"]
  AI["AI-assisted enablement<br/>(reduce cognitive load)"]
  OUT["Outcomes<br/>(flow, quality, learning)"]

  Q --> SL --> TE --> OUT
  AI --> SL
  AI --> TE
```

### Diagram Index
- Repository Overview → see what’s in the repo
- System Storyline → QDD + shift-left + AI feedback loops
- AI Injection Points → where AI helps at requirements/design/test/code/ops
- Reference Architecture → how workflows, guardrails, and monitoring connect
- End-to-End Workflows → practical walkthroughs you can follow

