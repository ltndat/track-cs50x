# Week 01 — C Fundamentals & System Bootstrapping

> Track: cs50x
> Week: 01
> Protocol: Second Mind OS
> Format: Verified Thinking Notes + Schema-Driven Capture

## Objective

- **Core Concept(s)**:

  - Procedural flow in C
  - Compile → Execute → Validate loop
  - System protocols: input/output handling, control structures, greedy algorithms

- **Outcome**:

  - Ship modular programs in C with `get_int`, `printf`, loops, and Luhn logic
  - Validate control over system pipeline (`make`, `check50`, `submit50`)

- **Protocol Scope**:
  This note anchors the **PACER loop** across Lecture 1 and Problem Set 1. It acts as a **loop-state snapshot** prior to abstraction elevation.

## Concept Map / Schema

```mermaid
graph TD
  A[Execution Flow in C] --> B[Input Validation]
  B --> C[get_int(), do...while]
  A --> D[Computation Loop]
  D --> E[nested for loops → Mario]
  A --> F[Algorithmic Logic]
  F --> G[Luhn’s Check → Credit Validation]
```

- **Compile-Run Pipeline**:

  - `make file.c` → binary
  - `./file` → execution

- **Patterned Logic**:

  - `Cash`: greedy optimization
  - `Mario`: visual loop → geometry

## Mental Models

| Concept       | Model / Metaphor                           | First-principle Breakdown               |
| ------------- | ------------------------------------------ | --------------------------------------- |
| Loop Control  | Stair-builder / row-wise generator         | Outer = line, Inner = shape builder     |
| Luhn Checksum | Double-pass verifier → data fingerprinting | Split → Transform → Validate → Classify |
| CLI Pipeline  | Manual compiler → build loop               | Human-triggered automation chain        |

## 📣 ⌬ Insight Claims

| ⌬ ID | Claim Statement                                                           | Trigger Point        | Verified In                    |
| ---- | ------------------------------------------------------------------------- | -------------------- | ------------------------------ |
| 001  | "Control flow becomes geometry when nested in space."                     | Mario → pattern loop | `logs/2025-05-21-week-01-c.md` |
| 002  | "Checksum isn't magic — it's math over time."                             | Credit → Luhn algo   | `loop/week-01-c/reflect.md`    |
| 003  | "If you can modularize logic, you can protocolize thought."               | Refactor credit.c    | `loop/week-01-c/claim.md`      |
| 004  | "Greedy works not because it’s simple, but because the domain is convex." | Cash logic test      | `loop/week-01-c/reflect.md`    |

## 🚧 Blockers / Ambiguities

- \~ Re-mapping alignment logic in `Mario` to a general spacing algorithm
- \~ `Credit`: alternate card length handling and prefix accuracy under different locales
- \~ Validating behavioral consistency between `while` vs `do...while` with edge case inputs

## 🧪 Tests / Self-Checks

1. Why must `get_long()` be used instead of `get_int()` in `credit.c`?
2. Recreate the pyramid from `mario.c` for height = 5, using a hand-drawn matrix.
3. What logic breaks if we forget to add `\n` in `printf()`?
4. Simulate Luhn checksum by hand for: `4003600000000014`.

## 📃 Trace Log / Learning Path

- [x] VS Code + Docker devcontainer setup
- [x] Completed: `hello.c`, `hello_me.c`, `mario_less.c`, `cash.c`
- [x] Completed challenge: `mario_more.c`, `credit.c`
- [x] Refactored `credit.c` into modular functions
- [x] Style-verified & submitted all code

## 🔁 Linked Protocol Loops

| Loop Phase | Linked File                             |
| ---------- | --------------------------------------- |
| Plan       | `loop/week-01-c/pacer.yaml`             |
| Reflect    | `logs/2025-05-21-week-01-c.md`          |
| Claim      | `loop/week-01-c/claim.md`               |
| Reflect+   | `loop/week-01-c/reflect.md`             |
| Output     | `outputs/week-01-c/week-01-c-output.md` |

---

> _Powered by **Second Mind OS Lab** — recursive protocol lab for sovereign cognitive architecture._
