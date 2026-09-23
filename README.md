# awesome-claude

> **The awesome list for Claude — opinionated, current, no link rot** — hand-curated index of Claude prompts, skills, plugins, tools, integrations, themes, and production resources

<p align="center"><a href="https://github.com/hmzainjamil/awesome-claude">Repository</a> · <a href="https://github.com/hmzainjamil/awesome-claude/commits/main">Commits</a> · <a href="https://github.com/hmzainjamil/awesome-claude/issues">Issues</a></p>
<p align="center"><img alt="Visibility" src="https://img.shields.io/badge/visibility-public-blue"> <img alt="Documentation" src="https://img.shields.io/badge/documentation-deep%20editorial-lightgrey"> <img alt="Lifecycle" src="https://img.shields.io/badge/lifecycle-active-success"></p>

<!-- HMZ DEEP README v1 -->

## At a glance

| Field | Current state |
|---|---|
| Repository | awesome-claude |
| Visibility | Public |
| Lifecycle | Active |
| Evidence basis | Current repository documentation and source-visible material |

## Why this exists

**The awesome list for Claude — opinionated, current, no link rot** — hand-curated index of Claude prompts, skills, plugins, tools, integrations, themes, and production resources

The README presents the repository as a reference collection and separates included material from claims about compatibility, popularity, or production value.

## 🧠 CONCEPTS

Each row maps a concept to a real file. Click `[Source]` to read the actual code.

| # | Concept | Location | Description |
|---|---|---|---|
| 1 | **Curated index** | `README.md` | Hand-curated tables of Claude resources, refreshed quarterly · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/README.md) |
| 2 | **VSCode theme** | `claude-vscode-theme/README.md` | Claude-themed dark + light VSCode themes · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/README.md) |
| 3 | **Theme palette** | `claude-vscode-theme/src/theme/palette.ts` | Color tokens — high-contrast, italic variants · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/src/theme/palette.ts) |
| 4 | **Semantic tokens** | `claude-vscode-theme/src/theme/semanticTokens.ts` | TypeScript-aware semantic highlights · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/src/theme/semanticTokens.ts) |
| 5 | **Token colors** | `claude-vscode-theme/src/theme/tokenColors.ts` | TextMate token scope mappings · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/src/theme/tokenColors.ts) |
| 6 | **C++ tokens** | `claude-vscode-theme/src/theme/tokens/cpp.ts` | Per-language token overrides — C++ · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/src/theme/tokens/cpp.ts) |
| 7 | **Go tokens** | `claude-vscode-theme/src/theme/tokens/golang.ts` | Per-language token overrides — Go · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/src/theme/tokens/golang.ts) |
| 8 | **HTML tokens** | `claude-vscode-theme/src/theme/tokens/html.ts` | Per-language token overrides — HTML · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/src/theme/tokens/html.ts) |
| 9 | **Build script** | `claude-vscode-theme/build.ts` | Compiles palette + tokens into final theme JSON · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/claude-vscode-theme/build.ts) |
| 10 | **Wide banner asset** | `assets/wide.svg` | Hero SVG used in README headers · [Source](https://github.com/hmzainjamil/awesome-claude/blob/main/assets/wide.svg) |

## ⚙️ HOW IT WORKS

```
┌─────────────────────────────────────────────────────────────┐
│  Input  →  awesome-claude  →  Output                                    │
├─────────────────────────────────────────────────────────────┤
│  1. Prompt / file / event lands at the entry point          │
│  2. Manifest resolves trigger → concrete handler            │
│  3. Handler invokes tools / scripts / sub-agents in order   │
│  4. Output is structured (JSON / Markdown / HTML / file)    │
│  5. Side-effects: logs, alerts, artifacts, commits          │
└─────────────────────────────────────────────────────────────┘
```

The architecture is intentionally narrow: one entry point, one router, deterministic handlers. No hidden global state, no `process.env` surprises, no daemons phoning home.

## 🚀 Install

## 🧩 Usage

Once installed, invoke the primary surface from any Claude Code session:

```text
# example 1 — basic trigger
use awesome-claude to ...

# example 2 — explicit skill name
@skill:awesome-claude run on <input>

# example 3 — CLI-style invocation
npx awesome-claude --help
```

Each concept in the table above is independently usable — you don't have to wire the whole thing up at once.

## ⚙️ Configuration

All configuration is file-based. No web dashboards, no SaaS sign-up, no env-var roulette.

| Setting | Default | Description |
|---|---|---|
| `LOG_LEVEL` | `info` | One of: `debug`, `info`, `warn`, `error` |
| `MODEL_TIER` | `tier0` | Route to free local/cloud models before paid |
| `MAX_TOKENS` | `8192` | Hard cap per invocation |
| `CACHE_TTL` | `3600` | Seconds before refetching upstream data |
| `OUTPUT_DIR` | `~/Downloads` | Where generated artifacts land |
| `DRY_RUN` | `false` | Print plan, skip side-effects |
| `RETRY_COUNT` | `3` | Network/transient failure retries |
| `TIMEOUT_MS` | `30000` | Per-call timeout |
| `TELEMETRY` | `off` | Never on by default |
| `VERBOSE_ERRORS` | `true` | Full stacks in dev, redacted in prod |

## Validation and evidence

Each referenced project should be evaluated independently. Inclusion in a collection does not establish that every example is current or tested.

## 🛰️ Security posture

- Secrets: never committed; use a secrets manager (1Password CLI, doppler, age-encrypted .env).
- Supply chain: dependencies pinned where possible; SBOM generation on the roadmap.
- Sandbox: tools that touch the filesystem default to dry-run preview.
- Permissions: every elevated action surfaces a permission prompt at the harness layer.
- Audit log: every tool call appends to a structured log under `~/.claude/`.

## Limitations

- Reference collections can contain projects with different maturity levels.
- External projects can change without notice.
- Quantitative claims require source-specific evidence.



## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)