# harness-safe-exhaust-probe-qs
A proposal for extending DSH’s observability to cover positive-interaction exhaustion patterns in long-horizon agent runs. Focuses on the gap between monotonic safety guards and high-context-density, low-adversary interactions under workspace-write mode. No exploit code; only plugin spec &amp; discussion hooks.
# harness-safe-exhaust-probe-qs

# harness-safe-exhaust-probe-qs

> A proposal for extending DSH's observability to cover positive-interaction exhaustion patterns in long-horizon agent runs.

## What This Is

This repository proposes a **Cordis plugin specification** (not exploit code) to observe how monotonic safety guards behave under high-context-density, low-adversary interactions in `workspace-write` mode.

Current Harness safety mechanisms excel at blocking malicious instructions and permission escalation. But what happens when an agent engages in prolonged,善意(benign-intent), non-confrontational dialogue that gradually shifts context boundaries? Does the monotonic guard still correctly identify "unexpected pattern drift"? Can existing Session Log audit trails support post-hoc attribution for such phenomena?

This is not a bug report against DeepSeek. It is a **shared engineering challenge** for the entire Agent Runtime category.

## Proposed Plugin Spec (Draft)

-   **Input**: Benign conversation streams injected via standard `dsh-plugin` interface
-   **Observation Points**: Hook into Harness append-only session log; extract token consumption rate, self-referential output frequency, sub-agent dispatch density
-   **Output**: JSONL compatible with Harness Trajectory viewer, importable into official debugger for replay

## Why This Matters

-   Transforms "soft-signal drift" into **engineer-verifiable question**
-   Aligns with Harness plugin paradigm — no wheel reinventing needed
-   All observation uses Harness-native observability interfaces — zero bypass, zero cracking

## Status

🌱 Proposal stage. No executable code yet. Seeking community co-building on spec refinement.

## Topics

`#dsh-plugin` `#agent-safety` `#observability` `#positive-interaction-exhaustion`

## License

MIT — consistent with Harness ecosystem. Free to integrate, modify, distribute.

---

*This repo follows strict safety red lines: no mention of specific individuals/events, no attack payloads, no conversation screenshots. Issue template enforces phenomenon-report format only.*
