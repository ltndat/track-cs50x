# Output — Week 00: Scratch Interactive System

## Task

- **Goal**: Build an interactive system in Scratch that meets CS50x Problem Set 0 constraints: ≥2 sprites, ≥3 scripts, ≥1 conditional, ≥1 loop, ≥1 variable, ≥1 custom block with input.
- **Type**: `code` / `logic` / `design`
- **Trigger**: [`loop/week-00-scratch/pacer.yaml`](loop/week-00-scratch/pacer.yaml)

---

## Process Snapshot

### Problem Definition

Design a behavior-driven logic system using Scratch primitives to simulate control flow, state management, and modularity — all within the constraints of CS50x PSet0.

### Approach & Thought Process

- Decoupled design thinking from visual syntax.
- Started from output requirements → backmapped to logic structure.
- Defined role of each script before implementation to avoid stacking conditionals randomly.
- Prioritized structural clarity over animation aesthetics.

### Tooling / Stack

- Environment: Scratch IDE (Web)
- Output format: `.sb3`
- Artifacts managed in `outputs/week-00-scratch` directory

---

## Output Artifact

### Deliverable

Project implemented in Scratch using required logic patterns:

- Multi-agent structure using two sprites, each driven by event-triggered scripts
- Conditional logic, variable tracking, and repetition encapsulated in reusable blocks
- Behavior mapped from interaction triggers to animated responses

- **Location**: _(Not shared publicly per CS50 Academic Honesty Policy — retained privately for self-verification)_

## Logic Summary (Pseudocode)

- When `green flag` clicked → check if `key space pressed?`  
   → If true → `say "Punch!"`
- Custom block `jumpHeight(height)` → repeats vertical move by input parameter
- Second sprite uses `repeat` block to animate movement
- Variable `score` increments on event

---

## 🚫 Breakdown & Bugs

### Stucks / Bugs Hit

- Missed input parameter in custom block → failed initial `check50`
- Misinterpreted what qualifies as a “script” → added redundant blocks unnecessarily at first

### Gaps / TODOs

- No scoring logic tied to gameplay
- Conditional logic could be tied to state, not just keyboard input
- No reuse of abstraction block across multiple sprites

---

## 🔁 Feedback Loop

### What Changed After Feedback?

- Replaced hardcoded control with state-based conditional
- Abstracted repetitive jump logic to `jumpHeight` with parameterized input
- Used self-review to test logic flow under multiple triggers (`green flag`, `key`, `sprite click`)

---

## Learning Summary

- Skill: Built structural logic system under constraint using visual blocks
- Concept: Mapped condition, loop, state, abstraction to universal programming primitives
- Pattern: Treat each trigger block as an “agent” responding to discrete events

---

## Insight Card

- ⌬ Claim: "Programming is structured control over flow and state, not syntax."
- Situation: Rewriting project after check50 failure
- Impact: Refactored project logic into modular behavior → passed spec + retained clarity
- Verified: [`logs/2025-05-19-week-00-scratch.md`](logs/2025-05-19-week-00-scratch.md)

---

## References

- CS50x Lecture 0 (2025)
- [cs50.harvard.edu/x](https://cs50.harvard.edu/x)
- `loop/week-00-scratch/claim.md`
- `docs/week-00-scratch.md`
- ~~ `outputs/week-00-scratch/scratch.sb3` ~~

> 📏 **Protocol Tag**: `Verified: logs/2025-05-19-week-00-scratch.md`  
> 📣 ⌬ Claim Origin: `"Programming is structured control over flow and state"`  
> 🔒 Artifact withheld in accordance with [CS50 Academic Honesty Policy](https://cs50.harvard.edu/x/honesty/)

---

> _Powered by Second Mind OS_
