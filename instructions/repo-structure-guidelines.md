## 10. Enterprise Naming Enforcement (STRICT)

### 10.1 Case Sensitivity Model

| Component               | Format           | Example                     |
| ----------------------- | ---------------- | --------------------------- |
| Root folders            | PascalCase       | Codex, Skills, Instructions |
| Project folders         | lowercase-hyphen | dc-migration                |
| Subfolders              | PascalCase       | Scripts, Documents          |
| Script language folders | PascalCase       | PowerShell, Python          |
| Special folders         | PascalCase       | Artifacts, ChangeLog        |

---

### 10.2 Naming Consistency Rules

* Must be deterministic (no variation allowed)

* No mixed casing:
  ❌ powershell / Powershell
  ✔️ PowerShell

* No abbreviations unless standardized:
  ❌ docs
  ✔️ Documents

* No spaces:
  ❌ DC Migration
  ✔️ dc-migration

---

### 10.3 Reserved Folder Names (MANDATORY)

```text
Instructions
Skills
Codex
Projects
Scripts
Documents
Artifacts
SOP
FAQ
KB
ChangeLog
PowerShell
Python
```

---

### 10.4 File Naming Enforcement

#### SOP Files

```text
<topic>-sop.md
<topic>-sop-changelog.md
```

#### Scripts

```text
<action>-<target>-<purpose>-vX.X.<ext>
```

Examples:

```text
get-azure-vm-inventory-v1.0.ps1
invoke-dc-migration-validation-v1.1.py
```

---

### 10.5 Versioning Enforcement

* Version must be in filename (not only folder)
* Version format:

```text
v1.0, v1.1, v2.0
```

---

### 10.6 Structural Integrity Rules

* No files directly under project root
* Scripts must ONLY exist under:

```text
Scripts/<Language>/
```

* SOPs must ONLY exist under:

```text
Documents/SOP/
```

---

### 10.7 Enforcement Model

Violations must be corrected immediately:

* rename
* restructure
* recommit

No exceptions

---

### Metadata (Updated)

* Version: v1.1
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27
