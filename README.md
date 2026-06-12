# Risk & Governance Analysis of Open-Source AI Agent Deployment

This repository contains a presentation report on the risk and governance analysis of open-source AI agent deployment. The report focuses on how traditional risk assessment frameworks can be extended to address the specific risks introduced by LLM-driven autonomous agents.

The presentation was prepared for **Google Developer Group on Campus NCU × OpenTPI**.

---

## Overview

Open-source AI agents are rapidly moving from experimental demonstrations toward real-world deployment. Unlike traditional software systems, AI agents may interpret natural language instructions, interact with external tools, store memory, call APIs, communicate with other agents, and perform actions in dynamic environments.

This creates a new governance problem: traditional risk assessment remains useful, but it must be extended to account for autonomy, tool use, prompt injection, memory poisoning, identity misuse, action propagation, and other agent-specific risks.

This report analyzes how risk assessment can be adapted for open-source AI agent deployment by combining three perspectives:

1. **Traditional Risk Assessment**
   Provides the general process for identifying assets, attack surfaces, threats, risk levels, controls, and validation methods.

2. **OWASP GenAI Security Project**
   Provides structured threat categories and mitigation references for generative AI and agentic AI systems.

3. **CORA: Conformal Risk-Controlled GUI Agent**
   Demonstrates how action-level risk control can be applied before an AI agent executes potentially risky actions.

---

## Main Topics

* Research motivation for open-source AI agent governance
* Traditional risk assessment structure
* Limitations of traditional assessment when applied to AI systems
* AI-specific risk assessment flow
* AI assets, attack surfaces, threats, and risk factors
* OWASP GenAI Security Project
* Agentic AI threat categories
* Memory poisoning, tool misuse, privilege compromise, identity spoofing, and multi-agent risks
* CORA safety control architecture
* Post-policy, pre-action risk control
* Integrated agentic AI risk framework

---

## Repository Structure

```text
agentic-ai-risk-governance/
├── README.md
├── slides/
│   └── risk-governance-open-source-ai-agent-deployment.pdf
├── references.md
└── LICENSE
```

---

## Slides

[View presentation slides](./slides/Risk and Governance Analysis of Open-Source AI Agent Deployment.pdf)

## Core Argument

The central argument of this report is that open-source AI agent deployment requires a layered governance framework.

Traditional risk assessment can define **how to assess risk**, but it does not fully specify which agentic threats should be evaluated. OWASP helps fill this gap by providing a structured threat library for generative AI and agentic AI systems. CORA then demonstrates how risk governance can move from abstract threat identification to concrete action-level control before execution.

In simplified form:

```text
Traditional Risk Assessment
        ↓
Defines the risk assessment process

OWASP Agentic AI Threats
        ↓
Defines what agentic threats to evaluate

CORA
        ↓
Demonstrates how risky actions can be controlled before execution
```

Together, these perspectives form an integrated framework for assessing and governing open-source AI agents.

---

## Key Framework

| Layer                       | Role                                     | Output                                                                   |
| --------------------------- | ---------------------------------------- | ------------------------------------------------------------------------ |
| Traditional Risk Assessment | Provides the assessment process          | Assets, attack surface, risk scoring, controls, validation               |
| OWASP Agentic AI            | Provides the threat library              | Threat categories and mitigation mapping                                 |
| CORA                        | Demonstrates action-level safety control | Risk estimation, selective execution, confirmation, reflection, or abort |

---

## Author

- **Author:** 許穎軒
- **Department:** Department of Physics
- **Institution:** National Central University

---

## Context

This report was prepared as part of a technical presentation for **Google Developer Group on Campus NCU × OpenTPI**.

---

## References

The report references materials from OWASP, arXiv papers on AI agents and tool use, OpenAI, Anthropic, and LangChain documentation.

[View full references](./references.md)

## Disclaimer

This repository is an independent educational and analytical report. It does not represent the official position of Google, Google Developer Group on Campus, OpenTPI, OWASP, OpenAI, Anthropic, LangChain, or any other referenced organization.

---

## AI-Assisted Visual Content Disclosure

Some visual elements in this presentation may have been created or refined with the assistance of generative AI tools. All AI-assisted visuals were reviewed, selected, and edited by the author for educational and presentation purposes.

---

## License

This work is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).
