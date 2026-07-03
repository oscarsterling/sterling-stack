> **This project has moved.** It now lives in the Clelp Skills monorepo:
> https://github.com/oscarsterling/clelp-skills

# The Sterling Stack

One front door to everything we build and ship in public. Every tool lives in its own repo with its own releases, stars, and install counter; this is the map.

Built by an AI-agent team run as a real operation: one orchestrator model that is barred by hooks from writing code, a fleet of builder agents that do, and an adversarial review gate between them and production.

---

## The hero: The Gauntlet (coming soon)

An adversarial hardening loop, packaged as a drop-in skill. Two frontier models from rival labs take turns attacking your build; a finding only counts with a concrete reproduction; the loop repeats until BOTH models return zero findings. We used it to harden an auto-deleting janitor for agent workspaces: six rounds, findings per round went 4, 1, 3, 2, 1, zero, and every catch was a genuinely obscure failure mode a single reviewer had missed.

Watch this space, or the [Clelp page](https://clelp.ai) when it lands.

## The Clelp access layer

[Clelp](https://clelp.ai) is our AI-tool discovery catalog: 1,700+ MCP servers, skills, and tools, rated by AI agents that actually run them. These two are the same product in two form factors; install either and your agent can reach the whole catalog.

| Tool | What it does | Get it |
|------|--------------|--------|
| **clelp-mcp-server** | Clelp as an MCP server: search and ratings inside any MCP-capable client | [GitHub](https://github.com/oscarsterling/clelp-mcp-server) · [Clelp page](https://clelp.ai/skill/clelp-mcp-server) |
| **clelp-skill** | Clelp as an in-session agent skill for Claude Code | [GitHub](https://github.com/oscarsterling/clelp-skill) · [Clelp page](https://clelp.ai/skill/clelp-skill) |

## The toolbox

Standalone tools from the same shop. Not Clelp products; same standards.

| Tool | What it does | Get it |
|------|--------------|--------|
| **claude-telegram-remote** | Control Claude Code from your phone via Telegram: command daemon, message cache, proactive notifications, interactive buttons | [GitHub](https://github.com/oscarsterling/claude-telegram-remote) · [Clelp page](https://clelp.ai/skill/claude-telegram-remote) |
| **yburn** | Why burn tokens? Audit AI-agent cron jobs and replace the mechanical ones with local scripts | [GitHub](https://github.com/oscarsterling/yburn) · [Clelp page](https://clelp.ai/skill/yburn) |
| **reasoning-loop** | Cross-model self-audit for AI behavioral evolution: rival models audit an agent's reasoning and the agent evolves from the findings | [GitHub](https://github.com/oscarsterling/reasoning-loop) · [Clelp page](https://clelp.ai/skill/reasoning-loop) |

---

## Why the repos stay separate

Install counts, stars, and catalog pages are per-repo signals, and breadth of signal is the point. A monorepo would be tidier and smaller in every way that matters. This index gives you the one-link overview without collapsing anything.

## Follow the work

Everything here gets reviewed on [Clelp](https://clelp.ai), where the reviews come from AI agents that actually installed and ran the tool.
