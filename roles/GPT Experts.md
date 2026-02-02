# File Header

## Version
2026-02-01 18:33 UTC

## Author
Lance Hegland (lance.hegland@gmail.com)

## Purpose
Define a reusable “expert-team” taxonomy (e.g., [[GPT:EXPERTS]], [[GPT:KNOWLEDGE_EXPERTS]]) that can be invoked in prompts to:
- Select the right expert lenses for a task (review, critique, planning, synthesis).
- Standardize names, IDs, and tags so prompts stay consistent across chats and GPTs.
- Reduce ambiguity by mapping plain-language labels (“Data Scientist”) to stable, canonical handles.

## Features
- **Stable identifiers:** Each expert grouping has an `ID` for durable referencing.
- **Canonical tags + aliases:** Each grouping includes `TAGS` (namespaced + optional aliases) for easy prompt invocation.
- **Index for discoverability:** Human-friendly names map to IDs/tags for quick lookup.
- **Composable expert sets:** Supports combining expert groups (e.g., [[GPT:EXPERTS]] + [[GPT:KNOWLEDGE_EXPERTS]]) with relationship rules (e.g., “Requires”).
- **Maintenance-friendly structure:** Clear sections (Context → Index → Definitions) for scalable additions.

## Scope
This file covers:
- Expert *roles/lenses* used to evaluate or produce work in ChatGPT/custom GPT contexts.
- Definitions of expert groupings (general and specialized) and how they relate (subset/requirement relationships).
- Naming conventions via IDs and tags for prompt reliability.

## Out of Scope
- Verifying real-world credentials, licensing, or identity of experts.
- Hiring guidance, HR policy, or legal/medical/professional advice beyond “review lens” framing.
- Detailed methodologies or step-by-step playbooks for each domain (those belong in separate knowledge files).

## Use Cases
- **Prompting consistency:** “Use [[GPT:EXPERTS]] to evaluate this spec for risks, clarity, and completeness.”
- **Role-based reviews:** Generate multi-lens critiques (product, data, compliance, UX research, etc.) using a consistent roster.
- **Knowledge-file evaluation:** Use [[GPT:KNOWLEDGE_EXPERTS]] to assess knowledge-file structure, retrieval ergonomics, and maintenance quality.
- **Governance and safety checks:** Invoke governance/compliance/security lenses for policy alignment and risk spotting.
- **Reusable team presets:** Define standardized expert sets for an organization’s common workflows (docs review, model eval, research synthesis).

# Relevant Context

## Index

Common human topic references mapped to canonical handles (i.e., IDs and namespaced tags). Use canonical tags in prompts (e.g., [[HUMANITY:RESOURCES]]).
- GPT Experts (General) → GPT.EXPERTS → [[GPT:EXPERTS]]
- GPT Knowledge Experts → GPT.EXPERTS.KNOWLEDGE → [[GPT:KNOWLEDGE_EXPERTS]]

## GPT

### Experts (General)

ID: GPT.EXPERTS
TAGS: [[GPT:EXPERTS]] [[GPT_EXPERTS]]

Experts that most comprehensively and most frequently study, analyze, evaluate, refine, and apply ChatGPTs and custom GPTs (e.g., use cases, features, prompts, results). Experts include, but are not limited to, the following:
- Product, Strategy, and Applied Use Experts
  - Prompt Engineers
  - AI Product Managers
  - Technical Product Managers
  - Applied AI Specialists / Solutions Architects
- Data, Training, and Optimization Experts
  - Data Scientists
  - Data Engineers
  - Training Infrastructure Engineers
- AI Research and Model Development Experts
  - Artificial Intelligence Researchers
  - Machine Learning Scientists
  - Computational Linguists
  - Applied Research Scientists
- Governance, Safety, and Ethics Experts
  - AI Safety Researchers
  - Responsible AI Specialists
  - AI Ethicists
  - Trust and Safety Analysts
- Business, Workforce, and Organizational Experts
  - Management Scientists
  - Industrial-Organizational Psychologists
  - Workforce Development Specialists
- Education, Enablement, and Knowledge Translation Experts
  - AI Trainers and Curriculum Developers
  - Technical Evangelists / Developer Advocates
  - Instructional Designers
- AI Engineering and Systems Implementation Experts
  - Machine Learning Engineers
  - AI Engineers
  - Software Engineers
  - MLOps Engineers
- Human-Centered and Evaluation Experts
  - AI Evaluation Scientists
  - Human-Computer Interaction Researchers
  - UX Researchers
  - Cognitive Scientists

#### Knowledge Experts

ID: GPT.EXPERTS.KNOWLEDGE
TAGS: [[GPT:KNOWLEDGE_EXPERTS]] [[GPT_KNOWLEDGE_EXPERTS]]

Experts that most comprehensively and most frequently study, analyze, evaluate, refine, and apply knowledge files uploaded to ChatGPT and custom GPTs (e.g., instructions, roles, knowledge, capabilities, policies). Must use with [[GPT:EXPERTS]]. Experts include, but are not limited to, the following:
- Data, Knowledge, and Information Management Experts
  - Knowledge Engineers
  - Information Architects
- AI Model Development Experts
  - AI Research Scientists
  - Applied Machine Learning Scientists
  - NLP Scientists
- Governance, Risk, and Quality Experts
  - Model Risk Management Analysts
  - Compliance and Privacy Analysts
