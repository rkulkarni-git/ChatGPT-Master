# ChatGPT-Master
Centralized control repository for ChatGPT and Codex workflows including instructions, skills, and project-based script versioning.

Author - Rohit Kulkarni

# ChatGPT Master Repository

## Purpose

This repository acts as a centralized control plane for:

* ChatGPT instruction sets
* Codex (Copilot) project workflows
* Script versioning and structured knowledge management

---

## Repository Structure

```
ChatGPT/
│
├── Instructions/
│   ├── Coding/
│   └── Responses/
│
├── Skills/
│   └── Documentation/
│       ├── FileFormats/
│       └── Formatting/
│
└── Codex/
    └── Projects/
        └── Project-<Name>/
            ├── Scripts/
            │   ├── PowerShell/
            │   └── Python/
            │
            └── Documents/
                ├── SOP/
                ├── FAQ/
                ├── KB/
                └── ChangeLog/
```

---

## Version Control Strategy

* Each project maintains independent versioning
* Script updates must be committed with clear version tags
* ChangeLog must be updated for every change

---

## Usage Model

* ChatGPT: Uses Instructions and Skills as reference (manual input)
* Codex (Copilot): Reads active project files from VS Code
* GitHub: Source of truth for all artifacts

---

## Governance Rules

* No direct changes in production scripts without version update
* Maintain separation between Scripts and Documentation
* Always test scripts in controlled environment before commit

---

## Metadata

* Version: v1.0
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27
