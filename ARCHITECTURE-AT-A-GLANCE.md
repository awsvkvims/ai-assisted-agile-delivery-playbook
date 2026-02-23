# Architecture At A Glance

This repository is organized around a three-layer model designed to help teams move from predictability to speed to mastery in value delivery.

---

## The Three Layers

Layer 1: Thesis  
The opinionated foundation.  
Quality Driven Delivery (QDD), shift-left thinking, and AI as a feedback amplifier.

Layer 2: Workflow  
The end-to-end journey from idea to production to learning.

Layer 3: Role Guides  
Practical AI assistance for Product Owners, Developers, Test Engineers, DevOps, Platform, and Delivery Leaders.

---

## How The Layers Fit Together

``` mermaid
flowchart TB
  T[00-thesis\nPrinciples and philosophy]
  W[01-workflow\nIdea to production to learning]
  R[02-role-guides\nAI assistance per role]

  T --> W
  R --> W

  AA[ARCHITECTURE-AT-A-GLANCE.md\nVisual orientation]
  AA --> T
  AA --> W
  AA --> R
```
---

## Stream Aligned Teams And Platform Teams

Most organizations split responsibilities across two primary team types:

- Stream-aligned teams own product outcomes and business delivery.
- Platform teams own paved roads, guardrails, and shared capabilities.

The workflow spans both. The difference is where each team spends most of its time, and what done means.

``` mermaid
flowchart LR

  subgraph WF[End to End Delivery Workflow]
    I[Ideation and discovery]
    B[Backlog and slicing]
    D[Design and architecture]
    T[Test strategy and QDD]
    DEV[Code and review]
    CI[CI signals and quality gates]
    CD[Progressive delivery]
    RUN[Runtime monitoring]
    LRN[Learning and adaptation]

    I --> B --> D --> T --> DEV --> CI --> CD --> RUN --> LRN
  end

  AI1[AI assist\nclarify problem\nreframe hypothesis]
  AI2[AI assist\nstory slicing\nacceptance criteria]
  AI3[AI assist\ndesign tradeoff exploration]
  AI4[AI assist\ntest case generation]
  AI5[AI assist\ncode scaffolding\nrefactor suggestions]
  AI6[AI assist\nCI failure analysis]
  AI7[AI assist\nlog and metric summarization]
  AI8[AI assist\nretrospective signal clustering]

  AI1 -.-> I
  AI2 -.-> B
  AI3 -.-> D
  AI4 -.-> T
  AI5 -.-> DEV
  AI6 -.-> CI
  AI7 -.-> RUN
  AI8 -.-> LRN
```
---

## Stream Aligned And Platform Team Feedback Loop

Platform teams reduce cognitive load by providing paved roads.
Stream aligned teams generate real world signals that shape platform evolution.

``` mermaid
flowchart LR

  SA[Stream aligned team\nDelivers product outcomes]
  PT[Platform team\nBuilds paved roads and guardrails]

  SA -->|Feature needs\nPain points\nScaling limits| PT
  PT -->|Templates\nTooling\nPolicies\nObservability| SA

  SA -->|Adoption metrics\nFailure patterns\nDX feedback| PT
  PT -->|Platform roadmap\nCapability upgrades| SA
```
---

## Enablement Architecture

The workflow is supported by platform capabilities that reduce cognitive load and increase safety:

- Guardrails in CI/CD
- Built-in quality practices
- Observability and feedback signals
- Platform templates and paved roads
- Policy and compliance checks

These are described in 04-enablement-architecture.

---

## AI As An Overlay

AI is not a separate phase.

AI is injected at key feedback points:

- Requirement clarification
- Story slicing
- Test generation
- Code scaffolding
- CI signal interpretation
- Monitoring analysis
- Retrospective insight generation

The goal is amplification of signal, not replacement of discipline.

---

## MVP Scope

Current version focuses on:

- Stream-aligned team workflow
- Product Owner, Developer, DevOps roles
- One simple feature walkthrough

Future iterations will expand:

- Platform team operating model and roadmap integration
- Governance patterns for regulated environments
- Data and AI delivery workflows
- Advanced observability patterns

---

## Suggested Reading Order

- Start with 00-thesis to understand the stance and vocabulary
- Use 01-workflow as the shared map of how value moves
- Use 02-role-guides when you want role-specific AI assistance
- Use 03-sample-walkthroughs to see a complete example end-to-end