# SOP: Setup Codex + VS Code + GitHub Integration

## Objective

Standardized setup for Git, VS Code, GitHub, and Codex with structured repository design and version control.

---

## Step 1 — Install Git

```powershell
winget install --id Git.Git -e --source winget
git --version
```

Expected:

```
git version x.x.x
```

📸 [Screenshot Required]

---

## Step 2 — Create GitHub Repository

* Create repo: chatgpt-master
* Add README
* Commit to main

📸 [Screenshot Required]

---

## Step 3 — Install VS Code

```powershell
winget install --id Microsoft.VisualStudioCode -e
code --version
```

📸 [Screenshot Required]

---

## Step 4 — Clone Repository

```powershell
git clone https://github.com/<username>/chatgpt-master.git
cd chatgpt-master
code .
```

📸 [Screenshot Required]

---

## Step 5 — Create Base Structure

```powershell
mkdir Instructions, Skills, Codex
```

---

## Step 6 — Create SOP Structure

```powershell
mkdir Skills\Documentation\SOP -Force
```

---

## Step 7 — Create SOP Files

```powershell
New-Item Skills\Documentation\SOP\setup-codex-vscode-github-sop.md -ItemType File
New-Item Skills\Documentation\SOP\setup-codex-vscode-github-sop-changelog.md -ItemType File
```

---

## Step 8 — Add SOP + ChangeLog Content

* SOP.md → full process documentation
* ChangeLog.md → version tracking

---

## Final Structure

```
ChatGPT/
├── Instructions/
├── Skills/
│   └── Documentation/
│       └── SOP/
│           ├── setup-codex-vscode-github-sop.md
│           └── setup-codex-vscode-github-sop-changelog.md
└── Codex/
```

---

## Governance

* Validate each step before proceeding
* Maintain versioning for all updates
* Use GitHub as source of truth

---

## Metadata

* Version: v1.1
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27
