<p align="center">
  <img src="assets/yana-profile-hero.svg" alt="Vũ Văn Tâm — creator of Yana AI" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/yanacuti1121/Yana-AI"><strong>Yana AI</strong></a> ·
  <a href="https://yanacuti1121.github.io/Yana-AI/">Documentation</a> ·
  <a href="https://yanacuti1121.github.io/Yana-AI/desktop.html">Desktop App</a> ·
  <a href="https://crates.io/crates/yana-rt">Rust Runtime</a> ·
  <a href="https://pypi.org/project/yana-ai/">Python CLI</a>
</p>

<p align="center">
  <a href="https://github.com/yanacuti1121/Yana-AI/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/yanacuti1121/Yana-AI/ci.yml?branch=main&style=flat-square&label=Yana%20CI&color=ff7ab6" alt="Yana AI CI" /></a>
  <a href="https://crates.io/crates/yana-rt"><img src="https://img.shields.io/crates/v/yana-rt?style=flat-square&logo=rust&color=c084fc" alt="yana-rt on crates.io" /></a>
  <a href="https://pypi.org/project/yana-ai/"><img src="https://img.shields.io/pypi/v/yana-ai?style=flat-square&logo=pypi&color=22d3ee" alt="yana-ai on PyPI" /></a>
  <a href="https://github.com/yanacuti1121/Yana-AI/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-fbbf24?style=flat-square" alt="Apache 2.0 license" /></a>
</p>

---

## Xin chào — I’m Vũ Văn Tâm

I am a Vietnamese developer based in South Korea and the person behind **Yana AI**.

I started this system as a collection of files and personal automation rules under the name **YAMTAM**. It grew into a cross-platform AI runtime, governance layer, terminal workspace, desktop application, memory system, and operating plane for AI agents. I design and maintain that system in public.

My role in Yana AI is not limited to writing code:

| Product direction | System architecture | Engineering | Human governance |
|---|---|---|---|
| I decide what Yana should become and which problems it should refuse to solve. | I shape the boundaries between `yana-rt`, providers, adapters, capabilities, memory, Yana OS, and agent interfaces. | I build, review, test, release, investigate failures, and maintain the project across Rust, Python, Shell, and JavaScript. | I remain the final authority for destructive actions, releases, security trade-offs, and changes that affect user control. |

I work with Claude, Codex, Gemini, local models, and specialist agents as engineering collaborators. They help implement, review, test, and challenge decisions; they do not replace project ownership or human responsibility. AI-authored work is credited in Git history whenever possible.

> **My job is to make AI more capable without quietly making the human less in control.**

---

## What I am building

<h3 align="center">Yana AI 🐰</h3>
<p align="center"><strong>One runtime. Any AI. Human-governed.</strong></p>
<p align="center"><em>Build with AI. Govern what it builds.</em></p>

<p align="center">
  <img src="assets/yana-ai-key-visual.png" alt="Yana AI — Control, Verify, Protect" width="640" />
</p>

Yana AI is a **local-first, cross-platform control and runtime system for AI**. It connects local models, cloud models, coding agents, project tools, memory, and automation to one native execution layer while keeping deterministic policy and human authority in the path.

It is not a foundation model and it is not tied to one provider. Yana does not try to replace Claude, Codex, Cursor, Ollama, LM Studio, or llama.cpp. It gives them a shared runtime and a governed boundary for what they may inspect, change, and execute.

<p align="center">
  <img src="assets/yana-architecture.svg" alt="Yana AI architecture" width="100%" />
</p>

### The problem

AI can now read repositories, edit files, run commands, launch agents, call tools, and prepare releases. Intelligence is improving quickly, but operational control is still fragmented:

- each model or coding agent invents a different workflow;
- tool permissions are often mixed directly into UI or provider code;
- “safe”, “done”, and “approved” are frequently claims without evidence;
- local models and cloud models do not naturally share one governed execution layer;
- automation can become more autonomous without a clear boundary for when a human must decide.

Yana turns those questions into runtime behavior rather than policy text alone.

### The system

