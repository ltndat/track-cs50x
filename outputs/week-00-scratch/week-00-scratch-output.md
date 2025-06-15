# Output — Week 00: Scratch Interactive System

## 1. Task

- **Goal**: Build an interactive system in Scratch that meets CS50x Problem Set 0 constraints: ≥2 sprites, ≥3 scripts, ≥1 conditional, ≥1 loop, ≥1 variable, ≥1 custom block with input.
- **Type**: `code` / `logic` / `design`
- **Trigger**: [`loop/week-00-scratch/pacer.yaml`](/loop/week-00-scratch/pacer.yaml)

## 2. Process Snapshot

#### 2.1 Problem Definition

Design a behavior-driven logic system using Scratch primitives to simulate control flow, state management, and modularity — all within the constraints of CS50x PSet0.

#### 2.2 Approach & Thought Process

- Decoupled design thinking from visual syntax.
- Started from output requirements → backmapped to logic structure.
- Defined role of each script before implementation to avoid stacking conditionals randomly.
- Prioritized structural clarity over animation aesthetics.

#### 2.3 Tooling / Stack

- Environment: Scratch IDE (Web)
- Output format: `.sb3`
- Artifacts managed in `outputs/week-00-scratch` directory

## 3. Output Artifact

#### 3.1 Deliverable

> 🔒 Per **CS50’s Academic Honesty**, output files and solution logic are **not shared publicly**.

Fully working `.sb3` file with the following:

- Amon sprite: conditional attack behavior with custom block (`jumpHeight`)
- Anina sprite: animated loop and interaction trigger
- Variable tracking (`score`), event-driven scripts, and branching logic

- **Location**: `outputs/week-00-scratch/scratch.sb3`

## 4. 🚫 Breakdown & Bugs

#### 4.1 Stucks / Bugs Hit

- Missed input parameter in custom block → failed initial `check50`
- Misinterpreted what qualifies as a “script” → added redundant blocks unnecessarily at first

#### 4.2 Gaps / TODOs

- No scoring logic tied to gameplay
- Conditional logic could be tied to state, not just keyboard input
- No reuse of abstraction block across multiple sprites

## 5. 🔁 Feedback Loop

#### 5.1 What Changed After Feedback?

- Replaced hardcoded control with state-based conditional
- Abstracted repetitive jump logic to `jumpHeight` with parameterized input
- Used self-review to test logic flow under multiple triggers (`green flag`, `key`, `sprite click`)

## 6. Learning Summary

- Skill: Built structural logic system under constraint using visual blocks
- Concept: Mapped condition, loop, state, abstraction to universal programming primitives
- Pattern: Treat each trigger block as an “agent” responding to discrete events

## 7. Insight Card

- ⌬ Claim: "Programming is structured control over flow and state, not syntax."
- Situation: Rewriting project after check50 failure
- Impact: Refactored project logic into modular behavior → passed spec + retained clarity
- Verified: [`logs/2025-05-19-week-00-scratch.md`](logs/2025-05-19-week-00-scratch.md)

## 8. References

- CS50x Lecture 0 (2025)
- [cs50.harvard.edu/x](https://cs50.harvard.edu/x)
- [CS50’s Academic Honesty](https://cs50.harvard.edu/x/honesty/).
- `loop/week-00-scratch/claim.md`
- `docs/week-00-scratch.md`
- 🔒 Locked: `outputs/week-00-scratch/scratch.sb3`

> 📏 **Protocol Tag**: `Verified: logs/2025-05-19-week-00-scratch.md`  
> 📣 ⌬ Claim Origin: `"Programming is structured control over flow and state"`

---

> _Powered by Second Mind OS_
