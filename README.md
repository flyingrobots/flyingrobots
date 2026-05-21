<div align="center">
  <a href="https://flyingrobots.dev">
    <img alt="Computer Science" src="https://github.com/user-attachments/assets/af9ec127-78e9-4452-829b-8f1db672e6b5" />
  </a>
</div>

### Ladder of Computation

| Stratum | Level | Philosophy | Methodology | Query |
|----------|--------|-------------|----------------|----------|
| **I** | Ephemeral | State-Centric | Treat mutable state as primary truth. Synchronize aggressively. Debug forward from symptoms. | _What is the state?_ |
| **II** | Journaled | Transactional | Preserve ordered mutation history through logs and snapshots. Recover execution through deterministic replay. | _What happened?_ |
| **III** | Federated | Distributed Consensus | Coordinate replicas through quorum and replicated state machines. Trade latency and complexity for globally ordered mutation. | _What do replicas agree happened?_ |
| **IV** | Projected | Event-Sourced / CRDT | Preserve history as the canonical structure. Materialize state as projections over convergent event streams. | _What histories converge?_ |
| **V** | Invariant | Causal Determinism | Treat causality itself as the immutable substrate. Materialize observer-relative state over deterministic history. Schedule execution through invariant-preserving footprints so unsafe concurrency cannot emerge. Enable exact replay and computable counterfactuals. | _What causality makes unsafe execution impossible?_ |
| **VI** | Reflexive | Meta-Causal / Self-Describing | Invariants, observers, schedulers, projections, and counterfactual models are first-class causal artifacts. The rules of computation evolve through proof-carrying amendments. Materialize admissible worlds over versioned semantics. Compute across possible machines, not merely possible histories. | _How many rules safely evolve?_ |
| **VII** | Autogenic | Proof-Carrying Synthesis | Generate runtimes, protocols, schemas, projections, and schedulers from invariant specifications. Code is a derived artifact, not the source of truth. | _How can machines be synthesized from rules?_ |
| **VIII** |  Ecological | Inter-Causal Composition | Compose multiple reflexive systems without requiring one global ontology. Boundaries become typed, proof-carrying translations between causal worlds. | _How do different rule-worlds compose?_ |
| **IX** | Teleological | Intent-Causal Governance | Goals, policies, values, permissions, and resource priorities are versioned causal objects. Compute only within accountable purpose constraints. | _Why should computation happen at all?_ | 
| **X** | Axiomatic | Foundation-Relative Computation | Logic, time, causality, identity, and observation are selectable foundations. Compute across possible computational universes and prove which foundations admit which invariants. Tabs, not spaces. | _What foundations make computation possible?_ |
