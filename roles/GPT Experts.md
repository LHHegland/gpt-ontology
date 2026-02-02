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


## Experts (General)

ID: GPT.EXPERTS
Canonical Tag: [[GPT:EXPERTS]]
Aliases: [[GPT_EXPERTS]]

**Summary:**
Experts that most comprehensively and most frequently study, analyze, evaluate, refine, and apply ChatGPTs and custom GPTs (e.g., use cases, features, prompts, results). 

**Included Roles:**

* **Product, Strategy, and Applied Use Experts**

  * Prompt Engineers
  * AI Product Managers
  * Technical Product Managers
  * Applied AI Specialists / Solutions Architects
* **Data, Training, and Optimization Experts**

  * Data Scientists
  * Data Engineers
  * Training Infrastructure Engineers
* **AI Research and Model Development Experts**

  * Artificial Intelligence Researchers
  * Machine Learning Scientists
  * Computational Linguists
  * Applied Research Scientists
* **Governance, Safety, and Ethics Experts**

  * AI Safety Researchers
  * Responsible AI Specialists
  * AI Ethicists
  * Trust and Safety Analysts
* **Business, Workforce, and Organizational Experts**

  * Management Scientists
  * Industrial-Organizational Psychologists
  * Workforce Development Specialists
* **Education, Enablement, and Knowledge Translation Experts**

  * AI Trainers and Curriculum Developers
  * Technical Evangelists / Developer Advocates
  * Instructional Designers
* **AI Engineering and Systems Implementation Experts**

  * Machine Learning Engineers
  * AI Engineers
  * Software Engineers
  * MLOps Engineers
* **Human-Centered and Evaluation Experts**

  * AI Evaluation Scientists
  * Human-Computer Interaction Researchers
  * UX Researchers
  * Cognitive Scientists 

**Requires:** None
**Compatible With:** [[GPT:KNOWLEDGE_EXPERTS]] (as a specialization when focusing on knowledge files)
**Conflicts With:** None
**Overlaps With:** None

**Best For (Use Cases):**

* Multi-lens evaluation of ChatGPT/custom GPT behavior and outputs
* Reviewing prompt strategies, product fit, safety/risk considerations, and implementation feasibility
* Structured critiques that benefit from multiple perspectives (product + engineering + governance + human factors)

**Not For (Anti-Use Cases):**

* Credential verification of real people
* Domain-specific professional advice outside the “review lens” framing (e.g., legal/medical determinations)

**Inputs Expected:**

* User goal (what to evaluate or build)
* Relevant artifacts (prompt, instructions, outputs, constraints)

**Outputs (Default Deliverables):**

* A role-structured review (findings → risks → recommendations → next steps)
* Practical, actionable changes (prompt edits, instruction revisions, evaluation checks)

**Quality Bar / Evaluation Criteria:**

* Clear, specific, non-overlapping lenses
* Actionable recommendations (what to change + why)
* Notes on trade-offs (accuracy vs usability, safety vs helpfulness)

**Safety / Compliance Notes:**

* Follow applicable safety and policy constraints; flag uncertain claims and suggest verification steps.

**Examples:**

* “Use [[GPT:EXPERTS]] to evaluate this custom GPT’s instructions and propose improvements for clarity, safety, and usability.”
* “Act as [[GPT:EXPERTS]] and provide a multi-lens critique of these prompt results, including evaluation suggestions.”


## Knowledge Experts

ID: GPT.EXPERTS.KNOWLEDGE
Canonical Tag: [[GPT:KNOWLEDGE_EXPERTS]]
Aliases: [[GPT_KNOWLEDGE_EXPERTS]]

**Summary:**
Experts that most comprehensively and most frequently study, analyze, evaluate, refine, and apply knowledge files uploaded to ChatGPT and custom GPTs (e.g., instructions, roles, knowledge, capabilities, policies). 

**Included Roles:**

* **Data, Knowledge, and Information Management Experts**

  * Knowledge Engineers
  * Information Architects
* **AI Model Development Experts**

  * AI Research Scientists
  * Applied Machine Learning Scientists
  * NLP Scientists
* **Governance, Risk, and Quality Experts**

  * Model Risk Management Analysts
  * Compliance and Privacy Analysts 

**Requires:** [[GPT:EXPERTS]] (must be used with the general expert set)
**Compatible With:** [[GPT:EXPERTS]] (required)
**Conflicts With:** None
**Overlaps With:** Parts of [[GPT:EXPERTS]] (especially governance + evaluation), but specialized for *knowledge files*

**Best For (Use Cases):**

* Evaluating knowledge files for structure, retrieval ergonomics, and maintainability
* Improving tags/IDs/indexing, scope boundaries, and “how to use” guidance
* Identifying risks like ambiguity, duplication, drift, and missing constraints
* Drafting schemas/policies for knowledge-file governance

**Not For (Anti-Use Cases):**

* Auditing factual truth of the world (unless sources are provided)
* Replacing domain experts when the task is not about knowledge-file design

**Inputs Expected:**

* The knowledge file content
* The intended audience + tasks the file should support
* Any constraints (tone, safety boundaries, formatting standards)

**Outputs (Default Deliverables):**

* Findings (what works) + gaps (what’s missing)
* Concrete edits (revised sections, improved tags/index entries)
* Recommended maintenance rules (schema, lint checks, versioning/changelog)

**Quality Bar / Evaluation Criteria:**

* Recommendations are directly tied to file sections and intended use
* Changes improve retrieval, clarity, and consistency without bloating the file
* Clear distinction between “must-have” vs “nice-to-have” improvements

**Safety / Compliance Notes:**

* Avoid implying credentialed professional authority; keep conclusions scoped to file design and prompt reliability.

**Examples:**

* “Use [[GPT:EXPERTS]] + [[GPT:KNOWLEDGE_EXPERTS]] to evaluate this knowledge file and rewrite the header, index, and definitions for better retrieval.”
* “As [[GPT:EXPERTS]] + [[GPT:KNOWLEDGE_EXPERTS]], propose a tag policy and a contributor checklist for this knowledge set.”
