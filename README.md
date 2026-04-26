<div align="center">
<a href="https://flyingrobots.dev"><img src="https://github.com/user-attachments/assets/6bb97c5d-6de9-451e-a48f-6b11809dee14" /></a>
</div>

<hr />

<h3>
📥 <a href="mailto:james@flyingrobots.dev">Email</a>
🔗 <a href="https://linkedin.com/in/flyingrobots">LinkedIn</a>
📄 <a href="https://www.flyingrobots.dev/james-ross-resume.pdf">Résumé</a>
</h3>
</div>

I've spent nearly two decades building systems. Custom AAA videogame engines and tools, application frontends and backends, MMORPG clients and servers, data platforms, DevOps pipelines, high-throughput event systems, and infrastructure for distributed systems that had to survive reality. After years of debugging race conditions, chasing nondeterminism, and watching mutable state systems lie under pressure, I started asking a more fundamental question.

<div align="center">
<h3><i>What if computation wasn't about state at all?<br />
What if it was about structure evolving through rules?</i></h3>
</div>

In the summer of 2025, I started exploring this question seriously and began writing the **AIΩN Foundations Series** as a way to formalize and document my research. I started by asking *what happens if we model computation using a graph that rewrites itself, recursively?* and then let the rest unfold naturally. Eight papers later, I conclude my research by reaching an entirely unexpected, but nevertheless beautiful discovery: there is no graph, there is no runtime, and there is no system — there is only witnessed causal history, and everything we call a "system" is an observer-relative reading of it.

<div align="center">
  <a href="https://github.com/flyingrobots/aion">
    <img src="https://github.com/user-attachments/assets/287ab2bc-653f-4951-adca-1766d5437082" />
  </a>
  <h3><i>A deterministic architecture for causal computation</i></h3>
</div>

## [AIΩN Foundations Series](https://github.com/flyingrobots/aion)

A sequence of eight papers deriving what happens when you stop storing state and start storing history. From recursive provenance to a protocol for distributed causal computation.

