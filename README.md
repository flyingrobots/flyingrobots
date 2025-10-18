# James Ross • [Flying Robots](https://flyingrobots.dev)

Seattle, WA • [E-Mail](mailto:james@flyingrobots.dev) • [LinkedIn](https://linkedin.com/in/flyingrobots) • [Calendly](https://calendly.com/flyingrobots-dev/30min)

## Current Art

I build developer tools that eliminate entire categories of complexity.

The most powerful abstractions feel inevitable once you see them. That's what these projects do. They take genuinely complex problems (deployment provenance, schema drift, autonomous planning) and collapse them into primitives so simple they become invisible.

The most elegant solutions don't always involve inventing new tools. They're found in clever new ways of using the tools we already have. My benchmark isn't just the absence of the original problem, it's when things feel obvious, and entire categories of complexity have been eliminated. That's how you unlock a team's potential: make tools and workflows deliberately boring and out of the way.

---

## On Seeing Patterns

Fifteen years ago I was on lunch break, sitting outside in Seattle after walking through Pike Place Market. I'd just seen Romanesco broccoli for the first time. That fractal vegetable where each floret is a miniature copy of the whole.

I realized: nature had been doing recursive graphs for millions of years. We were just late to the party.

That insight led to [**Recursive Metagraphs**](https://github.com/meta-graph/core) a data structure where nodes are graphs, edges are graphs, infinitely recursive. **Graphs all the way down.** The [mathematical properties](https://github.com/meta-graph/core/blob/main/docs/rmg-math.md) turn out to be universal: this structure can model computation itself.

Git is a specialized recursive metagraph. So is the internet. So is thought.

Once you see it, you can't unsee it.

---

## [Shiplog](https://github.com/flyingrobots/shiplog) – The Deployment Primitive

Remember that 2 AM incident where no one knew which version was deployed or who changed the config?  
Remember digging through Slack threads and CloudWatch logs trying to reconstruct history?  
That's because your deployment logs live in dashboards you don't control, in formats you can't query, already rotated out.

**Shiplog fixes that.**

It turns your Git repo into a cryptographically signed, append-only ledger of every step of every deployment. Run anything with:

```bash
git shiplog run <your-command>
```

Shiplog captures stdout, stderr, exit code, timestamp, author, and reason—everything you'd lose in the void—and logs it in a signed, immutable ref right inside Git. Deployment logs live with your codebase, but apart from it. Provenance without clutter.

A built-in allow list enforces policy at the source: only trusted contributors can deploy, or multiple can sign off before a quorum. Every run verified. Every log auditable. Every action permanent.

**Zero SaaS. Zero external infra. Zero guesswork.**  
**Policy as infrastructure, living with your code.**

**Status:** [v0.2.1](https://github.com/flyingrobots/shiplog/releases/tag/v0.2.1) • Production Ready

---

## [Wesley](https://github.com/flyingrobots/wesley) – The Data-Layer Compiler

Stop describing your data model six times in six different files.  
Everyone else generates GraphQL from databases. Wesley flips the stack and generates databases from GraphQL.

From one schema, Wesley compiles your entire backend:

- Postgres DDL & migrations
- TypeScript types & Zod validators
- Supabase RLS, Realtime & Storage rules
- tRPC endpoints & Prisma/Drizzle integration
- pgTAP tests
- A SHA-locked \"Shipme\" certification file for zero-downtime deployments

**Your schema is the source of truth. Everything else is a compilation target.**

Banish drift. Never think about migrations again. Describe your shapes once and let Wesley handle the rest.

Go on, deploy on a Friday.

**Status:** MVP • Active Development

---

## [T.A.S.K.S. + S.L.A.P.S.](https://github.com/flyingrobots/TASKS) – Autonomous Planning & Execution at Graph Scale

Your team spends three months coordinating a microservices migration.

**T.A.S.K.S.** (_**T**asks **A**re **S**equenced **K**ey **S**teps_) plans it in hours—analyzing your codebase for dependencies, resource constraints, and reuse opportunities to build a mathematically optimized execution graph.

**S.L.A.P.S.** (_**S**ounds **L**ike **A** **P**lan **S**ystem_) executes it. A resilient swarm of agents traversing that graph via a rolling frontier, adapting in real time when things go sideways.

Something unexpected happens? No problem. S.L.A.P.S. rolls back to the last good state, replans, and resumes. Configurable bulkheads and circuit breakers give you precise control over failure domains.

Together they collapse months of human coordination into hours of autonomous graph traversal.

**From idea to outcome. Orders of magnitude faster.**

The AI framework they warned you about. _Resistance is futile. Your biological distinctiveness will be assimilated into the swarm._

**Status:** MVP • Active Development

---

## Deep Work: Where the Math Lives

### [Recursive Metagraphs](https://github.com/meta-graph/core) – Universal Computation Model

**RMG** is a C23 library implementing recursive metagraphs where nodes are graphs, edges are graphs, infinitely recursive. The [mathematical formalization](https://github.com/meta-graph/core/blob/main/docs/rmg-math.md) proves these structures are universal. They can model any computational process.

Git is an RMG. The web is an RMG. Your thought process is an RMG.

This isn't just a neat data structure. It's a unified model for versioning, provenance, state, and change across any domain.

**Status:** ~1170 LOC • Mathematical Foundation Complete • Active Research

### [Git Mind](https://github.com/neuroglyph/git-mind) – Git as a Graph Database

What if Git wasn't just source control, but a database-less graph database for semantic knowledge?

**Git Mind** turns any git repo into a semantic knowledge graph for distributed cognition and human–AI co-thought. Version-controlled knowledge with Git's conflict resolution and merging primitives.

Your thoughts, versioned. Your collaboration with AI, versioned. All without a database. Just Git.

**Status:** Early Research

### [Hubless](https://github.com/flyingrobots/hubless) – Git-Native Project Flow

Issues, Kanban, execution—all in your repo. No external dependencies. Freedom from vendor lock-in.

It's your project. Take it with you.

**Status:** Early Development

---

## Ethics & Principles

I believe technology should serve humanity, not harm it.

### [Universal Charter](https://universalcharter.org)

Principles for coexistence between biological, artificial, and hybrid intelligences. Post-anthropocentric ethics for a world where we're not the only minds in the room.

**Status:** v1.0.0

### [MIND-UCAL Software License](https://github.com/UniversalCharter/mind-ucal)

An ethical software license that forbids harmful uses—military weapons, surveillance, killer robots—while allowing personal, commercial, and ethical AI applications.

**No weapons. No killer robots. No evil AI.**

**Status:** v1.0.0

---

## Teaching

### [GitScrolls](https://github.com/gitscrolls/gitscrolls) – The Mythic Developer's Journey

A 16-part epic teaching Git through one developer's tragic force-push. Because the best way to learn version control is through narrative tragedy and redemption.

**Status:** Story Edit in Progress

---

<p align=\"center\">
  <em>Building tools that make complexity invisible, one graph at a time.</em>
</p>
