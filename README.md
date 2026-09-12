# Slava Weber

**Senior Full-Stack Engineer · AI integration · 10 yrs web (PHP, WordPress, JS) · Remote, contract/B2B**

Based in Ukraine, EU time zone (UTC+2/+3). Open to remote roles and contract / B2B engagements, EU time zone or worldwide.

## What I have published

A mod you can play, a renderer that runs in a browser tab, and four public repositories. Each repository holds only what a reader can check: the modules, their tests, and the numbers with the run they came from.

### [Vega AI Mod](https://fallout2vegamod.netlify.app/?lang=en) — a language model plays every character in Fallout 2

The player types whatever they want and the characters answer freely. What the model cannot do is change the world. It returns an intent and effect tokens from a closed vocabulary, and the engine decides every number: skill rolls, whether the player actually carries the item, what a merchant can afford. A character can promise anything; only the engine can make it true.

The public extract of that arbiter is **[llm-npc-arbiter](https://github.com/slav-weber/llm-npc-arbiter)** — one chokepoint for every durable change, a whitelist of designer-authored effects with guards and named invariants, a validated state ledger, a graded dice check, and an adversarial run: **17 hostile turns from the model, zero unauthorised writes to game state**. Standard library only. It ships with the knowledge graph the characters retrieve from, rendered as an interactive map.

That gap is the part I find worth working on — what the model imagines, and what still holds up when someone plays it.

### [Sandsea](https://slav-weber.github.io/sandsea/) — an infinite desert, raymarched in real time

A WebGL2 renderer built from scratch: no engine, no meshes, nothing loaded from disk. The world is a signed distance field raymarched per pixel in the fragment shader — procedural dunes, a day cycle, weather, rain, caves — and every colour comes out of a palette generated in code. The full shader takes about half a minute to link, because the driver unrolls the march, so a small preview shader draws the scene immediately and is swapped out once the real one is ready: first frame in under half a second. Code: **[sandsea](https://github.com/slav-weber/sandsea)**.

### [legal-rag-evals](https://github.com/slav-weber/legal-rag-evals) — retrieval, a citation gate, and the harness that measures both

The retrieval pipeline, citation gate and evaluation harness of a Ukrainian statute RAG. Hybrid retrieval (dense, full-text and lemma channels fused by reciprocal-rank fusion, an exact-lookup route, a cross-encoder reranker); generation where the model may cite only the candidate IDs it was handed, so a fabricated citation is structurally impossible rather than discouraged; and a harness that measures recall@k, precision@1 and MRR per question class, classifies answers, and gates on replay noise measured at temperature 0. **336 tests run offline in one command.** The citation class went from 0.167 to 1.000 recall@10 once exact lookups got a route of their own.

### [agent-review-kit](https://github.com/slav-weber/agent-review-kit) — the acceptance rules those two projects produced

A template repository: one list of gates that CI and the benchmark share, a test ratchet that fails a removed test, seeded-bug catalogues written blind by an agent that never sees the tests, and an agent review layer with a skeptic that has to refute every finding. The numbers are measured, not asserted — in the statute RAG the gates went from **13 of 26** planted bugs to **17 of 20** on a fourth blind catalogue; in the arbiter from **5 of 20** to **12 of 20** on a second; the review layer caught **10 of 10** planted defects with no false alarm in two rounds, the second inside 82-to-250-line refactors carrying several defects each. Every protocol was committed before its run, and every miss is published.

## How I work with coding agents

All of the above was built with a coding agent (Claude Code) from specifications, acceptance criteria and evaluation questions I wrote, and I accepted the work against evidence rather than by eye. Nearly all commits carry the agent's Co-Authored-By trailer, and each repository says plainly how it was built: what was mine, what was the agent's, and what changed when the code was extracted for publication.

What I bring to that work is the part an agent does not supply: where the boundaries go, which invariant must never break, what to measure, and what the numbers do not show.

## Background

Slava Weber is the name on every commit from September 2026; earlier agency work is in private repositories under my legal name and a work e-mail.

2016–2026: platform owner at a German digital agency (4eck Media), as an independent contractor. That platform (Dockerised, Composer-managed WordPress with a custom block library) became the foundation of 50+ agency projects. I also worked full-stack in Laravel + Inertia + Vue 3/TypeScript on a large SaaS product, and in 2026 built and rolled out the team's coding-agent harness (skills, path-scoped rules, project memory, self-review gate).

Stack: PHP · WordPress as an engineering platform (custom blocks, headless, Composer) · Laravel · JavaScript/TypeScript · Vue 3 / Nuxt · WebGL2/GLSL · Docker, CI/CD · since 2026: Python, RAG, evals, MCP.

## Contact

- LinkedIn: https://www.linkedin.com/in/slava-weber/
- Email: slav.weber@gmail.com
- Languages: English (my working language for the last 10 years, daily, in a remote German team), Ukrainian, Russian
