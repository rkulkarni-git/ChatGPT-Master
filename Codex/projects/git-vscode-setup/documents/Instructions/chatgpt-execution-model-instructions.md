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
