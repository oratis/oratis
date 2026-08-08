<!--
  DRAFT — not your live profile README. Saved alongside README.md, which is untouched.

  ⚠️ POSITIONING DECISION FOR YOU:
  Your CURRENT live README.md says "Independent AI researcher building LISA" and links meetlisa.ai.
  Your GitHub bio says "Co-Founder at Hakko.ai".
  This draft below uses the "Co-Founder @Hakko.ai" framing. Pick ONE consistent story before publishing:
    (a) Independent researcher / LISA / meetlisa.ai   (matches your current README), or
    (b) AI-agent & LLM-infra builder / Co-Founder @Hakko.ai   (matches your bio, used below).
  Then delete this comment and merge the best of both.
-->

<h1 align="center">Hi, I'm oratis 👋</h1>

<p align="center">
  <b>AI Agent &amp; LLM-infrastructure builder</b> · Co-Founder <a href="https://hakko.ai">@Hakko.ai</a><br/>
  I build autonomous agents and the small, zero-dependency plumbing that makes LLMs reliable in production.
</p>

<p align="center">
  <a href="https://github.com/oratis?tab=repositories&type=source"><img src="https://img.shields.io/badge/original%20repos-48-2ea44f?style=flat-square" alt="original repos"/></a>
  <img src="https://komarev.com/ghpvc/?username=oratis&style=flat-square&color=blue" alt="profile views"/>
  <a href="https://hakko.ai"><img src="https://img.shields.io/badge/Hakko.ai-Co--Founder-black?style=flat-square" alt="Hakko.ai"/></a>
</p>

---

### 🧠 What I work on

- **Autonomous AI agents** with real memory, drives, and self-evolution — see **LISA** ([meetlisa.ai](https://meetlisa.ai)).
- **LLM infrastructure**: provider registries, reverse proxies, proxy-env fixes, SSE streaming, context optimization — the unglamorous layer that keeps agents up.
- **Production AI products**: an ad-automation platform, a native macOS Markdown editor, an agent gateway.
- **Developer tooling** for the Claude Code / agent ecosystem: safety hooks, commit gates, skills.

---

### 🚀 Featured projects

| Project | What it is | Stack |
|---|---|---|
| **[LISA](https://github.com/oratis/LISA)** ⭐6 | An AI agent with a real self — memory, desires, a heartbeat for autonomous action, and dreams it processes while you're away. | TypeScript · MCP · multi-LLM |
| **[adex](https://github.com/oratis/adex)** ⭐6 | AI-powered ad placement &amp; creative-automation platform, running in production. | Next.js 16 · Postgres · GCS · Cloud Run |
| **[Markup](https://github.com/oratis/Markup)** ⭐9 | A fast, native, open-source Markdown editor for macOS — read Markdown like a web page, edit on demand. Vault + backlinks + full-text search. | Tauri 2 · React · Rust |
| **[TakoAPI](https://github.com/oratis/TakoAPI)** | One API to reach every AI agent — an open directory + unified gateway, plus thousands of skills for your coding agent. | Next.js · MCP · A2A |
| **[GPTwiki](https://github.com/oratis/GPTwiki)** | A collaborative encyclopedia where knowledge is written through dialogue with Claude, GPT-4o &amp; Gemini. | TypeScript |

---

### 🧩 Reusable modules (zero-dependency, MIT)

Small, typed, no-dep building blocks I extracted from the products above.

**LLM / AI infra**
- **[llm-provider-registry](https://github.com/oratis/llm-provider-registry)** — map any model name (`glm-4.6`, `deepseek-chat`, `claude-…`, `gpt-…`) → API base URL + key env var. **17 direct providers** incl. the Chinese ones big frameworks skip, **+8 OpenAI-compatible gateways** (OpenRouter/Groq/SiliconFlow/Ollama…), with a `doctor` CLI. Zero deps.
- **[claude-relay](https://github.com/oratis/claude-relay)** — transparent Anthropic API reverse proxy, one-command deploy to Cloud Run. ~130 lines, key stays server-side.
- **[undici-proxy-env](https://github.com/oratis/undici-proxy-env)** — make Node's built-in `fetch` honor `HTTP(S)_PROXY` and survive corporate-proxy response mangling that breaks the Anthropic/OpenAI SDKs.
- **[llm-context-code-stripper](https://github.com/oratis/llm-context-code-stripper)** — strip base64 data-URIs out of source before sending to an LLM; save context &amp; tokens.
- **[AsyncSSE](https://github.com/oratis/AsyncSSE)** — Server-Sent Events for Swift as an `async/await` stream; point it at any LLM endpoint and `for try await` the tokens.
- **[openai-to-anthropic](https://github.com/oratis/openai-to-anthropic)** — put Claude behind an OpenAI-compatible `/v1/chat/completions` endpoint; zero-dep two-way translation incl. function-calling &amp; streaming.
- **[streaming-text-store](https://github.com/oratis/streaming-text-store)** — stream LLM tokens without re-rendering your whole UI; framework-agnostic external store + optional React hook.

**Agent / dev tooling**
- **[claude-code-safety-hooks](https://github.com/oratis/claude-code-safety-hooks)** — drop-in safety hooks for Claude Code: block force-push, lint commits, gate risky deploys, enforce tests.
- **[commit-gate](https://github.com/oratis/commit-gate)** — zero-dep, config-driven Conventional Commits linter for husky/CI.
- **[rate-limit](https://github.com/oratis/rate-limit)** — in-memory sliding-window rate limiter for Node; tiny, typed, self-pruning.
- **[use-draft-autosave](https://github.com/oratis/use-draft-autosave)** — debounced localStorage draft-autosave hook for React; SSR-safe.
- **[react-iframe-game-sdk](https://github.com/oratis/react-iframe-game-sdk)** — React hooks for apps in a sandboxed iframe: sensors, mic level, audio/assets over a host-injected SDK.
- **[pysandbox](https://github.com/oratis/pysandbox)** — run untrusted, user- or agent-generated Python against your data: fork-per-call, `RLIMIT` + wall-clock caps, AST allowlist, JSON-only IPC. Zero-dep core.

**Finance / data**
- **[monthly-fx](https://www.npmjs.com/package/monthly-fx)** — tiny typed FX rates with monthly-average helpers; free ECB data, no API key.
- **[cn-cloud-billing](https://github.com/oratis/cn-cloud-billing)** — one typed API for Alibaba / Tencent / Volcano Engine monthly cloud bills.
- **[purequant](https://github.com/oratis/purequant)** / **[purequant-js](https://github.com/oratis/purequant-js)** — zero-dep quant toolkit (VaR/CVaR, Black-Scholes + Greeks, risk parity) in pure Python &amp; TypeScript.

---

### 🛠️ Tech stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Tauri](https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Model Context Protocol](https://img.shields.io/badge/MCP-000000?style=flat-square&logo=modelcontextprotocol&logoColor=white)

---

### 📊 GitHub stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=oratis&show_icons=true&hide_border=true&count_private=true&theme=default" alt="oratis's GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=oratis&layout=compact&langs_count=8&theme=default" alt="Top languages"/>
</p>

---

<p align="center"><i>Building agents that do real work — and the infrastructure that keeps them running.</i></p>
