# SOP: Setup Codex + VS Code + GitHub Integration

---

## 1. Objective

Establish a standardized development environment integrating Git, VS Code, GitHub, and Codex (Copilot) with structured repository design and version control.

---

## 2. Scope

Applicable for:

* PowerShell automation
* Python scripting
* Infrastructure projects (Azure, AWS, NOC, etc.)

---

## 3. Prerequisites

* Windows system with PowerShell
* GitHub account
* Internet connectivity
* Administrative access (recommended)

---

## 4. Steps

---

### Step 1 — Install Git

**Command**

```powershell
winget install --id Git.Git -e --source winget
git --version
```

**Expected Output**

```text
git version x.x.x
```

📸 Screenshot
[Insert PowerShell output showing git version]

---

### Step 2 — Create GitHub Repository

* Navigate to https://github.com/new
* Repository name: `chatgpt-master`
* Visibility: Private
* Add README
* Commit to main

📸 Screenshot
[Insert GitHub repository creation screen]

---

### Step 3 — Install VS Code

**Command**

```powershell
winget install --id Microsoft.VisualStudioCode -e
code --version
```

📸 Screenshot
[Insert VS Code version output]

---

### Step 4 — Clone Repository

**Command**

```powershell
git clone https://github.com/<username>/chatgpt-master.git
cd chatgpt-master
code .
```

📸 Screenshot
[Insert VS Code showing repo opened]

---

### Step 5 — Create Base Structure

**Command**

```powershell
mkdir Instructions, Skills, Codex
```

📸 Screenshot
[Insert folder structure in VS Code]

---

### Step 6 — Create SOP Structure

**Command**

```powershell
mkdir Skills\Documentation\SOP -Force
```

📸 Screenshot
[Insert created folder structure]

---

### Step 7 — Create SOP Files

**Command**

```powershell
New-Item Skills\Documentation\SOP\setup-codex-vscode-github-sop.md -ItemType File
New-Item Skills\Documentation\SOP\setup-codex-vscode-github-sop-changelog.md -ItemType File
```

📸 Screenshot
[Insert file creation view]

---

### Step 8 — Add SOP and ChangeLog Content

* Populate SOP with structured steps
* Populate ChangeLog with version history

📸 Screenshot
[Insert file content in VS Code]

---

## 5. Validation

After completion:

```powershell
tree /F
```

**Expected Structure**

```text
chatgpt-master/
├── Instructions/
├── Skills/
│   └── Documentation/
│       └── SOP/
│           ├── setup-codex-vscode-github-sop.md
│           └── setup-codex-vscode-github-sop-changelog.md
└── Codex/
```

---

## 6. Visualization

* All CLI commands must have screenshots
* All UI actions must have screenshots
* Use placeholders if screenshots unavailable

---

## 7. Final Structure

```text
chatgpt-master/
├── Instructions/
├── Skills/
├── Codex/
```

---

## 8. Governance

* Validate each step before proceeding
* Do not execute scripts in production without testing
* Maintain version control for all artifacts
* Follow SOP Authoring Framework strictly

---

## 9. Metadata

* Version: v2.0
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27
