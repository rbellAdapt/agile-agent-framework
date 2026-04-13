# Agile Agent Framework

A specialized, multi-agent scaffolding architecture designed to supercharge AI-driven software development by enforcing strict Agile, Scrum, and role-based personas within your workspace. 

By compartmentalizing instructions across specialized personas, you ensure that your LLM agents (like Google Gemini or GitHub Copilot) act with hyper-focused context, eliminating hallucination and preventing architectural drift from a lack of specialization.

## 🚀 Core Philosophy
The framework is built to mirror an elite enterprise engineering team. Instead of interacting with a generic AI, you interact with specific roles (@arch, @dev, @ops, @qa) constrained by explicit project rules, workflows, and environmental variables. 

- **Role-Based Execution:** LLMs perform substantially better when assigned rigid personas with distinct boundaries. 
- **Strict Guardrails:** Rules engine for branch locking, atomic commits, design guidelines, and code aesthetics.
- **Workflow Automation:** Reusable `slash-command` workflows mapped to continuous integration and pipeline logic.

## 📂 Framework Structure

The repository architecture is divided into the framework logic (`.agents`) and your environment (`project-root`):

```text
/
├── .agents/                    # The AI Framework Logic
│   ├── handover.md             # Continuous state context
│   ├── project_charter.md      # Ground truth mission & tech stack boundaries
│   ├── personas/               # Role instructions (@arch, @dev, @brand, etc.)
│   ├── rules/                  # Development guardrails (locks, scrum, git rules)
│   ├── skills/                 # Extensible abilities for agents
│   └── workflows/              # Reusable automation processes (e.g. /atomic-commit-push)
│
├── project-root/               # Your actual project code lives here
│   ├── docs/                   # Logs, UI guides, implementation plans
│   ├── src/                    # Source Code
│   ├── tests/                  # Unit and Integration Tests
│   └── README.md               # Your project-specific Readme
```

## 🛠️ Usage & Integration

1. Clone or copy the `.agents` and `project-root` structure into your working environment.
2. Update the `.agents/project_charter.md` with your specific objectives, tech stack, and SME boundaries.
3. Configure `docs/environment_config.md` with relevant domain pointers.
4. Begin your coding session by addressing a persona (e.g., *"@arch, please draft an implementation plan for..."*).

## 🧑‍💻 The Antigravity Team Personas

- **@arch**: The Lead Technical Architect - Plans, researches, and writes system implementation plans.
- **@dev**: The Core Gameplay/Software Developer - Strictly executes code against established guidelines.
- **@ops**: Deployment & Infrastructure - Handles Docker compose, Vercel/AWS routing, CI/CD.
- **@sme**: Subject Matter Expert - Analyzes domains like tax logic, fluid dynamics, or financial ledgers to govern logic.
- **@brand / @prod**: Product Owner - Governs styling, aesthetic rules, UI elements, and user experience.
- **@qa**: Quality Assurance - Scrutinizes paths, linters, accessibility bounds, and writes tests.

## 🤝 Contribution
Designed and iterated upon for `rbellAdapt/agile-agent-framework`. Pull requests for enhanced agent skills or workflows are welcome.
