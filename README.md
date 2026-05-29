> I build deterministic developer infrastructure: schema compilers, Git-native provenance systems, replayable runtimes, terminal UI tooling, and agent-safe repo context systems. Most of the work is Rust/TypeScript. Start with Bijou for a runnable product, Wesley for compiler work, Echo/`git-warp` for causal runtime research.

# My Work

```mermaid
 mindmap
    root((Ecosystem))
      Foundations
        ))Continuum((
        ))Wesley((
      Runtimes & Apps
        ))Echo((
          jedit
        ))git-warp((
          Graft
          Think
          Xyph
      Tooling
        ))WARP-TTD((
      Libraries
        Bijou
          Alfred
        Nine Lives
        git-cas
      Standalone
        Geordi
        Shiplog
        METHOD
```

For decades, most systems have quietly inherited the Unix mental model: processes mutating files on a shared, hierarchical filesystem. State lives in place. Logs are best-effort. History is whatever you remembered to write to disk.

That model scales surprisingly far, but it shows its limits under concurrency, distribution, and automation. Process-local mutation and ad hoc logging make it hard to answer basic questions: What actually happened? Who did it? In what order? Can we replay it?

The work here is an experiment in a post‑Unix posture:

- **Processes** become strands in a shared causal history, not anonymous workers scribbling over state.  
- **Files** become materializations over history, not the source of truth.  
- **The data model** is an append-only ledger of events with verifiable provenance, not mutable bytes at paths.  
- **Time** is encoded in the causal structure of that ledger—links, worldlines, ticks, receipts—not in loose timestamps.  
- **Runtimes** own admission, ordering, and replay; applications submit intents and consume evidence.  

You don’t fix a bug by guessing from logs—you derive it from the causal record. You don’t pray your editor and planner are in sync—you ask what the underlying history allows them to see.

The repositories below are materializations of this stack.

***

```mermaid
graph TD
      subgraph Foundations
          Continuum("<b>Continuum</b><br>Core Protocol"):::p
          Wesley("<b>Wesley</b><br>Contract Compiler"):::t
      end

      subgraph "Libraries"
          subgraph "Rust Libs"
              NineLives("<b>Nine Lives</b><br>Resilience"):::l
          end
          subgraph "TS Libs"
              Bijou("<b>Bijou</b><br>TUI Toolkit"):::l
              Alfred("<b>Alfred</b><br>Resilience"):::l
              git_cas("<b>git-cas</b><br>Storage"):::l
          end
      end

      subgraph "Continuum Runtimes & Applications"
          subgraph "Echo Runtime Ecosystem"
              Echo("<b>Echo</b><br>Runtime"):::r
              jedit("<b>jedit</b><br>Editor App"):::a
          end

          subgraph "git-warp Runtime Ecosystem"
              git_warp("<b>git-warp</b><br>Runtime"):::r
              Graft("<b>Graft</b><br>Agent Governor"):::a
              Think("<b>Think</b><br>Capture App"):::a
              Xyph("<b>Xyph</b><br>Planning Compiler"):::a
          end
      end

      subgraph "Tooling & Standalone"
          WARP_TTD("<b>WARP-TTD</b><br>Debugger"):::t
          Geordi
          Shiplog
          METHOD("<b>METHOD</b><br>Process")
      end

      %% Foundational Dependencies
      Continuum --> Echo
      Continuum --> git_warp
      Continuum --> WARP_TTD

      Wesley --> Echo
      Wesley --> git_warp
      Wesley --> jedit
      Wesley --> Geordi

      %% Library Dependencies
      NineLives --> Echo
      Alfred --> Bijou
      Bijou --> jedit
      Bijou --> Graft
      Bijou --> Think

      %% Runtime App Dependencies
      Echo --> jedit
      git_warp --> Graft
      git_warp --> Think
      git_warp --> Xyph

      %% Looser Dependencies / Interactions
      git_cas -. "Provides storage for" .-> git_warp

      classDef p fill:#eceff1,stroke:#607d8b
      classDef l fill:#f9f9f9,stroke:#333,stroke-width:1px
      classDef r fill:#e8f5e9,stroke:#4CAF50,stroke-width:2px
      classDef a fill:#e3f2fd,stroke:#2196F3,stroke-width:1px
      classDef t fill:#fff3e0,stroke:#FB8C00,stroke-width:1px
```

## Foundations

**[Continuum](https://github.com/flyingrobots/continuum)** — Shared protocol and contract language for witnessed causal history. The coordination layer that keeps sibling runtimes compatible without forcing them to share a database.

**[Wesley](https://github.com/flyingrobots/wesley)** — GraphQL SDL compiler. One schema drives TypeScript, Rust, SQL, manifests, and runtime plans. Proven semantics, zero hand-maintained drift.

**[METHOD](https://github.com/flyingrobots/method)** — Lightweight engineering process framework backed by the filesystem. Backlog, cycle loop, retros, drift detection — no sprint theater.

---

## Storage & history

**[git-warp](https://github.com/git-stunts/git-warp)** — Git-native causal history engine. Patches over worldlines, speculative strands, canonical braids. Git's distribution model plus structured, replayable provenance.

**[git-cas](https://github.com/git-stunts/git-cas)** — Industrial-grade content-addressable storage inside Git's object database. Chunked, deduplicated, AES-256-GCM encrypted. No external artifact host required.

**[Shiplog](https://github.com/flyingrobots/shiplog)** — Git-native deployment ledger. Signed, append-only deployment runs recorded inside Git refs. Every deploy step permanent, queryable, and reviewable.

**[Xyph](https://github.com/flyingrobots/xyph)** — Planning compiler built on git-warp. Replaces scattered tickets with a single deterministic WARP graph. Cryptographic settlement, Ed25519 guild seals, offline-first.

**[Think](https://github.com/flyingrobots/think)** — Instant thought-capture engine. Raw ideas into a private Git-backed cognitive worldline. Capture speed over organization; browse and reflect later.

---

## Runtimes & reliability

**[Echo](https://github.com/flyingrobots/echo)** — Deterministic runtime where state is a materialized view over immutable causal history. 300k+ rewrites/second at 60fps. Replay, time-travel, and provable transitions built in.

**[Alfred](https://github.com/git-stunts/alfred)** — Policy engine for async resilience in TypeScript. Composable, testable retry/backoff/circuit behavior with a live control plane.

**[Nine Lives](https://github.com/flyingrobots/ninelives)** — Tower-native resilience framework for Rust. Algebraic composition of retry, timeout, circuit breaker, bulkhead, and fallback — plus runtime policy control.

---

## Interfaces & products

**[Bijou](https://github.com/flyingrobots/bijou)** — TypeScript toolkit for terminal software. Real character grid, layout engine, i18n, deterministic render output. Terminal as a serious application platform.

**[Geordi](https://github.com/flyingrobots/geordi)** — Deterministic GPU scene IR for interactive vector UI. Canonical intermediate representation between authoring tools and WebGL/WebGPU/Metal/Vulkan backends.

**[Graft](https://github.com/flyingrobots/graft)** — Context governor for coding agents. Policy-enforced reads, parser-backed structural views, causal provenance over repo activity. Agents see the smallest safe view.

**[jedit](https://github.com/flyingrobots/jedit)** — Terminal-first text and Markdown editor over Echo and Graft. Vim-shaped. Edits are contract-shaped intents submitted to a causal runtime.

---

## Debugging & observation

**[WARP TTD](https://github.com/flyingrobots/warp-ttd)** — Time-travel debugger for deterministic causal runtimes. Inspect worldlines, receipts, rejected counterfactuals, and provenance. Pause, step, seek, fork.
