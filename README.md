# 🤖 What is AICode?

AICode is a complete **AI coding assistant** solution for Visual Studio Code, based on ChatGPT 5.2, able to analyse any codebase and generate code based on your prompts. But it also has a singularity:  
It helps you **catch AI mistakes before they reach your repo** by combining additional AI analysis with **explicit human review** at every step.

- ✅ **Structured specifications** you can review and fix before any code is produced
- ✅ **Refine** (pre-code checks) and **Verify** (post-code audit) loops to catch design flaws and hidden side-effects early
- ✅ **Reviewable patches** in a virtual workspace that you accept file by file and line by line

![AICode AI Coding assistant](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/aicode-workflow.webp)

# 🧠 Who is it for?

- Developers who want an **AI coding assistant** but refuse unreviewed auto-edits
- Teams who care about **code quality, architecture, and long-term maintainability**
- People who want to use AI on **large production codebases** without turning the repo into a “prompt-generated mess”

# 🎯 How does it work?

AICode is designed to reduce the most common failure modes of AI-assisted coding:

- unclear requirements turning into incorrect implementations,
- overconfident “fixes” that hide symptoms instead of solving root cause,
- regressions caused by narrow-focus changes,
- architecture drift and inconsistent patterns from unreviewed auto-edits.

AICode prevents these issues by forcing a controlled workflow: **Ideate → Specify → Refine → Code → Verify**

- **Before coding**: clarify and lock the intent (Ideate + Specify)
- **Before coding**: catch mistakes early (Refine)
- **During coding**: you review patches (virtual workspace, manual accept)
- **After coding**: audit vs spec (Verify)

Bottom line: **AI speed + human control**.

> YouTube introduction + real workflow demo: https://youtu.be/RMB0etc3DnI

# 🚀 Quick setup

![setup](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/quick-setup.png)

# ✨ Feature highlights

### 💬 Chat with your codebase (grounded answers)

AICode can read your workspace using multiple tools and indexes (project map, lexical search, vector search, AST/symbol navigation, Git history).  
This helps it analyse the project and find relevant sections in every way possible.

### 🛡️ Safe patch workflow (no silent actions)

- No automatic repo edits
- No hidden background changes
- Every change is presented as a reviewable patch

### 📝 Structured specs (review-first)

Turn complex requests into a specification you can read and correct before any code is produced.

### 🐞 AI-assisted debugging workflows

Built-in guided debugging approaches (instrumentation-based workflows, regression investigation via Git history, etc.).

### 👀 Code reviews

AICode can help review PRs using your local Git repo and (optionally) MCP connectors (GitHub, GitLab, Jira, etc.).

### 🔒 Offline-first + BYOK

AICode is designed to avoid uploading your entire codebase:

- indexing is local,
- chat history is local,
- only relevant excerpts are sent to your model provider,
- BYOK means you connect directly to OpenAI / Azure (no intermediate server).
