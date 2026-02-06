# Global GPT Knowledge File Policies (meta/kf-policies.md)

## File Header

### Domain
GPT.KNOWLEDGE.FILE.POLICIES

### Version
2026-02-06 00:00 UTC

### Author
[Lance Hegland](mailto:lance.hegland@gmail.com)

### Purpose
Identify **relevant context (knowledge)** entries for **GPT knowledge file policies**, a commonly used GPT domain topic. **Domain context entries** in knowledge files give a GPT structured, authoritative background about a commonly used domain topic (a knowledge field) so it can reason *as if it understands the domain’s rules, language, and priorities*. Subsequently, the GPT can offer results that are intentionally more accurate, relevant, specific, clear, practical, fair, and efficient.

### Features
TBD

### Scope
TBD

### Out of Scope
TBD

### Use Cases
TBD

### Policies
See [[KF_POLICIES:ROOT]].


## Index
Bulleted list of common human topic references mapped to canonical handles (i.e., IDs and namespaced tags). Use canonical tags (not tag aliases) in prompts (e.g., [[KF_POLICIES:NAMING_TAGS]]).
- Global Knowledge File Policies → KF_POLICIES → [[KF_POLICIES:ROOT]]
- Tag Policies → KF_POLICIES.TAGS → [[KF_POLICIES:TAGS]]
- Canonical Tag Policies → KF_POLICIES.TAGS.CANONICAL → [[KF_POLICIES:TAGS_CANONICAL]]
- Tag Alias Policies → KF_POLICIES.TAGS.ALIASES → [[KF_POLICIES:TAG_ALIASES]]
- Tag Naming Convention Policies → KF_POLICIES.TAGS.NAMING → [[KF_POLICIES:TAG_NAMING]]
- Tag Governance Policies → KF_POLICIES.TAGS.GOVERNANCE → [[KF_POLICIES:TAG_GOVERNANCE]]
- Schema → KF_POLICIES.SCHEMA → [[KF_POLICIES:SCHEMA]]
- Required Fields → KF_POLICIES.SCHEMA.FIELDS.REQUIRED → [[KF_POLICIES:FIELDS_REQUIRED]]
- Content Fields → KF_POLICIES.SCHEMA.FIELDS.CONTENT → [[KF_POLICIES:FIELDS_CONTENT]]
- Relationship / Composition Fields → KF_POLICIES.SCHEMA.FIELDS.RELATIONSHIP → [[KF_POLICIES:FIELDS_RELATIONSHIP]]
- GPT Prompt Use Examples Field → KF_POLICIES.SCHEMA.FIELDS.EXAMPLES → [[KF_POLICIES:FIELDS_EXAMPLES]]
- Maintenance Metadata Fields → KF_POLICIES.SCHEMA.FIELDS.MAINTENANCE → [[KF_POLICIES:FIELDS_MAINTENANCE]]
- Schema Templates (Copyable/Pasteable) → KF_POLICIES.SCHEMA.TEMPLATES → [[KF_POLICIES:SCHEMA_TEMPLATES]]


## Knowledge Entries (Relevant Context)
The sections below identify **relevant context (knowledge)** entries for a commonly used GPT domain topic. **Domain context entries** in knowledge files, like this one, give GPT structured, authoritative background about a specific knowledge field (domain) so it can reason *as if it understands the domain’s rules, language, and priorities*. These entries help improve results as follows:
- **Accuracy**: They anchor responses to **domain-approved facts, definitions, constraints, and assumptions**, reducing hallucinations and factual drift.
- **Relevance**: They define **what matters in the domain** (goals, stakeholders, common problems), so GPT filters out generic or irrelevant information.
- **Specificity**: They supply **domain terminology, edge cases, workflows, and examples**, enabling precise answers instead of high-level generalities.
- **Clarity**: They establish **shared context and vocabulary**, allowing GPT to explain concepts at the right abstraction level without over- or under-explaining.
- **Practicality**: They encode **real-world constraints, best practices, and decision criteria**, guiding GPT toward actionable, usable outputs.
- **Fairness**: They surface **domain norms, ethical considerations, regulatory boundaries, and stakeholder perspectives**, helping avoid biased or one-sided responses.
- **Efficiency**: They reduce the need for back-and-forth clarification by **pre-answering contextual questions**, enabling faster, more direct responses.

**In short:** Domain context entries function like a *professional briefing* for GPT—aligning its reasoning with how experts in that domain actually think and work.


### Global Knowledge File Policies
**ID:** KF_POLICIES
**Tag:** [[KF_POLICIES:ROOT]]

**Global knowledge file policies** are identified within the following sections. This domain is a subdomain of GPT.KNOWLEDGE.FILE.POLICIES


#### GPT Knowledge File Types
**ID:** KF_POLICIES.TYPES
**Tag:** [[KF_POLICIES:TYPES]]

