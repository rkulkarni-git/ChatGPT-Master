# SOP: SOP Authoring Framework (Reusable Skill)

## Objective

Define a standardized, enterprise-grade framework to create SOP documents with:

* clarity
* consistency
* version control
* visual-first design
* Git integration

---

## Scope

Applicable for:

* ChatGPT / Codex / Claude workflows
* Infrastructure, automation, and engineering processes
* L1 to L4 engineering audiences

---

## Audience Design

| Level | Requirement                          |
| ----- | ------------------------------------ |
| L1    | Step-by-step clarity                 |
| L2    | Operational understanding            |
| L3    | Technical depth                      |
| L4    | Architectural and governance insight |

---

## Core Principles

1. No preamble — direct execution
2. One step at a time
3. Mandatory validation before proceeding
4. Visual-first (screenshots required)
5. Version-controlled artifacts
6. Git as source of truth

---

## Naming Convention (MANDATORY)

```text
<topic>-sop.md
<topic>-sop-changelog.md
```

Rules:

* lowercase only
* hyphen-separated
* no spaces

---

## Standard Document Framework

1. Objective
2. Scope
3. Prerequisites
4. Steps
5. Validation
6. Visualization
7. Final Structure
8. Governance
9. Metadata

---

## Step Construction Standard

### Step X — <Title>

**Command**

```powershell
<command>
```

**Expected Output**

```text
<output>
```

📸 Screenshot:
[Mandatory — CLI or UI capture]

---

## Validation Standard

```text
Reply with:
- success confirmation
OR
- exact error output
```

---

## Visualization Standard

* Every command → screenshot
* Every UI action → screenshot
* If not available → placeholder

Example:

```text
📸 Insert screenshot of PowerShell output
```

---

## Version Control Model

### Inside SOP

* Maintain version in Metadata
* Update on every change

### External ChangeLog

* Track all updates
* Maintain history (no overwrite)

---

## Change Management Rules

* v1.0 → initial release
* v1.x → incremental improvements
* v2.0 → major structural changes

---

## Git Integration Workflow

```powershell
git add .
git commit -m "SOP vX.X - <summary>"
git push origin main
```

---

## Artifact Rule (CRITICAL)

Every prompt-driven output MUST produce:

* SOP document
* ChangeLog document

No exceptions

---

## Governance

* No execution without validation
* No production use without testing
* Maintain separation:

  * Instructions
  * Skills
  * Projects

---

## Quality Checklist

* [ ] Clear steps
* [ ] Commands validated
* [ ] Screenshots included
* [ ] Naming correct
* [ ] Version updated
* [ ] ChangeLog updated

---

## Metadata

* Version: v1.0
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27
