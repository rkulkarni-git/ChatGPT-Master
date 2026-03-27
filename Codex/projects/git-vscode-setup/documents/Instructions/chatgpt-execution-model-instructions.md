# Instructions: ChatGPT Execution Model (Project-Specific)

---

## 1. Objective

Define strict execution model for ChatGPT usage within this project to:

* control prompt flow
* enforce discipline
* ensure correct artifact generation
* maintain structured outputs

---

## 2. Chat Segmentation Model (MANDATORY)

Each chat is purpose-specific and isolated.

### Chat Types

| Chat Name         | Purpose                         |
| ----------------- | ------------------------------- |
| brainstorming     | architecture, planning          |
| script build      | script creation                 |
| script testing    | debugging and testing           |
| script validation | final validation                |
| documentation     | SOP, KB, documentation          |
| revision          | context and instruction updates |

---

## 3. Chat Enforcement Rules

### 3.1 Strict Isolation

* Each chat must only handle its defined purpose
* No cross-functional prompts allowed

---

### 3.2 Violation Handling

If incorrect prompt detected:

```text
This prompt belongs to <correct chat>.
Please move this request.
```

Execution must stop immediately.

---

## 4. Execution Discipline

* One objective per prompt
* Step-by-step execution
* Validation required before next step
* No skipping steps

---

## 5. Artifact Generation Rules

Based on SOP framework:

| Task          | Output               |
| ------------- | -------------------- |
| Script build  | script file          |
| Documentation | SOP + ChangeLog      |
| Revision      | updated Instructions |

---

## 6. Context Model

```text
Instructions → control behavior
Skills → define execution
Projects → implementation
Chats → execution channels
```

---

## 7. Revision Model

### 7.1 Default

* Incremental revision only
* Based on last checkpoint

---

### 7.2 First Revision

* Full scan of all chats
* Establish baseline (v1.0)

---

### 7.3 Subsequent Revisions

* Process only new changes
* Increment version

---

### 7.4 Full Revision

Triggered only by:

```text
full revision
```

---

## 8. Governance

* Instructions override all behavior
* No deviation allowed
* All outputs must follow:

  * naming standards
  * structure rules
  * SOP framework

---

## 9. Metadata

* Version: v1.0
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27

---

## 10. Artifact Generation Model (MANDATORY)

### 10.1 Objective

Create a complete, append-only record of all interactions between:

* User prompts
* ChatGPT responses

This serves as:

* contextual history
* audit trail
* knowledge artifact

---

### 10.2 Trigger

Artifact generation is triggered ONLY when user says:

```text
Generate artifact
```

And must be executed in:

```text
documentation chat
```

---

### 10.3 Output Files

Each execution must generate:

```text
artifact.md
artifact-changelog.md
```

Location:

```text
Codex/Projects/<project>/Documents/Artifacts/
```

---

### 10.4 Structure Format (STRICT)

Each entry must follow:

```text
### Entry <number>

User Prompt:
<exact user input>

ChatGPT Response:
<exact response>
```

---

### 10.5 Numbering Rules

* Sequential numbering (no resets)
* Continue from last entry
* Example:

```text
Entry 1 → Entry 2 → Entry 3
```

---

### 10.6 Append-Only Model (CRITICAL)

* No modification of previous entries
* Only append new entries
* No deletion allowed
* No overwrite allowed

---

### 10.7 ChangeLog Rules

Each artifact update must include:

```text
## vX.X - <date>
- Added entries <start> to <end>
```

---

### 10.8 Content Rules (STRICT)

Artifact is a raw interaction log.

Must include:

* Exact user prompts
* Exact ChatGPT responses

Must NOT:

* Use SOP framework
* Summarize content
* Reformat responses
* Optimize structure

Artifact = full conversation preservation

---

### 10.9 Enforcement Rules

* Must be generated only in documentation chat
* Must follow append-only model
* Must maintain numbering integrity

Violation handling:

```text
Artifact generation must be executed in documentation chat.
Please move this request.
```

---

## 11. Governance

* Instructions override all behavior
* No deviation allowed
* All outputs must follow:

  * naming standards
  * structure rules
  * SOP framework
  * artifact model

---

## 12. Metadata

* Version: v1.1
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27