| Layer | What it does |
|---|---|
| **`yana-rt`** | The native Rust core for chat, capabilities, routing, missions, memory, evidence, workspace operations, host health, and runtime coordination. |
| **Model providers** | Connect local and cloud inference without spreading provider-specific logic throughout the interface. |
| **Project adapters** | Bring the same governed project contract to Claude Code, Codex, Cursor, and Antigravity. |
| **Capability runtime** | Centralizes repository, Git, host, process, and command operations so every interface uses the same boundary. |
| **Deterministic gates** | Check risky operations, scope, truth claims, destructive commands, integrity, and release evidence without asking another LLM to decide. |
| **Memory and evidence** | Preserve project facts, session context, turn history, receipts, and audit trails while keeping local-first defaults. |
| **Yana OS + Giám Thị** | Supervise the runtime and host, expose health, support HALT/quarantine flows, and keep high-autonomy behavior subordinate to human unlock. |
| **Terminal + Desktop** | Give the same core a keyboard-first local AI workspace and a graphical application rather than building separate brains for each UI. |

### What exists today

- A Rust runtime with native chat, streaming, cancellation, sessions, routing, missions, capabilities, health, workspace, and OS surfaces.
- Local model paths for Ollama, LM Studio, llama.cpp, and compatible local endpoints, alongside cloud-provider integrations.
- Project adapters for Claude Code, Codex, Cursor, and Antigravity.
- More than **2,000 skills**, **100 specialist agents**, **170 commands**, and **60 deterministic hooks** maintained from canonical sources.
- A multi-platform Electron desktop application and a Rust terminal chat experience connected to the same runtime direction.
- Project memory, evidence, audit, integrity, quarantine, and human approval mechanisms.
- Cross-platform work targeting macOS, Linux, and Windows.

These numbers describe a fast-moving project, not a promise that every surface has equal maturity. I keep architecture-health reports and known limitations public because runtime truth matters more than a large feature count.

---

## What makes Yana different

<table>
<tr>
<td width="25%" valign="top">

### ◆ Local-first

Local inference, project state, memory, and deterministic checks should work without mandatory telemetry or a cloud control plane.

</td>
<td width="25%" valign="top">

### ◇ Provider-neutral

The UI talks to runtime abstractions, not provider-specific code scattered across the product.

</td>
<td width="25%" valign="top">

### ◈ Deterministic

Safety-critical decisions use inspectable code, explicit gates, evidence, and reproducible tests—not another model’s confidence.

</td>
<td width="25%" valign="top">

### ◎ Human-governed

Higher autonomy requires stronger evidence and clearer human authority, not fewer controls.

</td>
</tr>
</table>

Yana’s autonomy model is intentionally asymmetric: routine work should become automatic, while irreversible or high-impact actions stay human-controlled.

```text
Observe → Recommend → Prepare → Execute safely → Escalate high-impact decisions
                                                  ↑
                                         human authority remains
```

---

## My responsibility inside the project

### I define the direction

I decide the product principles, the autonomy boundary, which runtimes and interfaces belong in Yana, and where the project should remain deliberately conservative.

### I protect the architecture

`yana-rt` is the deepest core. Terminal chat, desktop UI, project adapters, MCP surfaces, and future interfaces should converge on its capabilities rather than create independent execution paths. When duplicate implementations appear, I treat that as architectural debt.

### I operate the system

I investigate CI failures, release breakage, packaging gaps, hook races, platform differences, runtime regressions, and drift between documentation and executable behavior. A feature is not complete because its file exists; it must be reachable, wired, tested, packaged, and observable.

### I make the final call

Agents can propose architecture, write patches, review code, and run verification. I decide whether high-impact changes ship. Yana’s own development process follows the same philosophy the product enforces: **AI can act, but human authority defines how far it may go.**

---

## Current engineering focus

- Making the capability runtime the single source of truth across chat, MCP, project tools, and host operations.
- Deepening `yana-rt` integration so terminal and desktop interfaces share one runtime rather than duplicate behavior.
- Improving local AI sessions, memory recall, context management, model switching, and provider health.
- Building reliable cross-platform supervision for CPU, GPU, process, service, and Yana system health.
- Making releases reproducible without depending exclusively on GitHub-hosted automation.
- Raising autonomy for routine work while preserving explicit human gates for destructive, security-sensitive, and production actions.
- Continuously separating what is truly wired from what is only implemented, documented, experimental, or planned.

---

## Main project surfaces

