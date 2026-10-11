# trust-graph

Personal hermeneutic trust model for AI assistants. Evidence-based. 5 dimensions. Exponential decay.

## Status

Early scaffolding. The working implementation lives in [Agent-Friday](https://github.com/FutureSpeakAI/Agent-Friday) under `src/agent_friday/trust/` (a hash-chained evidence log and per-person trust). This repo is reserved for the standalone package when it is extracted.

## Concept

A trust graph tracks per-entity (people, agents, sources) trust along five dimensions:

- **Competence** — do they get things right?
- **Honesty** — do they say what they believe?
- **Care** — do they act with the user's interest in mind?
- **Reliability** — do they show up consistently?
- **Predictability** — can you model what they'll do next?

Evidence accumulates over time. Each piece of evidence decays exponentially, so recent signal dominates.
