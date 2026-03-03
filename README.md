# 🤖 What is AI Code?

AI Code is a complete **AI copilot** solution for Visual Studio Code, based on ChatGPT 5.2. Use it to:

- ✅ explore and understand your codebase
- ✅ debug, write, or modify code with an AI coding assistant

Unlike other AI tools, it **catches AI mistakes before they reach your codebase** by combining AI analysis with explicit **human review**, making AI safe even for large, critical projects.

- ✅ **Structured specifications** you can review and fix before any code is produced
- ✅ **Refine** (pre-code checks) and **Verify** (post-code audit) loops to catch design flaws and hidden side-effects early
- ✅ **Reviewable patches** in a virtual workspace that you accept file by file and line by line

<br />

![AI Code assistant](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/aicode-workflow.webp)

AI Code also includes features you won’t find in typical AI agents:

- ✅ an extensive system-instruction layer specialized for programming workflows and engineering best practices
- ✅ a project map that helps the model understand your project’s global architecture with far fewer hallucinations
- ✅ a powerful AI debugger: it can instrument suspected code and iteratively explore code paths, or trace regressions to their root cause using Git history

<br />

# 🧠 Who is it for?

- Developers who want an **AI coding assistant** but refuse unreviewed auto-edits
- Teams who care about **code quality, architecture, and long-term maintainability**
- Managers who want to use AI on **large production codebases** without turning the repo into a “prompt-generated mess”

<br />

# 🎯 How does it align models and enforce guardrails?

AI Code is designed to reduce the most common failure modes of AI-assisted coding:

- unclear requirements turning into incorrect implementations
- overconfident “fixes” that hide symptoms instead of solving the root cause
- regressions caused by narrow-focus changes
- architecture drift and inconsistent patterns from unreviewed auto-edits

For the most complex tasks, AICode prevents these issues by using a controlled workflow: **Ideate → Specify → Refine → Code → Verify**.

- **Before coding - Ideate**: clarify and lock the intent
- **Before coding - Specify**: control the software architecture
- **Before coding - Refine**: audit spec to catch design mistakes early
- **During coding - Code**: review patches
- **After coding - Verify**: audit generated code vs spec

Bottom line: **AI speed + AI audit loops + human control = maintainable AI-generated code**.

> YouTube introduction + real workflow demo: https://youtu.be/RMB0etc3DnI

<br />

# 🚀 Setup

Because AICode is offline-first, the install from VS Code takes 2-3 minutes. Please be patient.

![setup AI code assistant](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/quick-setup.png)

<br />

# ✨ Feature highlights

### 💬 Chat with your codebase

AICode can read your workspace using a five-dimensional index, making it smarter by allowing it to find relevant sections in every way possible:

- project map: the AI can immediately see the whole project architecture, reducing hallucinations
- lexical search
- vector search
- AST/symbol navigation
- git history: to see back in time

### 📝 Structured specs (review-first)

Turn complex requests into a specification you can read and correct before any code is produced.

### 🔎 Refine and verify loops

Instruct the AI to second-guess its work, as many times as you want. Each iteration finds more errors in the specification/code.

### 🛡️ Safe patch workflow

Keep a human in the loop. Every change is presented as a reviewable patch.

### 🐞 Powerful AI-assisted debugger

- Instrumentation-based debug: automatically finds and explains bugs in code areas that you don't fully understand
- Regression investigation via Git history: compares current code to old revisions to find the commit that introduced the regression

### 🧠 Specialized system instructions

AI Code isn’t a raw chat model plugged into VS Code. It runs the model inside a system-instruction layer specialized for programming tasks.

- **Honest by design:** it won’t bluff when context is missing or uncertain; instead it will work with you to reach a reliable result
- **Architecture & quality guardrails:** it plans changes, enforces engineering best practices, keeps code architectured and maintainable
- **Anti-hallucination by default:** answers must be grounded in evidence

### 👀 Code review

AICode agent can review PRs using your local Git repo and MCP connectors (GitHub, GitLab, Jira, etc.).

### 🔒 Enterprise-grade security

AI Code copilot is offline-first, designed to avoid uploading your entire codebase:

- indexing is local, including vector indexing
- chat history is local
- only relevant excerpts are sent to your model provider
- BYOK means you connect directly to OpenAI / Azure (no intermediate server)

For large corporations: Azure cloud compatibility fits strict data policies.
