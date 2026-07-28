# Elchai Group Pre-Interview Assessment Prototype

**Candidate:** Abdullah Saleem  
**Role:** AI Agent & OpenClaw Research Intern  

---

## Overview

This repository contains a functional workflow prototype demonstrating a **Client Brief to Proposal SOW Pipeline** powered by an OpenClaw-governed architecture.

## Key Governance Features

* **Prompt Injection Isolation:** Enforces strict XML tag boundary isolation for raw client inputs.
* **Human-in-the-Loop (HITL) Gate:** Automatically pauses execution after drafting and sets status to `PENDING HUMAN REVIEW`.
* **Audit Logging:** Logs timestamps, tools, input/output paths, and review states in `execution_log.json`.

---

## 📁 Repository Structure

```text
.
├── agent_workflow.py            # Main agent pipeline script
├── execution_log.json           # Execution and audit log history
├── sample_brief.txt             # Input sample client brief
├── output/                      # Generated proposals folder
│   ├── SOW_Draft_ApexLogistics.md      # Draft requiring review
│   └── SOW_APPROVED_ApexLogistics.md   # Final approved proposal
└── README.md                    # Documentation


## Quick Start
1. Clone & Navigate
Bash
git clone [https://github.com/abdullahsaleem2005-svg/elchai-proposal-agent-assessment.git](https://github.com/abdullahsaleem2005-svg/elchai-proposal-agent-assessment.git)
cd elchai-proposal-agent-assessment

2. Run Script
Bash
python3 agent_workflow.py
