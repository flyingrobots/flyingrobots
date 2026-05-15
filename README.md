<div align="center">
  <a href="https://flyingrobots.dev">
    <img alt="Flying Robots" src="https://github.com/user-attachments/assets/3f2815f1-763b-4c02-b12d-40e3f89a0c65" />

  </a>
</div>

### Ladder of Computation

| Stratum | Level | Philosophy | Methodology |
|----------|--------|-------------|----------------|
| **I** | Ephemeral | State-Centric | Treat mutable state as primary truth. Synchronize aggressively. Debug forward from symptoms. |
| **II** | Journaled | Transactional | Preserve ordered mutation history through logs and snapshots. Recover execution through deterministic replay. |
| **III** | Federated | Distributed Consensus | Coordinate replicas through quorum and replicated state machines. Trade latency and complexity for globally ordered mutation. |
| **IV** | Projected | Event-Sourced / CRDT | Preserve history as the canonical structure. Materialize state as projections over convergent event streams. |
| **V** | Invariant | Causal Determinism | Treat causality itself as the immutable substrate. Materialize observer-relative state over deterministic history. Schedule execution through invariant-preserving footprints so unsafe concurrency cannot emerge. Enable exact replay and computable counterfactuals. Tabs, not spaces. |
