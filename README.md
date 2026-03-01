<div align="center">
<a href="https://flyingrobots.dev">
<img src="https://github.com/user-attachments/assets/fc06206f-437f-49e2-bbd0-a72330b95579" />
</a>

<hr />

<h3>
📥 <a href="mailto:james@flyingrobots.dev">Email</a>
🔗 <a href="https://linkedin.com/in/flyingrobots">LinkedIn</a>
📄 <a href="https://www.flyingrobots.dev/james-ross-resume.pdf">Résumé</a>
</h3>

</div>

<hr />

# Senior Distributed Systems Engineer

I’ve spent nearly two decades building production distributed systems, MMO backends, data platforms, DevOps pipelines, high-throughput event systems, custom engines, and infrastructure that had to survive reality.

After years of debugging race conditions, chasing nondeterminism, and watching mutable state systems lie under pressure, I started asking a more fundamental question:

What if computation wasn’t about state at all?

What if it was about *structure evolving through rules*?

---

## WARP Graphs: _Worldline Algebra for Recursive Provenance_

Modern systems are not really "state machines." They are evolving graphs of relationships.

If we treat them that way, literally, and build around rewrite rules instead of mutable state, we gain something powerful:

- **Always-on time travel debugging**
- **Bit-perfect determinism across platforms**
- **Complete system-wide provenance**
- **Lockless concurrency where race conditions are impossible by construction**

This is the foundation of the systems I build. I formalize this model as **WARP graphs**, a deterministic rewrite substrate for replayable, inspectable computation.

This GitHub is where I publish the systems that emerge from that idea.

---

<div align="center">
  <img src="https://github.com/user-attachments/assets/3838c7ec-2042-422a-bf6c-99c57cdbba6a" />
</div>

<hr />

### I ❤️ Git

Git is the most battle-tested software on Earth.  

It’s also _quietly_ **a primitive WARP graph**.

I run a GitHub organization called **[git-stunts](https://github.com/git-stunts)**, where I publish projects that treat Git plumbing as a foundation for unconventional systems—databases, content graphs, event buses, coordination protocols. 

These are **stunts**, _not hacks_: deliberate and grounded in how Git really works. These projects are about understanding tools deeply enough that surprising architectures emerge naturally. 

The ability to deconstruct a system to its primitives is one of the most valuable skills in an engineer's toolkit. The repos in this org are about learning more than just how Git works under the hood. We aren't playing Macgyver with Git just for the fun of it; we do it to understand how to think outside the box when conventional tools fail.

Often, the most elegant solutions come from looking at the tools we use every day and asking _"What else can this thing do?"_

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

- **[git-cas](https://github.com/git-stunts/git-cas)** — Git, freebased: pure CAS that’ll knock your SHAs off. LFS hates this repo!


<hr />

![compsci](https://github.com/user-attachments/assets/18067c4f-fad0-4838-ae12-1e7cc3a44b92)

</div>

---

## Is the universe a deterministic graph rewrite engine… or does it just *look* like one because we’re imperfect observers?

I build systems around **WARP graphs**: deterministic replay, time-travel debugging, provenance sovereignty, and **computational holography**. 

If you’ve ever wanted to **rewind a system**, inspect it like a crime scene, fork it like a multiverse, and still keep the receipts—hi.

- **Deterministic replay**: rewind, inspect, fork any execution
- **Machine geometry**: make computation’s hidden structure visible
- **Refactor gravity**: measure why some code yields, and some code resists

**Key reads:**  
- WARP graphs paper: https://doi.org/10.5281/zenodo.17908005  
- Computational holography: https://doi.org/10.5281/zenodo.17963669  

---

## What I’m building (featured)

| Project | What it is | Why it matters |
|---|---|---|
| **[AIΩN](https://github.com/flyingrobots/aion)** | Formal framework for deterministic, history-native computation | “Transforms, not states.” Replayability as a first-class invariant. |
| **[Echo](https://github.com/flyingrobots/echo)** | Real-time WARP rewrite engine (Rust) | Deterministic simulation you can rewind and fork without lying to yourself. |
| **[Git-WARP](https://github.com/git-stunts/git-warp)** | WARP graph engine on Git commits | CRDT-friendly history with deterministic replay and brutal simplicity. |
| **[xyph](https://github.com/flyingrobots/xyph)** | Reificatory Engine | Xyph it done. |
| **[git-mind](https://github.com/flyingrobots/git-mind)** | Semantic knowledge graph on Git | Version your thoughts. Branch ideas. Merge understanding. |

---

<div align="center">
<img src="https://github.com/user-attachments/assets/287ab2bc-653f-4951-adca-1766d5437082" />
</div>

<hr />

AIΩN treats computation as a **verifiable rewrite process**: transformations are the primary artifact, not ephemeral state.

Built on WARP graphs and **double-pushout (DPO) rewriting**, it turns execution into a rewindable, forkable history with provenance you can actually trust.

It’s “graphs all the way down” with a practical goal: **systems that can explain themselves**. What happened, why, and what would’ve happened if we’d chosen differently.

### AIΩN Foundations Series

| ID | Title | Status | Contribution |
| :---: | --- | :---: | --- |
| **I** | *Worldline Algebra for Recursive Provenance* | ✅ Published | Defines **WARP graphs** as recursive provenance structures. |
| **II** | *Canonical State Evolution and Deterministic Worldlines* | ✅ Published | Deterministic semantics via **DPO rewriting**. |
| **III** | *Computational Holography & Provenance Payloads* | ✅ Published | Recover full derivations from compact boundary data. |
| **IV** | *Rulial Distance & Observer Geometry* | ✅ Published | Abstraction cost + time perception (Chronos–Kairos–Aion). |
| **V** | *Emergent Dynamics from Deterministic Rewrite Systems* | ✅ Published | Emergence via coarse-graining (quantum/thermo analogs). |
| **VI** | *Ethics & Sovereignty* | 🧪 Draft | Accountability and agency in replayable worldlines. |
| **VII** | *Architecture & Operating System* | 🧪 Draft | **Continuum**: a causal OS built on these invariants. |

### AIΩN Applied

- **[CΩMPUTER](https://github.com/flyingrobots/aion-computer-book)** — book-in-progress: computation as base reality  
- **[Continuum OS](https://github.com/flyingrobots/continuum)** — causal runtime + holographic artifacts *(very early)*  

---

