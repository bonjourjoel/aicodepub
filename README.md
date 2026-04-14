# 🤖 What is AICode?

> AI models generate low quality code at record speed: junior-grade, duplicated, and inconsistent code that breaks your architectural invariants.  
> AICode is the operating system above the model. It constrains the model to respect the project's global context and to produce senior-grade code.  
> 💀 Generative AI is saturating the market with toxic code. 💡 AICode is the antidote.
>
> Dogfooding: AICode itself is a typescript program of 500.000 lines of code, generated and maintained by a solo developer using AICode.  
> Think it's impossible? Try it.

AICode has all the abilities of classical agents:

- ✅ explore and understand your codebase
- ✅ debug, write, or modify code with an AI coding assistant

So what makes it different? ➡️ Unlike other AI coding agents that produce code directly from a prompt, AICode is _spec driven_. It combines AI analysis with human review to **catch AI mistakes before they reach your codebase**, making AI safe even for large, critical projects.

- ✅ **Structured specifications** you can review and fix before any code is produced
- ✅ **Refine** (pre-code checks) and **Verify** (post-code audit) loops to catch design flaws and hidden side-effects early
- ✅ **Reviewable patches** in a virtual workspace that you accept file by file and line by line

<br />

![AI Code assistant](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/aicode-workflow.webp)

AICode also includes features you won’t find in typical AI agents:

- ✅ an overpowered 5D index, able to find related code and documentation in every way possible
- ✅ an extensive system-instruction layer specialized for programming workflows and engineering best practices
- ✅ a project map that helps the model understand your project’s global architecture with far fewer hallucinations
- ✅ a powerful AI debugger: it can instrument suspected code and iteratively explore code paths, or trace regressions to their root cause using Git history

<br />

# 🎯 Who is it for?

- Developers who want an **AI coding assistant** but refuse unreviewed auto-edits  
  ➡️ Solve the problem: “_I vibe-coded a prototype to prove the idea, but now I must rewrite it from scratch manually._”

- Teams who care about **code quality, architecture, and long-term maintainability**  
  ➡️ Solve the problem: “_AI helps us move faster, but our codebase is gradually becoming unmaintainable._”

- Managers who want to use AI acceleration on **large production codebases** without turning the repo into a “prompt-generated mess”  
  ➡️ Solve the problem: “_I want to provide AI assistance to my development teams, but I'm worried it could lead to low-quality code._”

<br />

# 🧠 How does it align models and enforce guardrails?

AICode is designed to reduce the most common failure modes of AI-assisted coding:

- ↘️ unclear requirements turning into incorrect implementations
- ↘️ overconfident “fixes” that hide symptoms instead of solving the root cause
- ↘️ regressions caused by narrow-focus changes
- ↘️ architecture drift and inconsistent patterns from unreviewed auto-edits

For the most complex tasks, AICode prevents these issues by using a controlled workflow: **Ideate → Specify → Refine → Code → Verify**.

- ↗️ **Before coding - Ideate**: clarify and lock the intent
- ↗️ **Before coding - Specify**: control the software architecture
- ↗️ **Before coding - Refine**: audit spec to catch design mistakes early
- ↗️ **During coding - Code**: review patches
- ↗️ **After coding - Verify**: audit generated code vs spec

Bottom line: **↗️ AI speed + ↗️ AI audit loops + ↗️ human control = ↗️↗️↗️ maintainable AI-generated code**.

> YouTube introduction + real workflow demo: https://youtu.be/RMB0etc3DnI

<br />

# 🚀 Setup

Because AICode is offline-first, the install from VS Code takes 2-3 minutes. Please be patient.

![setup AICode assistant](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/quick-setup.png)

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

### 👀 Code review

AICode agent can review PRs using your local Git repo and MCP connectors (GitHub, GitLab, Jira, etc.).

### 🧠 Specialized system instructions

AICode isn’t a raw chat model plugged into VS Code. It runs the model inside a system-instruction layer specialized for programming tasks.

- **Honest by design:** it won’t bluff when context is missing or uncertain; instead it will work with you to reach a reliable result
- **Architecture & quality guardrails:** it plans changes, enforces engineering best practices, keeps code architectured and maintainable
- **Anti-hallucination by default:** answers must be grounded in evidence

### 🧩 MCP connectors

Connect any local or cloud service supporting the MCP protocol.

### 🔒 Enterprise-grade security

AICode copilot is offline-first, designed to avoid uploading your entire codebase:

- indexing is local, including vector indexing
- chat history is local
- only relevant excerpts are sent to your model provider
- BYOK means you connect directly to OpenAI / Azure (no intermediate server)

For large corporations: Azure cloud compatibility fits strict data policies.
