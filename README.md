# 🤖 AICode: develop at light speed, without code review.

> Classical AI coding agents write code fast. But the bottleneck was never generation, it's the human code review that follows, capping the real gain at 0x to 4x, with uncertain quality. AICode moves the control **before** the code is generated, not after: reading and fixing an intent is far easier than reading and fixing code. Result: **10x to 200x speed, with industrial quality**. Nothing slows down the AI.

![AICode workflow: Ideate, Specify, Refine, Code, Verify](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/aicode-workflow.webp)

<br />

## ⚡ Why it's fast

Standard agents write code, then you review it. That review is the real bottleneck: heavy debug, every time. AICode audits the **spec**, not the code: a specification is an order of magnitude smaller and easier to read than the code it produces. Catching a mistake there is roughly 100x cheaper than catching it in production.

![Classical AI rush (heavy debug) versus AICode (heavy spec)](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/shift.png)

<br />

## 🔁 Ideate → Specify → Refine → Code → Verify

- **Ideate**: clarify and lock the intent with the model
- **Specify**: get a formal spec you read and correct, not code you have to reverse-engineer
- **Refine**: the AI audits the spec against your real codebase, as many passes as you want, each one graded by severity
- **Code**: generated in a virtual workspace, reviewable patch by patch
- **Verify**: the AI audits its own code against the spec afterward

![Refine pass: severity-graded list of changes with justification](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/refine-en.png)

<br />

## 📊 Proof, on a real system

In this case study, the agent rebuilds a core system invariant across 160 files in three days, correcting 201 errors before shipping with zero bugs and zero regressions: [read the case study →](https://aisovereignlabs.ai/docs/case-study/liveSession/case-study-live-session-en.pdf)

<br />

## 🕵️ Understands code nobody documented

Most codebases lose their map the moment the person who built them leaves, or the moment nobody bothered to write it down in the first place. AICode's 5D index (project map, lexical, vector, symbols, Git history) rebuilds that missing map from the code itself, so you're never the first person forced to reverse-engineer it from scratch.

![Understanding undocumented code despite turnover](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/turnover.png)

<br />

## 🧠 What makes AICode different

- ✅ **Structured specs, reviewed before code exists**, not after
- ✅ **Refine + Verify loops** catching design flaws and hidden side effects early
- ✅ **Reviewable patches**, file by file, line by line, nothing auto-written
- ✅ **AI debugger**: instrumentation-based exploration, or Git-history regression tracing
- ✅ **Specialized system instructions**: honest by design, won't bluff when context is missing
- ✅ **MCP connectors / Skills**: no vendor lock-in
- ✅ **Offline-first / BYOK**: local index, your own API key, direct connection to OpenAI or your private Azure tenant, nothing transits through us

<br />

## 🚀 Setup

Offline-first, so the initial install takes 2-3 minutes.

![setup AICode assistant](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/quick-setup.png)

1. Install the extension from the marketplace
2. Open Settings, configure your LLM provider
3. Paste your OpenAI or Azure key, stored locally
4. Wait for indexing (~20 min per 100k LOC). Start a new chat, describe your task
