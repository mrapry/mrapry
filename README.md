<div align="center">

# Hi, I'm mrapry 👋

### Software Engineer • Systems & Architecture • Local-first & AI Tooling

I'm genuinely obsessed with how software is *built* — not just making it work, but making it **clean, principled, and durable**. I care deeply about system architecture, sound engineering principles (SOLID, clean boundaries, testability), performance, and developer experience.

I gravitate toward fast, private, no-nonsense tools — the kind that run as a single binary, work offline, and respect your data. Every project I ship is an exercise in getting the fundamentals right.

`Architecture` · `Clean Code` · `Design Principles` · `Performance` · `Local-first` · `AI Tooling` · `Rust` · `Systems Programming`

</div>

---

### 🧭 How I approach engineering

- 🏛️ **Architecture first** — I design around clear boundaries and stable interfaces (traits/contracts), so systems stay flexible as they grow.
- 🧱 **Principles over shortcuts** — SOLID, separation of concerns, and dependency inversion aren't buzzwords to me; they're how I keep code maintainable.
- ✅ **Tested & verifiable** — a clean, fully tested core is non-negotiable. If it can't be verified, it isn't done.
- ⚡ **Performance & footprint** — single binaries, no bloated runtimes, no unnecessary dependencies.
- 🔒 **Privacy by default** — your data stays yours; local-first is the baseline, not a feature.

---

<div align="center">

## 🧠 Featured Project — [YourBrain (`yb`)](https://github.com/mrapry/YourBrain)

**A local-first memory engine that gives AI coding agents a persistent, coherent long-term memory — with first-class conflict resolution.**

[![Rust](https://img.shields.io/badge/Rust-1.75%2B-000000?style=for-the-badge&logo=rust&logoColor=white)](https://www.rust-lang.org/)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue?style=for-the-badge)](https://github.com/mrapry/YourBrain/blob/main/LICENSE)
[![Local-first](https://img.shields.io/badge/Local--first-100%25%20offline-2ea44f?style=for-the-badge)](https://github.com/mrapry/YourBrain)
[![MCP](https://img.shields.io/badge/MCP-ready-8A2BE2?style=for-the-badge)](https://github.com/mrapry/YourBrain)

[![Stars](https://img.shields.io/github/stars/mrapry/YourBrain?style=social)](https://github.com/mrapry/YourBrain/stargazers)
[![Forks](https://img.shields.io/github/forks/mrapry/YourBrain?style=social)](https://github.com/mrapry/YourBrain/network/members)

**[⭐ Star it](https://github.com/mrapry/YourBrain)** · **[📦 Explore the code](https://github.com/mrapry/YourBrain)** · **[🛠️ Contribute](https://github.com/mrapry/YourBrain/blob/main/README.md#contributing)**

</div>

---

### 😵 The problem: agentic AI has amnesia

Today's AI coding agents are brilliant but **stateless**. Every new chat starts from zero — they forget your architecture decisions, burn tokens re-reading pasted context, and confidently contradict facts that changed three refactors ago. Most "memory" add-ons are just an append-only vector store that slowly rots into a pile of conflicting half-truths.

**MCP gave agents tools. It did not give them a coherent long-term memory.** YourBrain does.

### ✨ Why YourBrain is different

| | Without YourBrain | With YourBrain |
| --- | --- | --- |
| 🔁 Context | Re-explain everything each session | Agent recalls prior decisions instantly |
| ⚔️ Conflicts | Memory silently goes stale | Conflicts **detected & resolved** on write |
| 💸 Cost | Big prompts, high token spend | Token-budgeted, compressed recall |
| 🎯 Accuracy | Confident hallucinations | Answers **fact-checked** against your KB |
| 🔒 Privacy | Cloud lock-in, data leaves your machine | 100% local, single binary, your data stays put |

> **The differentiator is the conflict engine.** When new knowledge duplicates, supersedes, or contradicts what was stored before, YourBrain detects it, auto-resolves the safe cases, asks a human for the ambiguous ones, and keeps a full audit timeline + relationship graph so history is never lost.

### 🚀 Highlights

- 🧩 **Automatic conflict resolution** — duplicate / supersede / contradiction detection, auto or ask
- 🔍 **Hybrid search** — SQLite FTS5 keyword + vector similarity fused with Reciprocal Rank Fusion, then BM25 reranked
- 🗜️ **Code-safe compression** — preserves code, paths, and URLs while shrinking tokens
- 🛡️ **Guardrail / fact-check** — `yb validate` flags unsupported claims before an agent acts
- ⚡ **KB-grounded semantic cache** — reuse grounded answers with provenance-based auto-invalidation
- 🧠 **Optional ONNX embeddings** — e5 / MiniLM / BGE for true meaning-based recall
- 👥 **Team knowledge** — endorse / dispute with consensus confidence, share via JSONL
- 🔌 **Works in your IDE** — MCP server for Cursor, Claude Code, VS Code & Trae

### ⚡ Quick start

```bash
# Build (needs a Rust toolchain 1.75+)
git clone https://github.com/mrapry/YourBrain yourbrain && cd yourbrain
cargo build --release

# Store and recall knowledge
yb remember "Backend API uses Rust with the Axum web framework" --tag backend
yb recall  "how is the backend built"

# Wire it into your IDE
yb install --ide cursor
```

<div align="center">

**Give your AI agent a memory that doesn't rot → [github.com/mrapry/YourBrain](https://github.com/mrapry/YourBrain)**

</div>

---

<div align="center">

### 📊 GitHub Stats

![mrapry's GitHub stats](https://github-readme-stats.vercel.app/api?username=mrapry&show_icons=true&theme=tokyonight&hide_border=true)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=mrapry&layout=compact&theme=tokyonight&hide_border=true)

</div>

---

<div align="center">

🦀 Rust · 🧠 AI memory · 🗄️ SQLite · 🔌 MCP · 🔒 Local-first

*If YourBrain sounds useful, a ⭐ helps others find it — and PRs are always welcome.*

</div>
