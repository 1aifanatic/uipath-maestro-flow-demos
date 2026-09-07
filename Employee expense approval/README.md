# Employee Expense Approval — Maestro Flow (Part 1)

This project contains the complete solution source and video walkthrough for the **Employee Expense Approval** demo built using **UiPath Maestro Flow**, the **UiPath CLI**, and **Claude Code**.

🎥 **Watch the Part 1 Video**: [Download / Stream Video (MP4, 1440p 60fps)](https://github.com/1aifanatic/uipath-maestro-flow-demos/releases/download/v1.0.0/Maestro_Flow_Employee_Expense_Approval_Part1.mp4)

---

## 🎯 What this Demo Covers (Part 1)

In Part 1, we cover the full journey from initial architecture down to automated code scaffolding and publishing to Studio Web:

1. **The Architectural Blueprint**:
   - Why traditional monolithic automation fails for human-in-the-loop workflows.
   - Decoupling decision logic into declarative orchestration.
2. **Business Tier Rules**:
   - **Tier 1 (< $100)**: Instant auto-approval, automated ledger logging, and employee notification.
   - **Tier 2 ($100 – $500)**: Manager approval task via Action Center / email notification.
   - **Tier 3 (> $500)**: Senior Finance review with audit documentation attachment.
3. **Developer CLI Setup**:
   - Installing the official UiPath CLI (`uipath-cli/install.ps1`).
   - Logging in via OAuth to Orchestrator (`aifanatic / DefaultTenant`).
4. **Agentic Scaffolding with Claude Code**:
   - Running Claude Code with the `/uipath:uipath-maestro-flow` skill.
   - Generating 8 nodes, 8 edges, and 15 variables in `EmployeeExpenseApproval.flow` and `bindings_v2.json`.
   - Running full JSON validation and packaging.
5. **Publishing to Studio Web**:
   - Running `uip solution upload .` to synchronize the local solution into UiPath Studio Web.
   - Inspecting the resulting canvas and nodes in the browser.

---

## 🔜 Part 2 — Coming Soon!

In **Part 2**, we will cover:
- Connecting the dots with Integration Service connectors.
- Binding runtime data inputs from forms and enterprise sources.
- Configuring Action Center task forms for managers and finance teams.
- End-to-end execution, debugging, and live publishing of the Maestro Flow!

**Stay tuned!**

---

## 📂 Project Structure

```text
Employee expense approval/
├── EmployeeExpenseApproval/
│   ├── EmployeeExpenseApproval.uipx             # Solution manifest
│   ├── AGENTS.md                                # Instructions for coding agents
│   ├── CLAUDE.md                                # Instructions for Claude Code
│   ├── EmployeeExpenseApproval/                 # Flow project folder
│   │   ├── EmployeeExpenseApproval.flow         # Declarative Maestro flow definition
│   │   ├── bindings_v2.json                     # Resource bindings & declarations
│   │   ├── operate.json                         # Execution metadata
│   │   ├── project.uiproj                       # UiPath project definition
│   │   └── evals/                               # Evaluation sets and coverage tests
│   └── resources/                               # Solution folder resources & packages
└── video/
    └── Maestro_Flow_Employee_Expense_Approval_Part1.mp4  # Rendered walkthrough with cloned voice
```

---

## 🚀 How to Run / Replicate Locally

### 1. Install UiPath CLI
```powershell
irm https://download.uipath.com/uipath-cli/install.ps1 | iex
```

### 2. Login to Orchestrator
```powershell
uip login
```

### 3. Validate & Pack Solution
```powershell
cd EmployeeExpenseApproval
uip solution pack . ./out
```

### 4. Upload to Studio Web
```powershell
uip solution upload .
```

Open the printed `DesignerUrl` to inspect and edit your Maestro Flow directly in the cloud!
