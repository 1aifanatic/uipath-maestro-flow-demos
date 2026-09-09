# UiPath Maestro Flow Demos 🚀

A collection of production-ready [UiPath Maestro Flow](https://www.uipath.com/product/maestro) projects, orchestration templates, patterns, and hands-on video walkthroughs.

Curated by **Naveen Chatlapalli** ([@1aifanatic](https://github.com/1aifanatic)).

---

## 📂 Featured Demos

### 1. [Employee Expense Approval](./Employee%20expense%20approval/)

An intelligent, multi-tier expense approval workflow built with UiPath Maestro Flow, CLI automation, autonomous AI agents, and Context Grounding.

* **Part 1 Video**: 🎥 [Watch / Download Part 1 (Architecture & CLI)](https://github.com/1aifanatic/uipath-maestro-flow-demos/releases/download/v1.0.0/Maestro_Flow_Employee_Expense_Approval_Part1.mp4)
* **Part 2 Video**: 🎥 [Watch / Download Part 2 (Runtime & Action Center)](https://github.com/1aifanatic/uipath-maestro-flow-demos/releases/download/v2.0.0/Maestro_Flow_Employee_Expense_Approval_Part2.mp4)
* **Part 3 Video (New)**: 🎥 [Watch / Download Part 3 (AI Agent & Context Grounding)](https://github.com/1aifanatic/uipath-maestro-flow-demos/releases/download/v3.0.0/Maestro_Flow_AI_Agent_Context_Grounding.mp4)
* **Status**: Complete End-to-End Walkthrough Series.

---

## 🎬 Video Series Overview

### 🔹 Part 1: Architecture & Scaffolding
Scaffolding a Maestro Flow using the UiPath CLI and Claude Code:
| Timestamp | Chapter | Description |
|---|---|---|
| **00:00** | **Maestro Flow Concept** | Why Maestro Flow bridges AI agents, APIs, people, and RPA |
| **00:18** | **The Business Story** | Solving expense reimbursement bottlenecks and fragmented approvals |
| **00:34** | **Architecture in One Picture** | Multi-tier decision rules (<$100 auto-approval, manager escalation) |
| **00:50** | **UiPath CLI Setup** | Installing `uipath-cli` via PowerShell and exploring docs |
| **01:30** | **Orchestrator Staging & Login** | Authenticating to `aifanatic / DefaultTenant` |
| **02:15** | **Claude Code Automation** | Invoking `/uipath:uipath-maestro-flow` to scaffold 8 nodes & 15 variables |
| **03:40** | **Studio Web Canvas** | Inspecting the visual canvas in Studio Web |

### 🔹 Part 2: Runtime Execution & Multi-Channel Action Center
Runtime execution, inline human-in-the-loop task handling, and Integration Service notification:
| Timestamp | Chapter | Description |
|---|---|---|
| **00:00** | **Canvas Walkthrough** | Reviewing deployed 8-node Maestro Flow layout |
| **00:15** | **Auto Approve Node** | JavaScript payload block formatting approval output |
| **00:25** | **Threshold Logic** | `<=$100` condition branching between auto-approval and escalation |
| **00:36** | **Inline Action Center** | Multi-channel delivery across Slack, Teams, Email, and Action Center |
| **00:57** | **Send Email Activity** | Integration Service Gmail connector binding |
| **01:08** | **HTML Email Builder** | Dynamic card generation with status badges and comments |
| **01:25** | **Debug Run 1 ($50)** | Under-threshold execution and Gmail verification |
| **02:19** | **Debug Run 2 ($1,000)** | Policy escalation, inline task review ("Travel reason verified"), and approval |
| **03:34** | **Architecture Takeaway** | "Orchestration is the product" |

### 🔹 Part 3: Autonomous AI Agent with Context Grounding
Implementing an inline autonomous AI agent grounded with enterprise policy documents:
| Timestamp | Chapter | Description |
|---|---|---|
| **00:00** | **Inline AI Agent Introduction** | Adding the autonomous Expense Policy Reviewer Agent to the canvas |
| **00:19** | **Agent Configuration & Model** | Configuring standard harness with GPT-5.6-terra reasoning model |
| **00:39** | **System Prompt & JSON Schema** | Evidence-based compliance prompt and structured output schema |
| **00:59** | **Context Grounding Index** | Creating `EmployeeCompanyPolicy` in UiPath Agents with Advanced ingestion |
| **01:19** | **Company Policy Excel Sheet** | Inspecting policy rules (airfare, hotels, meals, receipt thresholds) |
| **01:50** | **Storage Bucket & File Ingestion** | Uploading `Expense_Review_Policies.xlsx` directly into storage bucket |
| **02:18** | **Index Synchronization** | Verifying `Successful` ingestion status and query readiness |
| **02:45** | **Zero-Code Agent Grounding** | Clicking `+ Context` to wire `EmployeeCompanyPolicy` directly to the agent |
| **03:17** | **Action Center Integration** | Binding manager approval task fields to AI policy outputs |
| **03:35** | **Test Run 1: $30 Meal Expense** | Debug execution triggering agent and context grounding tool calls |
| **04:35** | **Action Center Review: Hold for Receipt** | Reviewing AI findings, medium severity, and approving the task |
| **04:58** | **Gmail Verification: Run 1** | Inspecting the approved email notification in Gmail |
| **05:12** | **Test Run 2: $15 Under-Threshold** | Debug execution with $15 meal expense |
| **05:35** | **Severity Analysis: None** | Agent verifies $15 is under the $25 receipt threshold (`severity: None`) |
| **05:58** | **Final Branded Email & Outro** | Responsive HTML email with embedded AI policy review card |

---

## 🛠️ Tech Stack & Prerequisites

- **UiPath CLI** (`uip`) v1.200.0+
- **UiPath Studio Web** & **Automation Cloud**
- **UiPath Autonomous Agents** (`gpt-5.6-terra`)
- **UiPath Context Grounding** (Vector RAG on Storage Buckets)
- **UiPath Action Center** (Inline Tasks & Multi-Channel Delivery)
- **Integration Service** (Gmail Connector)
- **Claude Code** with `/uipath:uipath-maestro-flow` skill
- **Git & Git LFS**

---

## 🔗 Related Resources

- 🌟 [Awesome Maestro Flow](https://github.com/1aifanatic/awesome-maestro-flow) — Community-curated collection of Maestro Flow projects, patterns, and integrations.
- 📖 [UiPath Context Grounding Docs](https://docs.uipath.com/ai-center/automation-cloud/latest/user-guide/context-grounding)

---

## 📄 License

MIT License © Naveen Chatlapalli
