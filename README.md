# 💳 Ambient Expense Agent

> An AI-powered corporate expense approval agent built with **Google Agent Development Kit (ADK) 2.0** that automatically validates, categorizes, and approves expense reports using Graph Workflows and human-in-the-loop review.

![Python](https://img.shields.io/badge/Python-3.11+-blue)
![ADK](https://img.shields.io/badge/Google-ADK%202.0-green)
![License](https://img.shields.io/badge/License-Apache%202.0-orange)

---

## 📌 Overview

Ambient Expense Agent streamlines corporate expense approvals by combining AI reasoning with deterministic workflow execution.

Instead of relying on fixed approval rules, the agent:

- Validates submitted expenses
- Detects policy violations
- Performs receipt verification
- Categorizes expenses
- Routes high-risk claims for manual approval
- Automatically approves compliant reports

Built using **Google ADK 2.0 Graph Workflow API**, the project demonstrates production-ready agent development with human-in-the-loop interactions.

---

# ✨ Features

- 🤖 AI-powered expense validation
- 📄 Receipt verification
- 💰 Budget policy checks
- 🛡 Fraud detection hooks
- 👤 Human approval workflow
- ⚡ Google ADK 2.0 Graph Workflows
- 📊 Evaluation pipeline
- ☁ Deployable to Google Agent Runtime
- 🔍 Built-in tracing and observability

---

# 🏗 Architecture

```
                Employee

                    │

          Submit Expense Report

                    │

                    ▼

         Expense Validation Node

                    │

        ┌───────────┴───────────┐

        │                       │

        ▼                       ▼

  Auto Approve           Human Review

        │                       │

        └───────────┬───────────┘

                    ▼

             Final Decision
```

---

# 🛠 Tech Stack

| Category | Technology |
|-----------|------------|
| Language | Python |
| Framework | Google ADK 2.0 |
| Workflow | Graph Workflow API |
| Runtime | Agents CLI |
| Deployment | Google Agent Runtime |
| Package Manager | uv |
| Infrastructure | Terraform |
| Observability | Cloud Trace |

---

# 📂 Project Structure

```
ambient-expense-agent/

├── expense_agent/
│   ├── app/
│   ├── workflows/
│   ├── tools/
│   └── prompts/
│
├── tests/
├── deployment/
├── artifacts/
├── README.md
├── pyproject.toml
└── uv.lock
```

---

# 🚀 Getting Started

## Prerequisites

- Python 3.11+
- uv
- Google Agents CLI
- Google ADK 2.0
- Google AI Studio API Key

---

## Installation

```bash
git clone https://github.com/<username>/ambient-expense-agent.git

cd ambient-expense-agent

uv sync

agents-cli install
```

---

# 🔑 Configure Environment

Create a `.env`

```env
GEMINI_API_KEY=YOUR_API_KEY
```

---

# ▶ Run Locally

```bash
agents-cli playground
```

---

# 🧪 Run Tests

```bash
uv run pytest
```

---

# 🚀 Deployment

```bash
gcloud config set project PROJECT_ID

agents-cli deploy
```

---

# 📊 Evaluation

Run automated evaluations:

```bash
agents-cli eval
```

---

# 📈 Observability

The project exports telemetry to:

- Cloud Trace
- Cloud Logging
- BigQuery

---

# 🔒 Security

- Prompt injection protection
- Human approval for high-risk actions
- Policy validation
- Input sanitization

---

# 📖 Learning Objectives

This project demonstrates:

- Google ADK 2.0
- Graph Workflows
- Function Nodes
- Human-in-the-loop Agents
- Agent Deployment
- Production Evaluation
- Enterprise AI Agent Design

---

# 🗺 Roadmap

- [ ] OCR Receipt Parsing
- [ ] Fraud Detection Model
- [ ] Slack Integration
- [ ] Email Notifications
- [ ] Multi-currency Support
- [ ] Dashboard

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Open a Pull Request.

---

# 📄 License

Licensed under the Apache 2.0 License.