**GPT Knowledge File Types** are identified as follows:
- **Meta** applies throughout the GPT at all times, governing behavior across tasks, experts, domains, personas, and examples.
- **Tasks** are defined as objectives with specific individual steps (workflows).
Sometimes, the workflow can be performed by using the same **Expert** and the same **Domain** knowledge. Sometimes, one or more of the workflow's individual steps may be best performed using a different **Expert** and a different **Domain**. Sometimes, more complex **Tasks** may reuse the same workflow from less complex **Tasks**. In other words, **Tasks**, **Experts**, and **Domains** are independent and may be interchangeable. One or more workflow steps may be configured using a variety of distinct parameters, as follows:
  - **Experts** (unique, independent, and reusable capability set)
  - **Domains** (unique, independent, and reusable knowledge set)
- **Personas** present results of **Tasks** using specified structures and specified styles. Usually, a **Task** is presented by a single **Persona** using a specified structure and specified style. Rarely, the results of one or more individual steps of a task might be presented using different styles or structures.



#### Tag Policies
**ID:** KF_POLICIES.TAGS
**Tag:** [[KF_POLICIES:TAGS]]

**Tag policies** are identified within the following sections.


##### Canonical Tag Policies
**ID:** KF_POLICIES.TAGS.CANONICAL
**Tag:** [[KF_POLICIES:TAGS_CANONICAL]]

**Canonical tag policies** are as follows:
- **Format:** `[[KF_POLICIES:<NAME>]]` (namespaced, all-caps preferred for stability).
  - Example: `[[KF_POLICIES:TAGS]]`, `[[KF_POLICIES:NAMING_TAGS]]`
- **Purpose:** The canonical tag is the *primary* reference used in prompts, docs, and cross-file linking.
- **Uniqueness:** One canonical tag per definition. Canonical tags must be globally unique within the knowledge set.
- **Stability:** Canonical tags are treated as stable API-like identifiers and should almost never change once published.
- **Display Name Alignment:** Canonical tag name should match the definition title closely (avoid synonyms unless the canonical form is already established).


##### Tag Alias Policies
**ID:** KF_POLICIES.TAGS.ALIASES
**Tag:** [[KF_POLICIES:TAG_ALIASES]]
**Aliases:** [[TAG_SYNONYMS]]

**Alias tag policies** are as follows:
- **Format:** `[[<ALIAS>]]` (shorter/legacy-friendly; may use underscores), e.g. `[[NAMING_CONVENTIONS]]`
- **Purpose:** Provide backwards compatibility and capture common alternate spellings.
- **Limits:** Prefer **0–3 aliases** per definition. Fewer is better.
- **Non-authoritative:** Aliases should never introduce new meaning; they must be strict synonyms of the canonical tag.
- **Deprecation:** If an alias is being phased out, keep it listed but mark it:
  - Example: `**Aliases (deprecated)**: [[OLD_TAG]]` + add a note “Use [[KF_POLICIES:NEW_TAG]] instead.”


##### Tag Naming Convention Policies
**ID:** KF_POLICIES.TAGS.NAMING
**Tag:** [[KF_POLICIES:TAG_NAMING]]

**Tag naming convention policies** are as follows:
- **Case:** Prefer uppercase for the canonical `<NAME>` segment (e.g., `TAGS`) for readability and to avoid drift.
- **Separators:** Prefer underscores in multiword names (`TAG_NAMING`), avoid spaces.
- **Avoid collisions:** Do not create tags that are easy to confuse (e.g., `[[KF_POLICIES:PROS]]` vs `[[KF_POLICIES:KNOWLEDGE_EXPERTS]]`) unless there’s a clear hierarchy.


##### Tag Governance Policies
**ID:** KF_POLICIES.TAGS.GOVERNANCE
**Tag:** [[KF_POLICIES:TAG_GOVERNANCE]]

**Tag governance policies** are as follows:
- **Adding a new tag requires:**
  - a unique `ID`,
  - exactly one canonical tag,
  - a short definition,
  - index entry mapping a human label → canonical tag.
- **Changing canonical tags:** Only if absolutely necessary; when changed, keep the old canonical as an alias (deprecated) and update the Index.
  - Example: `**Aliases (deprecated)**: [[OLD_TAG]] — Use [[NEW_TAG]] instead.`


#### Schema
**ID:** KF_POLICIES.SCHEMA
**Tag:** [[KF_POLICIES:SCHEMA]]

**Schema** for knowledge definition entries are identified in the following sections. Use this schema for every definition entry to keep IDs/tags consistent, enable composability, and reduce drift.


##### Required Fields
**ID:** KF_POLICIES.SCHEMA.FIELDS.REQUIRED
**Tag:** [[KF_POLICIES:FIELDS_REQUIRED]]

**Required fields** for knowledge definition entries are as follows:
- **Title:** Human-readable label for the definition (e.g., "Required Fields").
- **ID:** Stable, unique identifier (dot-delimited) (e.g., `KF_POLICIES.SCHEMA.FIELDS.REQUIRED`).
- **Canonical Tag:** Namespaced tag used as the primary reference in prompts (e.g., `[[KF_POLICIES:FIELDS_REQUIRED]]`).
- **Aliases:** Optional synonym tags for compatibility and common variants (0–3 preferred) (e.g., `[[KF_POLICIES:FIELDS_NEEDED]]`, `[[KF_POLICIES:ESSENTIAL_FIELDS]]`).
- **Summary:** 1–3 sentences describing what this definition invokes and when to use it.


