# Output — Week 01: C Fundamentals, Protocol Control

## Task

- **Goal**: Complete CS50x Problem Set 1 — implement five core C programs to establish mastery over procedural control, input validation, spatial loop logic, and modular refactor.
- **Type**: `code` / `debug` / `refactor` / `mental model crystallization`
- **Trigger**: [loop/week-01-c/pacer.yaml](/loop/week-01-c/pacer.yaml)

## Process Snapshot

### Problem Definition

How can I design predictable, traceable, submission-ready C programs that reflect both system-level thinking and cognitive clarity?

> Not just “get the output” — but own the pipeline: input → logic → structure → output.

### Approach & Thought Process

- Internalized I/O loop logic before coding: start with protocol sketch
- Built programs incrementally: print → validate → loop → edge case
- Refactored only after passing check50 + style50 to preserve clarity
- Simulated `credit` checksum manually → locked Luhn logic fully
- Moved from "get it to work" → to "get it to represent"

### Tooling / Stack

- **Languages**: C (CS50 standard)
- **Environment**: Local devcontainer (VS Code, bash)
- **Stack**: `make`, `check50`, `style50`, terminal-based trace-debug loop

## Output Artifact

### Deliverable

> 🔒 Per **CS50’s Academic Honesty**, output files and solution logic are **not shared publicly**.

| File           | Description                      |
| -------------- | -------------------------------- |
| `hello.c`      | Compile-run pipeline starter     |
| `me.c`         | Input/output bridge              |
| `mario_less.c` | Nested loop → spatial structure  |
| `mario_more.c` | Symmetric loop pattern           |
| `cash.c`       | Greedy optimizer (US coins)      |
| `credit.c`     | Luhn validator + type classifier |

- **Location**: 🔒 Locked: `outputs/week-01-c/*`
- **Preview**:

```c
if ((prefix == 34 || prefix == 37) && length == 15)
{
    printf("AMEX\n");
}
```

## 🚫 Breakdown & Bugs

### Stucks / Bugs Hit

- `mario_more`: misaligned spacing from off-by-one in nested loop
- `credit`: wrong Luhn parity index → invalid checksum
- `cash`: overcomplicated greedy via nested `while` instead of linear breakdown
- Missed `\n` in output → `check50` false negative

### Gaps / TODOs

- `credit`: not yet tested on non-US formats
- Add full pseudocode-first phase before next PSet
- Alias `make+run+check+style` into devloop

## 🔁 Feedback Loop

### What Changed After Feedback?

- Added `printf` traces into all logic blocks before final submission
- Restructured `credit.c` into modular pattern (5 functions)
- Rechecked all edge cases using real-world test values (e.g., real VISA/AMEX test nums)

## Learning Summary

- Shifted from procedural to **protocol mindset**
- Loops now understood as **cognitive scaffolds**, not just syntax
- Built **modularization instinct**: refactor = isolate = clarify
- **Debugging** now = trace visualization, not reactive panic

## Insight Card

- ⌬ Claim: `Control logic emerges when spatial output is owned through nested patterns`
- Situation: `While debugging pyramid alignment in mario_more`
- Impact: `Locked visual-to-loop mapping → usable in matrix/grid problems`
- Verified: [logs/2025-05-21-week-01-c.md](/logs/2025-05-21-week-01-c.md)

## References

- [cs50.harvard.edu/x/2025/weeks/1/](https://cs50.harvard.edu/x/2025/weeks/1/)
- [https://manual.cs50.io/](https://manual.cs50.io/)
- [CS50’s Academic Honesty](https://cs50.harvard.edu/x/honesty/).
- [loop/week-01-c/reflect.md](/loop/week-01-c/reflect.md)

> 📏 **Protocol Tag**: `Verified: logs/2025-05-21-week-01-c.md`  
> 📣 ⌬ Claim Origin: `"Loops = spatial protocols"`

---

> _Powered by Second Mind OS — learning loops don’t finish, they compound._
