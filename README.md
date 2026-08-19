# 🤖 AICode: develop at light speed, without code review.

Classical AI coding agents write code very fast. But the bottleneck is the human code review that follows, capping the real gain at 0x to 4x.

AICode moves the control **before** the code is generated, not after. Reading and fixing an intent is far easier than reading and fixing code.

Result: Industrial quality code at 10x to 200x speed.

![AICode fast without review](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/aicode-speed-noreview.png)

<br />

## Featured in

- [↗ Sourcefeed](https://sourcefeed.dev/a/when-the-spec-becomes-the-code-review) → _"genuinely the most interesting protocol document I've read this year"_

- [↗ BizStack](https://bizstack.tech/ai-agent-refactored-189-files-in-a-717k-line-codebase-for-2430/) → _"For solo developers and small teams facing deep architectural debt, the protocol described here is worth reading carefully."_

- [↗ AI Weekly](https://aiweekly.co/alerts/abenhaim-ai-agent-refactors-189-files-in-717k-line-typescript-app) → _"protocol reference for spec-first agent refactors that is hard to wave away"_

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

![AICode workflow: Ideate, Specify, Refine, Code, Verify](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/aicode-workflow.webp)

<br />

## 🐞 The AI audits and finds the errors, pass after pass

This is what AICode can do for you, as many times as you want. Let the AI do the dirty job and find all the errors. Why would you bother?

![Refine pass: severity-graded list of changes with justification](https://raw.githubusercontent.com/bonjourjoel/aicodepub/main/marketplace-assets/screenshots/refine-en.png)

<br />

## 📊 Proof, on a real system

In the following case study, published on arXiv, the agent rebuilds a core system invariant in just three days, with minimal human input, running 31 verification passes and correcting 201 errors, before shipping code with zero bugs, zero regressions, and zero technical debt:

[↗ read the case study](https://arxiv.org/abs/2608.12440)

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
