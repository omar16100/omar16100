# Hi, I'm Omar Shabab

**ML Engineer** building GenAI and ML platforms at scale.

Currently at Singapore's largest grocery retailer, where I build LLM platforms, improve recommendation systems, and computer vision solutions for creatives.

## What I'm Working On

- Systems programming in C and Rust for Apple Silicon (inference kernels, thermal control, SMC/IOKit)
- Local and on-device LLM inference: Metal kernels, GGUF, MLX, benchmarking real hardware limits
- AI developer tooling: MCP servers, CLIs, and a local-first memory graph

## Projects

### Systems & CLI

| Project | Description | Tech |
|---------|-------------|------|
| [atlassian-cli](https://github.com/omar16100/atlassian-cli) | Unified CLI for Jira, Confluence, Bitbucket & JSM. Bulk ops, dry-run, JSON/CSV/YAML output, multi-instance profiles. [Docs](https://atlassiancli.com/) | Rust |
| [surge](https://github.com/omar16100/surge) | LLM inference engine for the Mac Studio M3 Ultra. Limiter-aware pacing scheduler, byte-exact Metal decode, no dependencies beyond macOS. Work in progress | C, Metal |
| [fanpro](https://github.com/omar16100/fanpro) | Fan control and thermal monitoring for Apple Silicon. CLI, TUI and root daemon, zero dependencies | C, IOKit |
| [speedlog](https://github.com/omar16100/speedlog) | Internet speed monitor. One bash script, one HTML file, no Docker, no database | Bash, HTML |
| [batteryconsole](https://github.com/omar16100/batteryconsole) | Logitech MX device battery levels on macOS | Rust |
| [logi_mx_auto_switch](https://github.com/omar16100/logi_mx_auto_switch) | Make an MX Master follow the MX Keys across Macs via HID++ ChangeHost, no Logitech software | Python |

### AI Tooling

| Project | Description | Tech |
|---------|-------------|------|
| [parsnip](https://github.com/omar16100/parsnip) | Local-first memory graph for AI assistants. Single binary, entities/relations/observations, 5 search modes, cross-project queries. [Site](https://omar16100.github.io/parsnip/) | Rust, redb, tantivy, MCP |
| [gemini-mcp-rust](https://github.com/omar16100/gemini-mcp-rust) | MCP server for Google's Gemini API | Rust, MCP |
| [reddit-mcp-server](https://github.com/omar16100/reddit-mcp-server) | Read-only Reddit MCP server over app-only OAuth | Rust, MCP |
| [skills](https://github.com/omar16100/skills) | Custom skills for the Claude Code CLI | Markdown |

### ML & Experiments

| Project | Description | Tech |
|---------|-------------|------|
| [llm-benchmark](https://github.com/omar16100/llm-benchmark) | Local LLM benchmark suite: 26 prompts, 6 categories, programmatic plus LLM-as-judge scoring | Python |
| [bengali-ocr-finetune](https://github.com/omar16100/bengali-ocr-finetune) | Bengali OCR fine-tuning on Apple Silicon with mlx-vlm | Python, MLX |

### Web

| Project | Description | Tech |
|---------|-------------|------|
| [saas_template](https://github.com/omar16100/saas_template) | Cloudflare-first SaaS starter. Opinionated, SEO-first, swappable. [Demo](https://omar16100.github.io/saas_template/) | Next.js 16, D1, Better Auth, Stripe |

*atlassian-cli: 28 stars, 7,217 GitHub release downloads, 541 crates.io downloads (as of 27 Aug 2026).*

## Contributing Elsewhere

Merged: [App-Store-Connect-CLI](https://github.com/rorkai/App-Store-Connect-CLI) (submission validation, localization updates, price point filtering, stale review handling) and [aws-codecommit-devops-model](https://github.com/aws-samples/aws-codecommit-devops-model).

Open: [psd-tools](https://github.com/psd-tools/psd-tools) (drop shadow and outer glow layer effect rendering), [whatsapp-mcp](https://github.com/lharries/whatsapp-mcp) (context-aware whatsmeow API), [HistoryHound](https://github.com/pkmishra/HistoryHound) (stdio transport, Chrome profile detection).

## Tech Stack

**Systems**: Rust, C, Metal, IOKit
**ML/AI**: Python, PyTorch, MLX, GGUF, llama.cpp, Computer Vision, NLP
**AI tooling**: Model Context Protocol (MCP), Claude Code
**Web**: TypeScript, Next.js, Cloudflare Workers/D1
**Cloud**: GCP (Vertex AI, BigQuery, Cloud Functions), AWS (SageMaker, Lambda), Kubernetes, Docker

## Talks & Writing

- [macOS clamps my M3 Ultra's GPU to 338 MHz before the fans even try](https://omarshabab.com/mac-studio-firmware-gpu-limiter/)
- [Kimi-Linear ran a real 1M context on my Mac Studio](https://omarshabab.com/kimi-linear-1m-context/)
- [The two numbers that decide local LLMs: 100 tokens/sec and 1M context](https://omarshabab.com/local-llm-two-numbers/)
- [Local LLM Benchmark: Gemma 4 vs Qwen 3.5](https://omarshabab.com/llm-benchmark/)
- [Serving ML Models Serverlessly](https://www.youtube.com/watch?v=Fon3xvdAKe4) (AWS UG Malaysia)
- [Practical Introduction to NLP](https://github.com/omar16100/Practical-Introduction-To-NLP)

## Connect

- Website: [omarshabab.com](https://omarshabab.com)
- LinkedIn: [/in/omar16100](https://linkedin.com/in/omar16100)
