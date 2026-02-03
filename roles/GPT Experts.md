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

## Tag Policy (Canonical vs Alias Rules)

### Canonical Tags
- **Format:** `[[GPT:<NAME>]]` (namespaced, all-caps preferred for stability).
  - Example: `[[GPT:EXPERTS]]`, `[[GPT:KNOWLEDGE_EXPERTS]]`
- **Purpose:** The canonical tag is the *primary* reference used in prompts, docs, and cross-file linking.
- **Uniqueness:** One canonical tag per definition. Canonical tags must be globally unique within the knowledge set.
- **Stability:** Canonical tags are treated as stable API-like identifiers and should almost never change once published.
- **Display Name Alignment:** Canonical tag name should match the definition title closely (avoid synonyms unless the canonical form is already established).

### Alias Tags
- **Format:** `[[<ALIAS>]]` (shorter/legacy-friendly; may use underscores), e.g. `[[GPT_EXPERTS]]`
- **Purpose:** Provide backwards compatibility and capture common alternate spellings.
- **Limits:** Prefer **0–3 aliases** per definition. Fewer is better.
- **Non-authoritative:** Aliases should never introduce new meaning; they must be strict synonyms of the canonical tag.
- **Deprecation:** If an alias is being phased out, keep it listed but mark it:
  - Example: `Aliases (deprecated): [[OLD_TAG]]` + add a note “Use [[GPT:EXPERTS]] instead.”

### Naming Conventions
- **Case:** Prefer uppercase for the canonical `<NAME>` segment (e.g., `EXPERTS`, `KNOWLEDGE_EXPERTS`) for readability and to avoid drift.
- **Separators:** Prefer underscores in multiword names (`KNOWLEDGE_EXPERTS`), avoid spaces.
- **Avoid collisions:** Do not create tags that are easy to confuse (e.g., `[[GPT:KNOWLEDGE]]` vs `[[GPT:KNOWLEDGE_EXPERTS]]`) unless there’s a clear hierarchy.

### Governance Rules
- **Adding a new tag requires:**
  - a unique `ID`,
  - exactly one canonical tag,
  - a short definition,
  - index entry mapping a human label → canonical tag.
- **Changing canonical tags:** Only if absolutely necessary; when changed, keep the old canonical as an alias (deprecated) and update the Index.

## Definition Schema

Use this schema for every definition entry to keep IDs/tags consistent, enable composability, and reduce drift.

### Required Fields
- **Title:** Human-readable label for the definition.
- **ID:** Stable identifier (dot-delimited).  
  - Example: `GPT.EXPERTS`, `GPT.EXPERTS.KNOWLEDGE`
- **Canonical Tag:** Namespaced tag used as the primary reference in prompts.  
  - Format: `[[GPT:<NAME>]]`
- **Aliases:** Optional synonym tags for compatibility and common variants (0–3 preferred).  
  - Example: `[[GPT_EXPERTS]]`
- **Summary:** 1–3 sentences describing what this definition invokes and when to use it.

### Content Fields
- **Included Roles:** Structured bullet list of included expert lenses/roles (grouped where helpful).
- **Best For (Use Cases):** 3–6 bullets describing recommended uses.
- **Not For (Anti-Use Cases):** 2–5 bullets describing misuse or non-goals.
- **Inputs Expected:** What the user should provide for high-quality output.
- **Outputs (Default Deliverables):** What the assistant should produce by default when invoked.
- **Quality Bar / Evaluation Criteria:** What “good” looks like (measurable or checkable criteria).
- **Safety / Compliance Notes:** Any constraints or special handling, including avoiding credential claims.

### Relationship / Composition Fields
- **Requires:** Tags that must also be invoked (or `None`).
- **Compatible With:** Tags that pair well (or `None`).
- **Conflicts With:** Tags that should not be combined (or `None`).
- **Overlaps With:** Tags with partial overlap (warn to avoid redundancy) (or `None`).
- **Supersedes:** Prior tags/definitions this replaces (or `None`).
- **Superseded By:** Replacement tag if this is deprecated (or `None`).

### Examples
- **Examples:** 1–3 short prompt examples showing correct invocation and composition.

### Maintenance  himMetadata
**Changelog:** None
**Owner:** Lance Hegland (lance.hegland@gmail.com)
**Last Reviewed:** 2026-02-02 06:02 UTC by Lance Hegland

### Copy/Paste Template

#### <Title>
ID: <ID>  
Canonical Tag: [[GPT:<NAME>]]  
Aliases: [[<ALIAS_1>]] [[<ALIAS_2>]] (optional)

Summary:
- <1–3 sentences>

Included Lenses / Roles:
- <group>
  - <role>
  - <role>

Requires: <tags or None>  
Compatible With: <tags or None>  
Conflicts With: <tags or None>  
Overlaps With: <tags or None>  
Supersedes: <tags or None>  
Superseded By: <tags or None>

Best For (Use Cases):
- <bullet>
- <bullet>

Not For (Anti-Use Cases):
- <bullet>
- <bullet>

Inputs Expected:
- <bullet>
- <bullet>

Outputs (Default Deliverables):
- <bullet>
- <bullet>

Quality Bar / Evaluation Criteria:
- <bullet>
- <bullet>

Safety / Compliance Notes:
- <bullet or None>

Examples:
- "<prompt example 1>"
- "<prompt example 2>"

Changelog: 
Owner:
Last Reviewed:

# Relevant Context

## Index

Common human topic references mapped to canonical handles (i.e., IDs and namespaced tags). Use canonical tags in prompts (e.g., [[GPT:EXPERTS]]).
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

**Changelog:** None
**Owner:** Lance Hegland (lance.hegland@gmail.com)
**Last reviewed:** 2026-02-02 06:02 UTC by Lance Hegland


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
**Overlaps With:** None

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

**Changelog:** None
**Owner:** Lance Hegland (lance.hegland@gmail.com)
**Last reviewed:** 2026-02-02 06:02 UTC by Lance Hegland
