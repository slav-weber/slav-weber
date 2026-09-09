# Slava Weber

**Senior Full-Stack Engineer · AI integration · 10 yrs web (PHP, WordPress, JS) · Remote, contract/B2B**

Based in Ukraine, EU time zone (UTC+2/+3). Open to remote roles and contract / B2B engagements, EU time zone or worldwide.

## In progress

Three repositories started from scratch in September 2026, none public yet:

1. `legal-rag-evalset` — measuring an AI system's quality and publishing the numbers together with what they do not show. By hand: 40 gold questions (some the system must refuse) and `metrics.py`; `METHOD.md` written before the questions. The report gives numbers measured on a private predecessor (a Ukrainian legal RAG). Numbers to watch (pending): recall@k, precision@1, hallucination rate, abstain rate.
2. `norm-lookup-mcp` — an MCP server over a statute index where the model can only cite what exists. The statute index and the rejection test are written by hand; FastMCP tooling, packaging and CI are written by a coding agent from my spec. Number to watch: 50/50 fabricated references rejected — pending.
3. `arbiter-kit` v0.1 — "the model decides, code verifies and applies": an agent cannot hand out an item that does not exist or spend money that is not there. A toy world, a strict pydantic response schema (intent plus effect tokens from a closed vocabulary), a hand-written applier, an adversarial-player spec. Number to watch: zero illegal transfers over 200+ hostile turns — adversarial run pending. Inspired by a private game-mod project.

## How I work with coding agents

Two private LLM projects in 2026 (the legal RAG and the game-mod project mentioned above) were built with a coding agent (Claude Code) from specs, acceptance criteria and eval questions I wrote; nearly all of their commits carry the agent's Co-Authored-By trailer.

In the three repositories above, the core module is written by hand and named in that repository's README; the agent types the rest from my spec, and I read every line before accepting it. Agent commits keep their trailers, and each repository's README has a "How this was built" section: files by hand, files by agent, approximate share of lines, what was rejected or rewritten, what was verified by hand and when.

## Background

Slava Weber is the name on every commit from September 2026; earlier agency work is in private repositories under my legal name and a work e-mail.

2016–2026: platform owner at a German digital agency (4eck Media), as an independent contractor. That platform (Dockerised, Composer-managed WordPress with a custom block library) became the foundation of 50+ agency projects. I also worked full-stack in Laravel + Inertia + Vue 3/TypeScript on a large SaaS product, and in 2026 built and rolled out the team's coding-agent harness (skills, path-scoped rules, project memory, self-review gate).

Stack: PHP · WordPress as an engineering platform (custom blocks, headless, Composer) · Laravel · JavaScript/TypeScript · Vue 3 / Nuxt · Docker, CI/CD · since 2026: Python, RAG, evals, MCP.

## Contact

- LinkedIn: https://www.linkedin.com/in/slava-weber/
- Email: slav.weber@gmail.com
- Languages: English (fluent), Ukrainian, Russian
