# UiPath Maestro Flow Demos 🚀

A collection of production-ready [UiPath Maestro Flow](https://www.uipath.com/product/maestro) projects, orchestration templates, patterns, and hands-on video walkthroughs.

Curated by **Naveen Chatlapalli** ([@1aifanatic](https://github.com/1aifanatic)).

---

## 📂 Featured Demos

### 1. [Employee Expense Approval](./Employee%20expense%20approval/)

An intelligent, multi-tier expense approval workflow built with UiPath Maestro Flow, CLI automation, and Claude Code scaffolding.

* **Video Walkthrough (Part 1)**: 🎥 [Watch / Download Part 1 Video (MP4)](https://github.com/1aifanatic/uipath-maestro-flow-demos/releases/download/v1.0.0/Maestro_Flow_Employee_Expense_Approval_Part1.mp4)
* **Video Walkthrough (Part 2 — Final)**: 🎥 [Watch / Download Part 2 Video (MP4)](https://github.com/1aifanatic/uipath-maestro-flow-demos/releases/download/v2.0.0/Maestro_Flow_Employee_Expense_Approval_Part2.mp4)
* **Status**: Complete (Part 1 Architecture & CLI Scaffolding + Part 2 Runtime Execution & Action Center).

---

## 🎬 Part 1 Video Overview

The Part 1 video walkthrough demonstrates the developer workflow for scaffolding a Maestro Flow using the UiPath CLI and Claude Code:

| Timestamp | Chapter | Description |
|---|---|---|
| **00:00** | **Maestro Flow Concept** | Why Maestro Flow bridges AI agents, APIs, people, and RPA into one orchestrated canvas |
| **00:18** | **The Business Story** | Solving expense reimbursement bottlenecks and fragmented approvals |
| **00:34** | **Architecture in One Picture** | Multi-tier decision rules: <$100 Auto-approval, $100–$500 Manager approval, >$500 Finance verification |
| **00:50** | **UiPath CLI Setup** | Installing `uipath-cli` via PowerShell and exploring Coding Agents docs |
| **01:30** | **Orchestrator Staging & Login** | Authenticating to `aifanatic / DefaultTenant` and confirming folder context |
| **02:15** | **Claude Code Automation** | Invoking `/uipath:uipath-maestro-flow` to scaffold 8 nodes, 8 edges, and 15 variables |
| **03:40** | **Studio Web Canvas & Part 2 Teaser** | Inspecting the visual canvas in Studio Web and teasing Part 2 runtime bindings |

---

## 🎬 Part 2 Video Overview (Final)

The Part 2 video walkthrough demonstrates the complete runtime execution, inline human-in-the-loop task handling, and Integration Service notification:

| Timestamp | Chapter | Description |
|---|---|---|
| **00:00** | **Studio Web Canvas Walkthrough** | Reviewing the deployed 8-node Maestro Flow layout on the visual canvas |
| **00:15** | **Auto Approve Node & Payload** | Inspecting the JavaScript block formatting the approval payload |
| **00:25** | **Check Auto Approval Threshold** | Examining the `<=$100` condition branching between auto-approval and escalation |
| **00:36** | **Inline Action Center & Multi-Channel** | Deep-dive into inline manager tasks and multi-channel delivery (Slack, Teams, Email, Action Center) |
| **00:57** | **Send Email Activity** | Integration Service Gmail connector binding to dynamic outcome data |
| **01:08** | **HTML Email Template Builder** | Custom responsive card generation with status badges and comments in JavaScript |
| **01:25** | **Live Debug Run 1: $50 Auto-Approve** | Running the flow with an under-threshold expense and verifying green trace |
| **02:05** | **Gmail Verification: Run 1** | Opening the auto-approved HTML email in Gmail with green status badge |
| **02:19** | **Live Debug Run 2: $1,000 Escalation** | Testing policy escalation with high-amount expense |
| **02:45** | **Action Center Task Submission** | Interacting with the inline task, adding comment "Travel reason verified", and approving |
| **03:18** | **Gmail Verification: Run 2** | Inspecting manager-approved email with decision audit trail and comment |
| **03:34** | **Architecture Takeaway** | "Orchestration is the product" — unifying agents, APIs, and people |

---

## 🛠️ Tech Stack & Prerequisites

- **UiPath CLI** (`uip`) v1.200.0+
- **UiPath Studio Web** & **Automation Cloud**
- **UiPath Action Center** (Inline Tasks & Multi-Channel Delivery)
- **Integration Service** (Gmail Connector)
- **Claude Code** with `/uipath:uipath-maestro-flow` skill
- **Git & Git LFS**

---

## 🔗 Related Resources

- 🌟 [Awesome Maestro Flow](https://github.com/1aifanatic/awesome-maestro-flow) — Community-curated collection of Maestro Flow projects, patterns, and integrations.
- 📖 [UiPath Solutions Management Docs](https://docs.uipath.com/solutions-management/automation-cloud/latest)

---

## 📄 License

MIT License © Naveen Chatlapalli
