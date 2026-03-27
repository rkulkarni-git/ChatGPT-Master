# SOP: Setup Codex + VS Code + GitHub Integration

## Objective

Standardize setup for VS Code, GitHub, and Codex (Copilot) with controlled structure and versioning.

---

## Step 1 — Install Git

**Command**

```
winget install --id Git.Git -e --source winget
git --version
```

**Expected Output**

```
git version x.x.x
```

📸 Screenshot Placeholder:
[Insert PowerShell screenshot showing git --version output]

---

## Step 2 — Create GitHub Repository

* Go to https://github.com/new
* Create: `chatgpt-master`
* Add README
* Commit to main

📸 Screenshot Placeholder:
[Insert GitHub repo creation screen]

---

## Step 3 — Install VS Code

**Command**

```
winget install --id Microsoft.VisualStudioCode -e
code --version
```

📸 Screenshot Placeholder:
[Insert VS Code version output]

---

## Step 4 — Clone Repository

**Command**

```
git clone https://github.com/<username>/chatgpt-master.git
cd chatgpt-master
code .
```

📸 Screenshot Placeholder:
[Insert VS Code opened with repo]

---

## Step 5 — Create Structure

**Command**

```
mkdir Instructions, Skills, Codex
mkdir Skills\Documentation\SOP -Force
New-Item Skills\Documentation\SOP\SOP.md -ItemType File
New-Item Skills\Documentation\SOP\SOP-ChangeLog.md -ItemType File
```

📸 Screenshot Placeholder:
[Insert tree /F output]

---

## Final Structure

```
ChatGPT/
├── Instructions/
├── Skills/
│   └── Documentation/
│       └── SOP/
│           ├── SOP.md
│           └── SOP-ChangeLog.md
└── Codex/
```

---

## Governance

* Validate each step before proceeding
* Use version control for all updates
* Do not execute scripts in production without testing

---

## Metadata

* Version: v1.0
* Author: Rohit Kulkarni
* Last Updated: 2026-03-27
