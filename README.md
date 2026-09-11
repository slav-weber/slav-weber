# Slava Weber

**Senior Full-Stack Engineer · AI integration · 10 yrs web (PHP, WordPress, JS) · Remote, contract/B2B**

Based in Ukraine, EU time zone (UTC+2/+3). Open to remote roles and contract / B2B engagements, EU time zone or worldwide.

## Published

Two repositories carved out of the private LLM systems I built in 2026. Each contains only what a reader can check: the modules, their tests, and the numbers with the run they came from.

**[legal-rag-evals](https://github.com/slav-weber/legal-rag-evals)** — the retrieval pipeline, citation gate and evaluation harness of a Ukrainian statute RAG. Hybrid retrieval (dense, full-text and lemma channels fused by reciprocal-rank fusion, an exact-lookup route, a cross-encoder reranker); generation where the model may cite only the candidate IDs it was handed, so a fabricated citation is structurally impossible rather than discouraged; and a harness that measures recall@k, precision@1 and MRR per question class, classifies answers, and gates on replay noise measured at temperature 0. 280 tests run offline in one command. The citation class went from 0.167 to 1.000 recall@10 once exact lookups got a route of their own.

**[llm-npc-arbiter](https://github.com/slav-weber/llm-npc-arbiter)** — the decision layer of a game mod where a language model plays every character. The model decides; code verifies and applies. One chokepoint for every durable change, a whitelist of designer-authored effects with guards and named invariants, a validated state ledger, a graded dice check, and an adversarial run of hostile model turns: 17 attempts, zero unauthorised writes. Standard library only. Includes the knowledge graph the characters retrieve from, rendered as an interactive map.

## How I work with coding agents

Both systems were built with a coding agent (Claude Code) from specifications, acceptance criteria and evaluation questions I wrote, and I accepted the work against evidence rather than by eye. Nearly all of their commits carry the agent's Co-Authored-By trailer, and each repository's README has a "How this was built" section that says what was mine, what was the agent's, and what changed when the code was extracted for publication.

What I bring to that work is the part an agent does not supply: where the boundaries go, which invariant must never break, what to measure, and what the numbers do not show.

## Background

Slava Weber is the name on every commit from September 2026; earlier agency work is in private repositories under my legal name and a work e-mail.

2016–2026: platform owner at a German digital agency (4eck Media), as an independent contractor. That platform (Dockerised, Composer-managed WordPress with a custom block library) became the foundation of 50+ agency projects. I also worked full-stack in Laravel + Inertia + Vue 3/TypeScript on a large SaaS product, and in 2026 built and rolled out the team's coding-agent harness (skills, path-scoped rules, project memory, self-review gate).

Stack: PHP · WordPress as an engineering platform (custom blocks, headless, Composer) · Laravel · JavaScript/TypeScript · Vue 3 / Nuxt · Docker, CI/CD · since 2026: Python, RAG, evals, MCP.

## Contact

- LinkedIn: https://www.linkedin.com/in/slava-weber/
- Email: slav.weber@gmail.com
- Languages: English (my working language for the last 10 years, daily, in a remote German team), Ukrainian, Russian
