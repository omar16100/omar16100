# Hi, I'm Omar Shabab

**ML Engineer** building GenAI and ML platforms.

## What I'm Working On

- Systems programming in C and Rust for Apple Silicon (inference kernels, thermal control, SMC/IOKit)
- Local and on-device LLM inference: Metal kernels, GGUF, MLX, benchmarking on real hardware
- AI developer tooling: MCP servers, CLIs, and a local-first memory graph

## Projects

### Systems & CLI

| Project | Description | Tech |
|---------|-------------|------|
| [atlassian-cli](https://github.com/omar16100/atlassian-cli) | Unified CLI for Jira, Confluence, Bitbucket & JSM. Bulk ops, dry-run, JSON/CSV/YAML/table output, multi-instance profiles. [Docs](https://atlassian-cli.pages.dev) | Rust |
| [surge](https://github.com/omar16100/surge) | Experimental LLM inference engine for the Mac Studio M3 Ultra. Byte-exact greedy Metal decode, no dependencies beyond macOS. Work in progress, and so far slower than mlx-lm and llama.cpp on the workloads measured | C, Metal |
| [fanpro](https://github.com/omar16100/fanpro) | Fan control and thermal monitoring for Apple Silicon Macs. CLI, live terminal dashboard and root daemon, monitor-only by default, no dependencies beyond macOS | C, IOKit |
| [speedlog](https://github.com/omar16100/speedlog) | Self-hosted internet speed monitor: a bash collector logs Ookla Speedtest CLI results to CSV and a FastAPI app serves a Chart.js dashboard. No database, no Docker | Bash, Python, Chart.js |
| [batteryconsole](https://github.com/omar16100/batteryconsole) | CLI to check Logitech MX device battery levels on macOS, over the BLE Battery Service or HID++ | Rust |
| [logi_mx_auto_switch](https://github.com/omar16100/logi_mx_auto_switch) | Make an MX Master follow the MX Keys across Macs on Easy-Switch via HID++ ChangeHost, no Logitech software | Python |
| [localsecrets](https://github.com/omar16100/localsecrets) | Small self-hosted secrets manager: single-binary server and CLI, Shamir unseal shares, append-only encrypted store, scoped machine tokens | Rust |
| [beacon-hunt](https://github.com/omar16100/beacon-hunt) | Passive Bluetooth tools for finding a lost Apple device indoors, when Find My has only given you a street address | Python, bleak |

### Apps

| Project | Description | Tech |
|---------|-------------|------|
| [openpos](https://github.com/omar16100/openpos) | Offline-first point of sale for small retail shops: one Rust core shared by the till, the browser and the server, so a shop keeps selling with the line down. Pre-release, AGPL-3.0-only | Rust, WASM, Svelte, Postgres |
| [cron_manager](https://github.com/omar16100/cron_manager) | Native desktop GUI for managing your crontab: visual schedule builder, next-run preview, conflict detection and automatic backups. [Site](https://omar16100.github.io/cron_manager/) | Rust, iced |
| [usagebar-no-tel](https://github.com/omar16100/usagebar-no-tel) | Unofficial no-telemetry fork of [robinebers/openusage](https://github.com/robinebers/openusage) (v0.7.10), a macOS menu bar app that tracks AI coding subscription usage. Not affiliated with or endorsed by OpenUsage | Swift |

### AI Tooling

| Project | Description | Tech |
|---------|-------------|------|
| [parsnip](https://github.com/omar16100/parsnip) | Local-first memory graph for AI assistants. Single binary, entities/relations/observations, exact, fuzzy and full-text search, MCP integration, cross-project queries, optional remote mode (source builds). [Site](https://omar16100.github.io/parsnip/) | Rust, redb, tantivy, MCP |
| [gemini-mcp-rust](https://github.com/omar16100/gemini-mcp-rust) | MCP server for Google's Gemini API, written in Rust | Rust, MCP |
| [reddit-mcp-server](https://github.com/omar16100/reddit-mcp-server) | Read-only Reddit MCP server over app-only OAuth | Rust, MCP |
| [skills](https://github.com/omar16100/skills) | Custom skills for the Claude Code CLI | Markdown |

### ML & Experiments

| Project | Description | Tech |
|---------|-------------|------|
| [llm-benchmark](https://github.com/omar16100/llm-benchmark) | Local LLM benchmark suite: 26 prompts across 6 categories, programmatic and Claude-as-judge scoring, plus long-context needle-in-a-haystack harnesses | Python |
| [bengali-ocr-finetune](https://github.com/omar16100/bengali-ocr-finetune) | Bengali OCR LoRA fine-tuning experiments (Gemma 4 E4B, PaddleOCR-VL-1.5) on Apple Silicon. Research log | Python, MLX, mlx-vlm |

### Web

| Project | Description | Tech |
|---------|-------------|------|
| [saas_template](https://github.com/omar16100/saas_template) | Cloudflare-first SaaS starter. Opinionated, SEO-first, swappable. [Site](https://omar16100.github.io/saas_template/) | Next.js 16, D1, Better Auth, Stripe |

*atlassian-cli: 30 GitHub stars, 8,911 GitHub release asset downloads, 666 crates.io downloads of the `atlassian-cli` crate (as of 27 Sep 2026).*

## Contributing Elsewhere

Merged: [App-Store-Connect-CLI](https://github.com/rorkai/App-Store-Connect-CLI) ([#739](https://github.com/rorkai/App-Store-Connect-CLI/pull/739) to [#743](https://github.com/rorkai/App-Store-Connect-CLI/pull/743): submission validation, localization updates, price point filtering, stale review submission handling, app privacy error hints) and [aws-codecommit-devops-model](https://github.com/aws-samples/aws-codecommit-devops-model) ([#4](https://github.com/aws-samples/aws-codecommit-devops-model/pull/4): Docker install prerequisite).

Open (as of 27 Sep 2026): [psd-tools #679](https://github.com/psd-tools/psd-tools/pull/679) (drop shadow layer effect rendering), [whatsapp-mcp #363](https://github.com/lharries/whatsapp-mcp/pull/363) (move to the context-aware whatsmeow API), [HistoryHound #12](https://github.com/pkmishra/HistoryHound/pull/12) (stdio transport, Chrome profile detection fix).

## Tech Stack

**Systems**: Rust, C, Metal, IOKit
**ML/AI**: Python, PyTorch, MLX, GGUF, llama.cpp, Computer Vision, NLP
**AI tooling**: Model Context Protocol (MCP), Claude Code
**Web**: TypeScript, Next.js, Cloudflare Workers/D1
**Cloud**: GCP (Vertex AI, BigQuery, Cloud Functions), AWS (SageMaker, Lambda), Kubernetes, Docker

## Talks & Writing

- [Write-up on M3 Ultra GPU clock drops under sustained LLM load](https://omarshabab.com/mac-studio-firmware-gpu-limiter/). It proposed a 338 MHz firmware GPU limiter; surge's own later telemetry did not support that premise ([retraction](https://github.com/omar16100/surge#the-gpu-limiter-premise-retracted))
- [Kimi-Linear ran a real 1M context on my Mac Studio](https://omarshabab.com/kimi-linear-1m-context/)
- [The two numbers that decide local LLMs: 100 tokens/sec and 1M context](https://omarshabab.com/local-llm-two-numbers/)
- [Serving Machine Learning Models in a Serverless Manner](https://www.youtube.com/watch?v=Fon3xvdAKe4): talk in the AWS User Group Malaysia March 2021 livestream (the link is the full stream)
- [Practical Introduction to NLP](https://github.com/omar16100/Practical-Introduction-To-NLP)

## Connect

- Website: [omarshabab.com](https://omarshabab.com)
- LinkedIn: [/in/omar16100](https://linkedin.com/in/omar16100)
