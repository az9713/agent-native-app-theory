# A Formal Theory of State in Agent-Native Applications

**Read it live:** [az9713.github.io/agent-native-app-theory/agent_native_state_theory_v2.html](https://az9713.github.io/agent-native-app-theory/agent_native_state_theory_v2.html)

A formal model of state in an application where humans and AI agents change the same underlying state. It extends the simple equation S<sub>t+1</sub> = F(S<sub>t</sub>, a<sub>t</sub>) to a partially observable, multi-actor transition system with typed state, provenance, permissions, and constrained transitions. The worked setting is an AI R&D operating system.

## What the document covers

- **§1–§7 State.** Domain graph, claims with confidence, workflow runs, agent runtime state, policy, and external state. It separates the full world state from the state the application stores and can replay.
- **§8–§10 Dynamics.** Actors (one actor and one action per logged step), a stochastic transition kernel, and partial observability.
- **§11–§16 Mechanisms.** Event sourcing, invariants and liveness, goals and a two-stage model router, human approval with version-bound proposals and a reviewer-capacity model, concurrency, and provenance.
- **§17–§18 The formal object** and a compact form for an AI R&D OS.
- **§19** Four properties that make an application agent-native, each with a test.
- **§20** Four consequences with short proofs: replay determinism, safety by induction, approval soundness, and rate independence.
- **§21** A worked example that traces one publish action through every component.

## Status

This is revision 2. It keeps the 18 sections of revision 1 in the same order and adds a notation table, the new subsections, and §19–§21. The last section of the document lists each change.

## Files

- `agent_native_state_theory_v2.html` — the document. It is a single self-contained page; the math is MathML, so it needs no scripts. It supports light and dark mode.
- `agent_native_state_theory_reviewed.html` — the review of revision 1: its full text with 98 inline review notes (strengths, weaknesses, suggestions) and a recommendation for each weakness. The change table at the end of revision 2 links to these notes. [Read the review live](https://az9713.github.io/agent-native-app-theory/agent_native_state_theory_reviewed.html).