1. If we store history locally, we get **deterministic replay** as a substrate property. ([Papers I–II](https://doi.org/10.5281/zenodo.17908005))
2. If we compress that history, we get **computational holography** — the ability to recover any state from a compact boundary. ([Paper III](https://doi.org/10.5281/zenodo.17963669))
3. If we define how an observer looks at it, we get **observer geometry** and the ability to navigate all possible machines. ([Papers IV–V](https://doi.org/10.5281/zenodo.18038297))
4. If we treat that history as sovereign, we arrive at an **ethics of replay**: provenance is interior life in executable form. ([Paper VI](https://doi.org/10.5281/zenodo.18863648))
5. If we unify the mechanics, we find a single, **scale-invariant WARP optic** that handles execution, merging, and transport identically. ([Paper VII](https://doi.org/10.5281/zenodo.19751149))

**The conclusion:** if history is the only reality, then no runtime is ontologically prior. The "operating system" dissolves. In its place emerges **Continuum** — a protocol to join. (Paper VIII — in progress)

---

<div align="center">
<a href="https://github.com/flyingrobots/continuum"><img alt="Continuum" src="https://github.com/user-attachments/assets/68b121de-5aa9-49d4-8f19-9ccc61e889bf" /></a>
  <h3><i>Continuum: A Protocol for Distributed Causal Computation</i></h3>
</div>

The AIΩN Foundations Series concludes by introducing a protocol-shaped causal medium. Continuum emerges when every participant speaks witnessed admission. These projects make it executable:

**What happens if we build a runtime for the optic?** You get **[Echo](https://github.com/flyingrobots/echo)** — a high-performance simulation engine where every tick is a witnessed admission. Deterministic, replayable, forkable.

**What happens if we host history on Git?** You get **[git-warp](https://github.com/git-stunts/git-warp)** — distributed collaboration without a central database, where worldlines interoperate by sharing the same admission ontology. No servers. Just Git.

**What happens if we compile intent into law?** You get **[Wesley](https://github.com/flyingrobots/wesley)** — a schema compiler that takes authored GraphQL SDL and produces runtime-checkable code for every participant. The application boundary is the sovereign system of record.

**What happens if we debug the derivation instead of the state?** You get **[WARP TTD](https://github.com/flyingrobots/warp-ttd)** — a time-travel debugger that works across any participant in the medium. If it speaks the protocol, it can be debugged here.

---

<div align="center">
  <a href="https://github.com/git-stunts/">
    <img src="https://github.com/user-attachments/assets/3838c7ec-2042-422a-bf6c-99c57cdbba6a" />
  </a>
  <h3><i>Git: Beyond source control</i></h3>
</div>

### I ❤️ Git

Git is the most battle-tested software on Earth. It's also _quietly_ **a primitive WARP graph**.

I run a GitHub organization called **[git-stunts](https://github.com/git-stunts)**, where I publish projects that treat Git plumbing as a foundation for unconventional systems: databases, content graphs, event buses, coordination protocols.

These are **stunts**, _not hacks_: deliberate and grounded in how Git really works. The ability to deconstruct a system to its primitives is one of the most valuable skills in an engineer's toolkit. Often, the most elegant solutions come from looking at the tools we use every day and asking _"What else can this thing do?"_

### Planned Stunts

| Part | Title | Status | Stunt | Lesson |
|------|-------|--------|-------|--------|
| I | Git as CMS | In Review | `commit-tree` as a DB-less API | Protocols reduce ops |
| II | Git as KV Store | Planned | KV using OIDs + notes | CAP tradeoffs in the real world |
| III | Git as Bus | Planned | `post-receive` hooks for pub/sub | Eventing under constraints |
| IV | Git FUSE | Planned | Virtual filesystem via OIDs | Lazy hydration + virtualization |
| V | Agent-Native Git | Planned | RAG + decisions via history | Verifiable memory for LLM work |
| VI | Git as Zero-Trust Gateway | Planned | AST validation in hooks | Shift-left security at the transport |

Follow along for some hot git 🔥 (and occasional self-inflicted pain).

- **[git-cas](https://github.com/git-stunts/git-cas)** — Git, freebased: pure CAS that'll knock your SHAs off. LFS hates this repo!

---

![compsci](https://github.com/user-attachments/assets/18067c4f-fad0-4838-ae12-1e7cc3a44b92)

---

## Related Reading

<a href="https://github.com/flyingrobots/aion-computer-book/blob/book/computer.pdf">
  <img width="500" alt="Cosmic Doorway Illumination" src="https://github.com/user-attachments/assets/31d310c0-22d9-4068-822d-2d0f306787ca" align="left" />
</a>

**[CΩMPUTER: The Geometry of All Possible Machines](https://github.com/flyingrobots/aion-computer-book)** is the synthesis work. It pushes the AIΩN machinery to its philosophical and architectural limit, arguing that computation is not a human invention but the base reality — and providing the map for navigating the Multi-Rule Multi-World space where everything is witnessed all the way down.

<p align="center"><a href="https://github.com/flyingrobots/aion-computer-book/blob/book/computer.pdf">READ CΩMPUTER FOR FREE ONLINE</a></p>

<br clear="left"/>

- **[Observer Geometry I: Beyond Distance](https://doi.org/10.5281/zenodo.18868896)** — Separates projection, basis & accumulation to characterize replayability & conflict visibility under resource limits.  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18868896.svg)](https://doi.org/10.5281/zenodo.18868896)

- **[The Open Charter](https://github.com/flyingrobots/open-charter)** — Constitutional governance for coordinating rights, safety, and accountability across biological, digital, and hybrid intelligence.  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18517806.svg)](https://doi.org/10.5281/zenodo.18517806)

- **[PRAXIS: A Field Guide to the Inevitable](https://github.com/flyingrobots/PRAXIS)** — An experiential model of how systems can make "choice" feel like friction.  
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18206427.svg)](https://doi.org/10.5281/zenodo.18206427)
