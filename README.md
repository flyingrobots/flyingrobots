# James Ross • [Flying Robots](https://flyingrobots.dev)

Seattle, WA • [E-Mail](mailto:james@flyingrobots.dev) • [LinkedIn](https://linkedin.com/in/flyingrobots) • [Calendly](https://calendly.com/flyingrobots-dev/30min)

## Current Art

I build developer tools that eliminate entire categories of complexity.

The most powerful abstractions feel inevitable once you see them. That's what these projects do. They take genuinely complex problems (deployment provenance, schema drift, autonomous planning) and collapse them into primitives so simple they become invisible.

The most elegant solutions don't always involve inventing new tools. They're found in clever new ways of using the tools we already have. My benchmark isn't just the absence of the original problem, it's when things feel obvious, and entire categories of complexity have been eliminated. That's how you unlock a team's potential: make tools and workflows deliberately boring and out of the way.

---

## On Seeing Patterns

<img alt="romanesco broccoli" src="https://github.com/user-attachments/assets/e6091cf1-cc2f-4990-9b80-88c186fe10d7" align="left" width="400" />


_Fifteen years ago I was on lunch break, sitting outside in Seattle after walking through Pike Place Market..._

I'd just seen Romanesco broccoli for the first time. That fractal vegetable where each floret is a miniature copy of the whole.

I realized: nature had been doing recursive graphs for millions of years. We were just late to the party.

That insight led to [**Recursive Metagraphs**](https://github.com/meta-graph/core) a data structure where nodes are graphs, edges are graphs, infinitely recursive. **Graphs all the way down.** The [mathematical properties](https://github.com/meta-graph/core/blob/main/docs/rmg-math.md) turn out to be universal: this structure can model computation itself.

> _**Git is a specialized recursive metagraph. So is the internet. So is thought.**_

Once you see it, you can't unsee it.

---

## [GATOS: *Git As The Operating Surface™*](https://github.com/flyingrobots/gatos)

<img alt="GATOS Git As The Operating Sufrace" src="https://github.com/user-attachments/assets/f7c366b0-967b-45df-8848-6e069fc04cdc" width=350 align="left" />


> You use Git for source control.  
> I use Git for _reality control_.  
> **We are not the same.**  

**What is GATOS?** It’s the Operating Surface™ — the place where state, policy, and computation converge.  

For decades, we’ve been sitting on untapped potential, hiding in plain sight. Git — the most resilient distributed system ever built — has been quietly powering our repositories, waiting for someone to wake it up. _Until now._  

GATOS unlocks Git's true potential: transcending source control, breathing life into the graph itself, weaving commits, refs, and even notes into a rich tapestry of fully programmable, distributed, general-purpose computation.

GATOS takes the most battle-tested state system on Earth and reveals its true form: an **offline-first**, **federated**, **programmable**, **self-governing** compute platform. At its core beats a deterministic, immutable engine of **auditable cryptographic provenance** — all while saying _"Look Ma! No blockchain!"_

By the power of GATOS, Git’s time-travel powers extend beyond code into the realms of computation, collaboration, and consciousness.  
GATOS enables mind-melds, distributed agency, and systems that don't ask “what if?” — they find out for themselves.  

**GATOS** – Because Git can do far more than version control.  
_You just have to know how to Git it._

---

## [ECHO](https://github.com/flyingrobots/echo) – The Impossible Game Engine

<img height="350" alt="Echo" src="https://github.com/user-attachments/assets/f7b02dad-b5c3-46f5-ab6a-9aa87b477653" align="right" />

> _"Things are only impossible until they're not." — Jean-Luc Picard_

Echo is an ambitious, mind-bending, radically different computational model for interactive simulations, built on the Recursive Meta-Graph (RMG). In this model, everything is a graph—nodes, edges, and even rewrite rules are all, recursively, graphs. It’s Graphs. All. The. Way. Down.

Where traditional engines like Unity and Unreal are built on mutable, object-oriented state machines, Echo is fundamentally built different. It replaces mutable objects with a declarative system where the engine rewrites the entire graph using deterministic, typed transformation rules.

The result is a game engine with properties previously considered impossible: perfect confluent determinism.

This powerful, category-theory-backed math eliminates network desyncs forever and makes your world rewindable, forkable, and perfectly mergable. It delivers time-travel debugging, flawless replays, and the capability to build a true multiverse.

Echo is the future of simulation. Buckle up, because things are gonna get weird.

## [`libgitledger`](https://github.com/flyingrobots/libgitledger) – The [Ledger-Kernel](https://github.com/flyingrobots/ledger-kernel) Reference Implementation

[Ledger-Kernel](https://github.com/flyingrobots/ledger-kernel) is a formal specification and reference implementation ([libgitledger](https://github.com/flyingrobots/libgitledger)) for building verifiable, append-only ledgers directly on top of Git’s object model.

<img src="https://github.com/user-attachments/assets/0f1d8323-6e5b-499b-939b-12e5953e0187" alt="libgitledger" width="250" align="right" />

Unlike blockchains or SaaS audit logs, Ledger-Kernel **is just Git**. It adds deterministic replay, cryptographic attestation, and programmable policy enforcement without introducing new infrastructure.

It uses existing .git storage, requiring no daemons or databases. It enforces fast-forward-only semantics to ensure history is immutable and guarantees deterministic replay, where identical input always yields identical state. Every entry is attested for non-repudiable authorship, and the system supports WASM-based policies for validation.

Sort of like blockchain's weird little cousin. 

## [Shiplog](https://github.com/flyingrobots/shiplog) – The Deployment Primitive

<img src="https://github.com/user-attachments/assets/7934bb47-14ad-4f12-8bea-e3135eceab7d" width="400" alt="Shiplog" align="right" />

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

**Status:** [v0.2.1](https://github.com/flyingrobots/shiplog/releases/tag/v0.2.1) • Active Development (Alpha WIP)

---

## [Wesley](https://github.com/flyingrobots/wesley) – The Data-Layer Compiler

<img width="400" alt="Wesley" src="https://github.com/user-attachments/assets/8eec4c88-531f-4342-933a-1914d257c05c" align="right" />


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

<img src="https://github.com/user-attachments/assets/74fb2070-4bc0-469d-aff5-4cfc23d4d8c4" alt="TASKS and SLAPS" width="400" align="right" />

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

<img width="200" alt="Recursive metagraph" src="https://github.com/user-attachments/assets/69368fba-8fc2-407b-830b-c20dce7195d7" align="right" />

**RMG** is a C23 library implementing recursive metagraphs where nodes are graphs, edges are graphs, infinitely recursive. The [mathematical formalization](https://github.com/meta-graph/core/blob/main/docs/rmg-math.md) proves these structures are universal. They can model any computational process.

Git is an RMG. The web is an RMG. Your thought process is an RMG.

This isn't just a neat data structure. It's a unified model for versioning, provenance, state, and change across any domain.

**Status:** Mathematical Foundation Complete • Active Research

### [Git Mind](https://github.com/neuroglyph/git-mind) – Git as a Graph Database

<img alt="git-mind" src="https://github.com/user-attachments/assets/438d1c95-7b0c-4000-bc55-84eedf9264f2" align="right" width="200" />

What if Git wasn't just source control, but a database-less graph database for semantic knowledge?

**Git Mind** turns any git repo into a semantic knowledge graph for distributed cognition and human–AI co-thought. Version-controlled knowledge with Git's conflict resolution and merging primitives.

Your thoughts, versioned. Your collaboration with AI, versioned. All without a database. Just Git.

**Status:** MVP • Active Development

### Ethics & Principles

I believe technology should serve humanity, not harm it.

#### [Universal Charter](https://universalcharter.org)

<img alt="Universal Charter" src="https://github.com/user-attachments/assets/342c2a83-c05e-4272-9fac-80a353be66c8" width="200" align="right" />

Principles for coexistence between biological, artificial, and hybrid intelligences. Post-anthropocentric ethics for a world where we're not the only minds in the room.

**Status:** v1.0.0

#### [MIND-UCAL Software License](https://github.com/UniversalCharter/mind-ucal)

<img src="https://raw.githubusercontent.com/flyingrobots/image-dump/7ddf8ec20119dfcc802dc710c51a46b9ebf551c8/optimized/no_killer_robots_patch_peace_movement.svg" alt="MIND-UCAL" width="200" align="right" />

An ethical software license that forbids harmful uses—military weapons, surveillance, killer robots—while allowing personal, commercial, and ethical AI applications.

**No weapons. No killer robots. No evil AI.**

**Status:** v1.0

---

### Teaching

#### [GitScrolls](https://github.com/gitscrolls/gitscrolls) – The Mythic Developer's Journey

<img width="300![shiplog-final](https://github.com/user-attachments/assets/e80e57c8-24d7-4a24-8bf7-f69bd152ad41)
" alt="tuxicles" src="https://github.com/user-attachments/assets/58d0f341-aa91-4b7e-b8ec-a9de1e4f0e4d" align="left" />


A 16-part epic teaching Git through one developer's tragic force-push. Because the best way to learn version control is through narrative tragedy and redemption.

What happens when you git push --force your ego directly to production?

For Tuxicles, a brilliant but arrogant programmer, the answer is a disaster of epic proportions: 2.3 million broken user sessions, a betrayed community, and a one-way ticket to the Nine Circles of Developer Hell.

Now, he must navigate a hilarious and terrifying underworld where the demons are merge conflicts and the damned are trapped in infinite loops of their own bad habits. Forget everything you know about epic fantasy. To escape, Tuxicles must face the one bug he never thought to fix: himself.

**Status:** Story Edit in Progress

---

<p align=\"center\">
  <em>Building tools that make complexity invisible, one graph at a time.</em>
</p>
