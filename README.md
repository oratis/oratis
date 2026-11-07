### Hi, I'm oratis

I build open-source AI assistants and tools for everyday work. I'm an independent AI researcher focused on memory, long-running tasks, and permission boundaries.

## Projects

**[LISA](https://github.com/oratis/LISA)** — An open-source AI personal assistant for planning, writing, and personal knowledge. Use [LISA Cloud](https://meetlisa.ai/cloud/), or run it on your own Mac.

[Website](https://meetlisa.ai) · [Demo](https://www.youtube.com/watch?v=J_00iwAB_WI) · [Mac app](https://github.com/oratis/LISA/releases/latest) · [npm](https://www.npmjs.com/package/@oratis/lisa) · [Homebrew](https://github.com/oratis/homebrew-tap)

```sh
brew install oratis/tap/lisa
# or
npm install -g @oratis/lisa
```

**[Markup](https://github.com/oratis/Markup)** — A fast, native, open-source Markdown editor for macOS. Read your notes like a web page and edit on demand, with a vault, backlinks, and full-text search.

[Download](https://github.com/oratis/Markup/releases/latest) · [Demo](https://youtu.be/X2_MDL9v7As)

**[DeepCode](https://github.com/oratis/deepcode)** — A DeepSeek-powered coding agent for local codebases. It reads, edits, and runs commands in a repository, with permission boundaries and resumable sessions. The [v0.4.0 release](https://github.com/oratis/deepcode/releases/tag/v0.4.0) includes a VS Code package. That release is not published to npm and does not include a Mac build.

Follow along for releases, demos, and practical engineering notes from these projects.

## Building blocks

Small libraries extracted from [LISA](https://github.com/oratis/LISA).

| Repo | What it does |
| --- | --- |
| **[AsyncSSE](https://github.com/oratis/AsyncSSE)** | Server-Sent Events as a Swift `async`/`await` stream. Point it at an LLM and `for try await` the tokens. Spec-compliant, zero dependencies. |
| **[llm-provider-registry](https://github.com/oratis/llm-provider-registry)** | Map a model name to its API base URL and key environment variable. 16 providers, including Chinese ones the big frameworks skip. Zero dependencies. |
| **[undici-proxy-env](https://github.com/oratis/undici-proxy-env)** | Make Node's built-in `fetch` honor `HTTP(S)_PROXY`, including Clash and corporate proxies that silently break LLM SDKs. |
| **[claude-relay](https://github.com/oratis/claude-relay)** | A transparent Anthropic reverse proxy you can host on Cloud Run. Swap keys at the edge and leave the SDK untouched. |

![oratis's GitHub stats](https://github-readme-stats.vercel.app/api?username=oratis&show_icons=true&hide_border=true&count_private=true)