##### Content Fields
**ID:** KF_POLICIES.SCHEMA.FIELDS.CONTENT
**Tag:** [[KF_POLICIES:FIELDS_CONTENT]]

**Content fields** for knowledge definition entries are as follows:
- **Various Domain Specific Fields:** Field labels and values depend on content type, as follows:
  - **MetaFiles**
    - **Policies:** Structured bullet list of rules/policies (grouped where helpful), if not identified in following subsections.
  - **Roles Files** 
    - **Roles:** Structured bullet list of included expert roles (grouped where helpful) to identify their perspectives and capabilities.
  - **Domain Files**
    - **Elements**: Structured bullet list of critical elements or key points (grouped where helpful) to help understand the domain definition.
- **Best For (Use Cases):** 3–6 bullets describing recommended uses.
- **Not For (Anti-Use Cases):** 2–5 bullets describing misuse or non-goals.
- **Inputs Expected:** What the user should provide for high-quality output.
- **Outputs (Default Deliverables):** What the assistant should produce by default when invoked.
- **Quality Bar / Evaluation Criteria:** What “good” looks like (measurable or checkable criteria).
- **Safety / Compliance Notes:** Any constraints or special handling, including avoiding credential claims.


##### Relationship / Composition Fields
**ID:** KF_POLICIES.SCHEMA.FIELDS.RELATIONSHIP
**Tag:** [[KF_POLICIES:FIELDS_RELATIONSHIP]]

**Relationship and composition fields** for knowledge definition entries are as follows:
- **Requires:** Tags that must also be invoked (or `None`).
- **Compatible With:** Tags that pair well (or `None`).
- **Conflicts With:** Tags that should not be combined (or `None`).
- **Overlaps With:** Tags with partial overlap (warn to avoid redundancy) (or `None`).
- **Supersedes:** Prior tags/definitions this replaces (or `None`).
- **Superseded By:** Replacement tag if this is deprecated (or `None`).


##### GPT Prompt Use Examples Field
**ID:** KF_POLICIES.SCHEMA.FIELDS.EXAMPLES
**Tag:** [[KF_POLICIES:FIELDS_EXAMPLES]]

**Use Case Examples:** 1–3 bullets with short prompt examples showing correct invocation and composition of the definition.


##### Maintenance Metadata Fields
**ID:** KF_POLICIES.SCHEMA.FIELDS.MAINTENANCE
**Tag:** [[KF_POLICIES:FIELDS_MAINTENANCE]]

**Maintenance metadata fields** for knowledge definition entries are as follows:
- **Last Reviewed:** UTC timestamp plus identity and contact information for last reviewer. (e.g., `2026-02-06 04:57 UTC — [Lance Hegland](mailto:lance.hegland@gmail.com)`).
- **Owner:** Identity and contact information for person responsible for maintaining the definition entry (e.g., `[Lance Hegland](mailto:lance.hegland@gmail.com)`).
- **Changelog:** Bulleted list of UTC timestamps, identity and contact information for editor, plus description of changes. (e.g., `- 2026-02-06 05:02 UTC — [Lance Hegland](mailto:lance.hegland@gmail.com) — added changelog field to schema maintenance metadata fields`).


##### Schema Templates (Copyable/Pasteable)
**ID:** KF_POLICIES.SCHEMA.TEMPLATES
**Tag:** [[KF_POLICIES:SCHEMA_TEMPLATES]]

**Schema Templates** that are copyable and pasteable for various types of definition entries are included below:
- **For Roles**
```
#### <Title> (for Roles)
**ID:** <ID>
**Tag:** [[GPT:<NAME>]]
**Aliases:** [[<ALIAS_1>]] [[<ALIAS_2>]] (optional)

**Summary:** <1–3 sentences>

**Included Roles:**
- <group>
  - <role>
  - <role>

**Requires:** <tags or None>
**Compatible With:** <tags or None>
**Conflicts With:** <tags or None>
**Overlaps With:** <tags or None>
**Supersedes:** <tags or None>
**Superseded By:** <tags or None>

**Best For (Use Cases):**
- <bullet>
- <bullet>

**Not For (Anti-Use Cases):**
- <bullet>
- <bullet>

**Inputs Expected:**
- <bullet>
- <bullet>

**Outputs (Default Deliverables):**
- <bullet>
- <bullet>

**Quality Bar / Evaluation Criteria:**
- <bullet>
- <bullet>

**Safety / Compliance Notes:**
- <bullet or None>

**Examples:**
- "<prompt example 1>"
- "<prompt example 2>"

**Last Reviewed:** yyyy-mm-dd HH:mm UTC by [<full name>](mailto:<email_address>)

**Owner:** [<full name>](mailto:<email_address>)

**Changelog:**
- yyyy-mm-dd HH:mm UTC [<full name>](mailto:<email_address>): <description>
- yyyy-mm-dd HH:mm UTC [<full name>](mailto:<email_address>): <description>
```
