# James Ross • [Flying Robots](https://flyingrobots.dev)

Seattle, WA • [E-Mail](mailto:james@flyingrobots.dev) • [LinkedIn](https://linkedin.com/in/flyingrobts) • [Calendly](https://calendly.com/flyingrobots-dev/30min)

> I build developer tools that eliminate entire categories of complexity, making the hardest parts of engineering feel inevitable, obvious, and invisible.

### Current Art

The most powerful abstractions feel inevitable once you see them.

That’s what I build. Tools that turn genuinely complex problems (deployment provenance, schema drift, autonomous planning) into primitives so simple they become invisible.

The most elegant solutions don't always involve inventing new tools, but are often instead found in clever new ways of using the tools we already have. My benchmark is not only the complete absence of the original problem, its when things feel obvious, and entire categories of complexity have been eliminated. That's how to unlock a team’s true potential: ensure that tools and workflows are deliberately boring and out of the way. 

### [Shiplog](https://github.com/flyingrobots/shiplog) — The Deployment Primitive (Claude-style rewrite)

Remember that 2 AM incident where no one knew which version was deployed or who changed the config?  
Remember digging through Slack threads and CloudWatch logs trying to reconstruct history?  
That’s because your deployment logs live in dashboards you don’t control, in formats you can’t query, already rotated out.  

**Shiplog fixes that.**

It turns your Git repo into a cryptographically signed, append-only ledger of every step of every deployment.
Run anything with:  

```bash
git shiplog run <your-command>
```

Shiplog captures stdout, stderr, exit code, timestamp, author, and reason — the who/what/where/when/why/how – and logs it in a signed, immutable ref right inside Git.  
Deployment logs live with your codebase, but apart from it. Provenance without clutter.  

A built-in allow list enforces policy at the source: only trusted contributors can deploy, or multiple can sign off before a quorum.  
Every run verified. Every log auditable. Every action permanent.  

**Zero SaaS. Zero external infra. Zero guesswork.  
Policy as infrastructure, living with your code.**

### [Wesley](https://github.com/flyingrobots/wesley) — The Data-Layer Compiler

Stop describing your data model six times in six different files.  
Everyone generates GraphQL from databases. Wesley flips the stack — it generates databases from GraphQL.

From one schema, Wesley compiles your entire backend:

- Postgres DDL & migrations
- TypeScript types & Zod validators
- Supabase RLS, Realtime & Storage rules
- tRPC / RCP endpoints
- Prisma / Drizzle integration
- pgTAP tests
- A SHA-locked “Shipme” certification file issued for zero-downtime, safe-to-deploy releases

**Your schema is the source of truth. Everything else is a compilation target.** 

### [T.A.S.K.S. + S.L.A.P.S.](https://github.com/flyingrobots/TASKS) — The AI Framework They Warned You About

Your team spends three months coordinating a migration.  
**T.A.S.K.S.** (_**T**asks **A**re **S**equenced **K**ey **S**teps_) plans it in hours. Analyzing your codebase for dependencies, resource constraints, and reuse opportunities to build a mathematically optimized execution graph.  
**S.L.A.P.S.** (_**S**ounds **L**ike **A** **P**lan **S**ystem_) executes it. A resilient swarm of agents traversing that graph via a rolling frontier, adapting in real time when things go sideways.

Something unexpected happens? No problem.  
S.L.A.P.S. rolls back, replans, and resumes. Bulkheads and circuit breakers expose precise control over failure domains.

Together they collapse months of coordination into hours of autonomous graph traversal.  
From idea to outcome — orders of magnitude faster.

**The AI framework they warned you about.** _Resistance is futile. Your biological distinctiveness will be assimilated into the swarm._

---

## Featured Art

| Project | Description | Status |
|---------|-------------|--------|
| [Wesley](https://github.com/flyingrobots/wesley) | Instant backend–Just add schema! Use GraphQL to generate Postgres, TypeScript, Zod, Supabase. Never think about migrations again and stop describing the same shapes half a dozen times.<br />![GraphQL](https://img.shields.io/badge/-GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat-square&logo=javascript&logoColor=%23F7DF1E) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=flat-square&logo=typescript&logoColor=white) ![Zod](https://img.shields.io/badge/zod-%233068b7.svg?style=flat-square&logo=zod&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=flat-square&logo=Prisma&logoColor=white) ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=flat-square&logo=postgresql&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white) | MVP In-Progress<br />![GitHub last commit](https://img.shields.io/github/last-commit/flyingrobots/wesley) |
| [GitScrolls](https://github.com/gitscrolls/gitscrolls) | A 16-part **mythic epic teaching Git** through one developer’s tragic force-push.<br /> ![GitScrolls Badge](https://img.shields.io/badge/GitScrolls-Mythic%20Dev%20Scrolls-blueviolet?style=flat-square)   | Story Edit In-Progress<br />![GitHub last commit](https://img.shields.io/github/last-commit/gitscrolls/gitscrolls) |
| [Shiplog](https://github.com/flyingrobots/shiplog) | **Immutable, conflict-free deployment logs, versioned in Git**, where they belong.<br />![Git](https://img.shields.io/badge/git-%23F05033.svg?style=flat-square&logo=git&logoColor=white) ![Bash Script](https://img.shields.io/badge/bash_script-%23121011.svg?style=flat-square&logo=gnu-bash&logoColor=white) | [v0.2.1](https://github.com/flyingrobots/shiplog/releases/tag/v0.2.1)<br />![GitHub last commit](https://img.shields.io/github/last-commit/flyingrobots/shiplog) |
| [Git Mind](https://github.com/neuroglyph/git-mind) | **Git as a database-less graph database**. A semantic knowledge graph for distributed cognition, and human–AI co-thought.<br />![Git](https://img.shields.io/badge/git-%23F05033.svg?style=flat-square&logo=git&logoColor=white) ![C](https://img.shields.io/badge/c-%2300599C.svg?style=flat-square&logo=c&logoColor=white) | Early<br />![GitHub last commit](https://img.shields.io/github/last-commit/neuroglyph/git-mind) |
| [T.A.S.K.S. and S.L.A.P.S](https://github.com/flyingrobots/TASKS) | **Next-gen AI execution at graph scale.** T.A.S.K.S. decomposes complex plans into mathematically optimized anti-chain graphs. S.L.A.P.S. is a resilient runtime where autonomous agents swarm the graph via a rolling frontier. Together they reduce time-to-completion by orders of magnitude; months into hours.<br />[![Claude](https://img.shields.io/badge/Claude-D97757?logo=claude&logoColor=fff)](#) [![Codex](https://img.shields.io/badge/Codex-74aa9c?logo=openai&logoColor=white)](#) | MVP<br />![GitHub last commit](https://img.shields.io/github/last-commit/flyingrobots/TASKS) |
| [Universal Charter](https://universalcharter.org) | **Ethics for tomorrow.** Principles for coexistence between biological, artificial, and hybrid intelligences.<br />![Charter Badge](https://img.shields.io/badge/Universal_Charter-Post_Anthropocentric_Ethics-brightgreen?style=flat-square) | v1.0.0 |
| [MIND-UCAL Software License](https://github.com/UniversalCharter/mind-ucal) | The MIND-UCAL License is an ethical software license that forbids harmful uses like military weapons and surveillance while allowing for personal, commercial, and ethical AI applications. **No weapons. No killer robots. No evil AI.**<br />[![License: MIND-UCAL v1.0](https://img.shields.io/badge/License-MIND--UCAL%20v1.0-orange?logo=fire&logoColor=fff&labelColor=000)](https://github.com/UniversalCharter/mind-ucal/blob/v1.0/LICENSE.md) | v1.0.0 |

---

<p align="center">
  <img src="https://raw.githubusercontent.com/flyingrobots/image-dump/7ddf8ec20119dfcc802dc710c51a46b9ebf551c8/optimized/no_killer_robots_patch_peace_movement.svg" height="200" alt="No Killer Robots Badge" />
</p>