| Surface | Purpose | Link |
|---|---|---|
| **Yana AI** | Main runtime, governance system, adapters, hooks, agents, skills, and documentation | [Repository](https://github.com/yanacuti1121/Yana-AI) |
| **Yana Desktop** | Cross-platform graphical AI workspace connected to the Yana runtime | [Download](https://yanacuti1121.github.io/Yana-AI/desktop.html) |
| **Yana Local Chat** | Rust terminal-native workspace for local and connected AI models | [Source](https://github.com/yanacuti1121/Yana-AI/tree/main/src/chat) |
| **`yana-rt`** | Native Rust runtime and CLI | [crates.io](https://crates.io/crates/yana-rt) |
| **`yana-ai`** | Python installer and project adapter CLI | [PyPI](https://pypi.org/project/yana-ai/) |
| **Documentation** | Architecture, installation, operations, limitations, and contribution guides | [Open docs](https://yanacuti1121.github.io/Yana-AI/) |
| **Yana GitHub App** | Repository-facing GitHub integration | [Install](https://github.com/apps/yana-ai-bot) |
| **CodexMate** | Companion dashboard for AI coding tools | [Project](https://sakurabytecore.github.io/codexmate/) |

---

## How I build

```text
Build > Talk
Ship > Promise
Verify > Assume
Evidence > Confidence
Human authority > silent autonomy
```

I use AI heavily, but I do not treat AI output as truth. My workflow emphasizes:

- inspect the real code before making architectural claims;
- test the execution path, not only isolated helpers;
- record authorship and review evidence;
- publish known limitations instead of hiding unfinished wiring;
- prefer small reversible changes over impressive but fragile rewrites;
- keep destructive and production actions explicitly human-gated.

---

## Technology

<p>
  <img src="https://img.shields.io/badge/Rust-160b24?style=for-the-badge&logo=rust&logoColor=fff7fb" alt="Rust" />
  <img src="https://img.shields.io/badge/Python-ff7ab6?style=for-the-badge&logo=python&logoColor=160b24" alt="Python" />
  <img src="https://img.shields.io/badge/Shell-c084fc?style=for-the-badge&logo=gnu-bash&logoColor=ffffff" alt="Shell" />
  <img src="https://img.shields.io/badge/JavaScript-fbbf24?style=for-the-badge&logo=javascript&logoColor=160b24" alt="JavaScript" />
  <img src="https://img.shields.io/badge/TypeScript-67e8f9?style=for-the-badge&logo=typescript&logoColor=160b24" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Electron-a78bfa?style=for-the-badge&logo=electron&logoColor=ffffff" alt="Electron" />
</p>

My strongest interest is not a single language. It is the boundary between **AI intelligence, native systems, developer tools, automation, and human control**.

---

## Open source and collaboration

Yana AI learns from open-source projects, research, runtime patterns, and real operational failures. When an upstream project directly influences an implementation, I aim to preserve license information and attribution in the relevant source or documentation.

Contributions are welcome—especially from people interested in Rust runtimes, local AI, terminal interfaces, cross-platform systems, safety engineering, reproducible releases, and human-centered automation.

<p align="center">
  <a href="https://github.com/yanacuti1121/Yana-AI/issues"><img src="https://img.shields.io/badge/Open_an_issue-ff7ab6?style=for-the-badge&logo=github&logoColor=160b24" alt="Open an issue" /></a>
  <a href="https://github.com/yanacuti1121/Yana-AI/blob/main/CONTRIBUTING.md"><img src="https://img.shields.io/badge/Contribute-c084fc?style=for-the-badge&logo=git&logoColor=ffffff" alt="Contribute" /></a>
  <a href="https://github.com/sponsors/yanacuti1121"><img src="https://img.shields.io/badge/Sponsor-67e8f9?style=for-the-badge&logo=githubsponsors&logoColor=160b24" alt="Sponsor" /></a>
</p>

---

## Contact

| | |
|---|---|
| GitHub | [@yanacuti1121](https://github.com/yanacuti1121) |
| Email | [phamlongh230@gmail.com](mailto:phamlongh230@gmail.com) |
| Website | [Yana AI Documentation](https://yanacuti1121.github.io/Yana-AI/) |
| TikTok | [@yana018](https://www.tiktok.com/@.yana018) |

<p align="center">
  <strong>Your AI can act. But who decides how far it can go?</strong><br />
  <sub>I am building Yana AI so that answer remains visible, inspectable, and human.</sub>
</p>
