### Hi, I'm oratis 👋

Independent AI researcher building **[LISA](https://meetlisa.ai)** — a self-evolving, local-first AI agent that runs on your own machine. I care about long-horizon agent coherence, privacy-first design, and shipping small tools that each do one thing well.

#### 🧩 Open-source building blocks — extracted from LISA

| Repo | What it does |
|---|---|
| **[AsyncSSE](https://github.com/oratis/AsyncSSE)** | Server-Sent Events as a Swift `async`/`await` stream — point it at an LLM and `for try await` the tokens. Spec-compliant, zero deps. |
| **[llm-provider-registry](https://github.com/oratis/llm-provider-registry)** | Map any model name → API base URL + key env var. 16 providers incl. the Chinese ones (GLM / DeepSeek / Kimi / Qwen / Doubao …) the big frameworks skip. |
| **[undici-proxy-env](https://github.com/oratis/undici-proxy-env)** | Make Node's built-in `fetch` honor `HTTP(S)_PROXY` — and survive the Clash / corporate-proxy mangling that silently breaks LLM SDKs. |
| **[claude-relay](https://github.com/oratis/claude-relay)** | A transparent Anthropic reverse proxy you can host on Cloud Run — swap keys at the edge, leave the SDK untouched. |

#### 🔬 Currently
- Driving **LISA** toward 1.0 — *Sense · Dispatch · Reve · Model*.
- Researching long-horizon coherence in autonomous agents.

<sub>🌐 [meetlisa.ai](https://meetlisa.ai) · built in the open</sub>

![oratis's GitHub stats](https://github-readme-stats.vercel.app/api?username=oratis&show_icons=true&hide_border=true&count_private=true)
