# Joseph Soper

**Software, Solutions and Support Engineer · Agentic AI and AI implementation · Python, Google Cloud, Linux**

I've spent my life building hardware and software, with more than 20 years as a hobbyist developer, and the last few years going deep on AI: agentic systems, context engineering and AI implementation. I'm looking for a remote, full-time role in software, AI, cloud or DevOps engineering, in solutions or implementation engineering, or in support engineering at a company that builds for developers.

I learned my first programming language 26 years ago and never stopped: hardware builds, more than 20 years of Linux, servers, networks, and now a private cloud on my own hardware. I run [BezaCore Labs](https://github.com/BezaCore-Labs), the studio where I build the projects below.

[soper.dev](https://soper.dev) · [LinkedIn](https://www.linkedin.com/in/joseph-soper-dev/) · [joseph@soper.dev](mailto:joseph@soper.dev)

## Projects

### [Never4gA](https://github.com/BezaCore-Labs/never4ga)

Open-source context and memory for AI coding agents, in Python, on [PyPI](https://pypi.org/project/never4ga/) under Apache-2.0. Agents start each session knowing nothing about a project, and memory tools usually answer that by asking a model what's relevant. Never4gA does that work with logic: it resolves the repository to its project, pulls that project's documents by type and metadata, runs BM25 full-text search, follows document links, fuses the results with reciprocal rank fusion, and assembles a context pack held to a strict budget, where every item says why it's there. A command line, a REST API and an MCP server share one core. I built vector search into it too, measured it against full-text search, and took it out: [why I removed the vector search lane](https://soper.dev/removing-the-vector-lane/).

*Python · FastAPI · SQLite · MCP*

### [BezaForge](https://github.com/thejollydev/bezaforge-infrastructure)

My studio's private cloud, on my own hardware and managed entirely as code. Terraform declares the Proxmox virtual machines and Ansible configures every host and service, so the whole environment can be rebuilt from the repository. Services run in Docker behind Traefik over segmented VLANs, with WireGuard for remote access. It hosts the studio's Git, project tracking and ERP, and a local AI stack with Ollama on a passed-through GPU and Langfuse tracing LLM calls. Prometheus, Grafana and Loki watch all of it, and encrypted backups go off-site every day.

*Terraform · Ansible · Docker · Proxmox · Prometheus · Grafana*

### [Petoskey Church of Christ](https://petoskeychurchofchrist.com)

The WordPress publishing platform a small church runs on, built pro bono and supported in production. The pastor writes the week once, and it becomes the website, the Sunday email and a print bulletin that sizes its own type to fit the page. Around that sit two-way Google Calendar sync and sermon videos through the YouTube Data API. Custom PHP and JavaScript, developed in local Docker, verified on staging and deployed by script. The repository is private.

*WordPress · PHP · JavaScript · MySQL · Google APIs*

### Intelligrace

Operations software for small churches and nonprofits, in development. One modular Django application with Next.js and Expo clients, where every record belongs to an organization, enforced by PostgreSQL row-level security, with field-level encryption on sensitive records. Its AI layer can change providers, stays off by default for private records, and requires approval on anything AI wrote. The Google Cloud foundation is built in Terraform. The repository is private; I'm glad to walk through it.

*Django · Next.js · PostgreSQL · Google Cloud · Terraform*

### [ansible-arch](https://github.com/thejollydev/ansible-arch)

One idempotent Ansible playbook that provisions my Arch Linux workstations end to end: packages, AUR, dotfiles, services and system configuration, with per-host feature flags.

*Ansible · Arch Linux*

## What I do with AI

I use local and frontier models and agentic AI daily, and I build the systems around them: agentic teams for real problems, MCP servers, agent skills, persistent agent memory, and a multi-model LangGraph workflow with human approval. I run local inference with Ollama on my own GPU, trace LLM calls, tokens and cost in Langfuse, and measure retrieval with Recall@k and MRR. I also know where AI doesn't belong, and measure before I decide.

## Background

Nine years in consultative sales taught me to find out what a customer actually needs. Support at AppleCare and Tier 2 at Intuit taught me to work from logs to root causes and take customers through database migrations and server installations.

- Google Cloud Associate Cloud Engineer
- IBM Back-End Development Professional Certificate
- B.S. in Computer Science, University of the People, expected December 2027

**Stack:** Python, FastAPI, Django, SQL, PostgreSQL, SQLite, Bash, Git, GitHub Actions · Linux, Docker, Terraform, Ansible, Proxmox, Traefik, Prometheus, Grafana · Google Cloud, Cloud Run · WordPress, PHP, JavaScript, Next.js · MCP, LangGraph, Ollama, Langfuse
