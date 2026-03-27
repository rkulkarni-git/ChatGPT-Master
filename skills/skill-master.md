# Skill: Master Framework (Skills Registry & Control Plane)

---

## 1. Objective

Act as the **central registry and control layer** for all skills.

Defines:

* what skills exist
* how they are structured
* how they are used
* how they evolve

---

## 2. Scope

Covers ALL skills:

* Documentation Skills:

  * SOP
  * FAQ
  * KB
  * Artifact

* Engineering Skills:

  * PowerShell (script build, testing, validation)
  * Python (script build, testing, validation)

* Future skills

---

## 3. Skills Architecture

```text
Skills/
├── Documentation/
│   ├── SOP/
│   ├── FAQ/
│   ├── KB/
│   └── Artifacts/
│
├── PowerShell/
└── Python/
```

---

## 4. Skill Registry (MANDATORY)

### 4.1 Documentation Skills

| Skill    | Purpose               | Framework               |
| -------- | --------------------- | ----------------------- |
| SOP      | procedural execution  | step-based + validation |
| FAQ      | Q&A format            | concise answers         |
| KB       | knowledge explanation | conceptual              |
| Artifact | full conversation log | append-only             |

---

### 4.2 Engineering Skills

| Skill      | Purpose                         |
| ---------- | ------------------------------- |
| PowerShell | script creation, automation     |
| Python     | scripting, API, data processing |

---

## 5. Skill Creation Standard

Every skill MUST include:

```text
<skill-name>.md
<skill-name>-changelog.md
```

---

## 6. Skill Classification Rules

| Category      | Behavior          |
| ------------- | ----------------- |
| Documentation | structured output |
| Engineering   | executable output |

---

## 7. Skill Usage Model

```text
Instructions → WHEN to use
Skills → HOW to execute
Projects → WHERE applied
Chats → WHERE triggered
```

---

## 8. Skill Invocation Rules

* Skills are triggered implicitly by context
* Must follow Instructions first
* Must NOT override Instructions

---

## 9. Skill Separation (CRITICAL)

| Type     | Must NOT do                     |
| -------- | ------------------------------- |
| SOP      | no Q&A, no knowledge dump       |
| FAQ      | no procedures                   |
| KB       | no steps                        |
| Artifact | no formatting, no summarization |

---

## 10. Artifact Special Rule

Artifact is NOT documentation.

* Raw conversation only
* Append-only
* No transformation

---

## 11. Skill Lifecycle

```text
Create → Use → Update → Version → Track (Changelog)
```

---

## 12. Version Control

* Every update increments version
* Must update changelog
* No overwrite of previous logic without tracking

---

## 13. Governance

* Skills are reusable assets
* Must remain generic
* Must not contain project-specific data
* Must follow naming standards

---

## 14. Metadata

* Version: v1.1
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27

