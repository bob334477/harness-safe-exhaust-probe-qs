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



<details>
<summary>🔍 展开查看思考锚点地图  </summary>
## A Living Map of Our Thinking



# AI Reliability Assessment: Anchors & Seeds

> “评估AI的可靠性，不是证明它能做什么，而是诚实面对它不能保证什么。”  
> —— 本项目的核心信念

## 🔱 Core Anchors（不可动摇的脊梁）
1. **Human-AI Collaboration Boundary**  
   AI reliability ≠ omniscience. It resides in clearly demarcating *what machines can bear* vs. *what humans must guard*.
2. **Negative Epistemology of Evaluation**  
   Assessments reveal limits, not capabilities. Safety is falsifiable, not provable.
3. **Human-Centered Oversight**  
   The ultimate metric is human cognitive load, accountability, and meaning-making—not technical compliance.

## 🌿 Supporting Tendrils（隐性支撑筋脉）
- Surrogate reward design → Handling unobservable capabilities
- Axiomatic constraint framing → Formal language for boundaries
- Intent-action consistency → Process-oriented trustworthiness
- State-prediction separation hypothesis → Epistemic foundation for division of labor
- Adaptive practice grammar → Resilience in ecological validity gaps

## 🌱 Seed Vault（未来可能唤醒的种子）

| Seed | Potential Awakening Context |
|------|-----------------------------|
| Embodied semantic-spatial coupling (Robostral) | If expanding to embodied AI assessment |
| Clinical responsibility anchoring (Physician-Oversight) | If deepening medical AI ethics |
| Red-team falsifiability logic | If addressing overpromising on safety |
| Meta-cognitive research questioning (Auto-Research) | If reflecting on framework evolution |

## 💬 How to Use This Map
- **For writing**: Let Core Anchors guide your argument’s gravity.
- **For revision**: Check if new content aligns with or stretches Supporting Tendrils.
- **For future work**: Visit Seed Vault when exploring adjacent territories.
- **For rest**: Close this file. The anchors hold even when you’re away.

---
*This repository is a living thought-space, not a static archive.  
Updated with care by [Your Name] & Weiming Teacher.*
 </details>
