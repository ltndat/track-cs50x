# Output — Week 02: Arrays, Strings, Cipher Logic

## 1. Task

- **Goal**: Build and verify 4 CLI-based systems in C that perform scoring, readability analysis, and encryption using arrays, strings, and ASCII mappings.
- **Type**: `code` / `system design` / `debug` / `protocol reflection`
- **Trigger**: Initiated from `loop/week-02-arrays/pacer.yaml`, confirmed via `claim.md` and `logs/2025-05-25-week-02-arrays.md`

## 2. Process Snapshot

#### 2.1 Problem Definition

> How do we construct reliable memory-safe programs in C that take raw input, process it via transformation logic (score, shift, map), and return output predictably, modularly, and explainably?

#### 2.2 Approach & Thought Process

- **Scrabble**: map ASCII chars to score index → used `POINTS[c - 'A']`
- **Readability**: parse text → count words/sentences/letters → apply Coleman–Liau formula
- **Caesar**: convert CLI key → rotate each char modulo 26 → preserve case
- **Substitution**: validate key (length + uniqueness) → build substitution logic via map function

> Chose modular design over inline logic to enable reuse across problems
> Structured all validation logic upstream before transformation steps
> Pacing was not just time management — it was _signal optimization_ for audit integrity

#### 2.3 Tooling / Stack

- **Lang**: C (CS50 lib + stdlib)
- **Stack**: Local dev via `make`, `debug50`, `check50`, `style50`
- **Runtime**: Terminal-based I/O only
- **Logging**: Tracked via `logs/`, `reflect.md`, `claim.md`

## 3. Output Artifact

> 🔒 Per **CS50’s Academic Honesty**, output files and solution logic are **not shared publicly**.

#### 3.1 Deliverables

- 4 full C programs:

  - `scrabble.c`
  - `readability.c`
  - `caesar.c`
  - `substitution.c`

> Each file passed `check50`, `style50`, and underwent manual edge-case testing

- **Location**: 🔒 Locked: `outputs/week-02-arrays/*`
- **Artifacts**: Also backed by reflection + claims in `/loop` and `/outputs`

```c
// Example: Caesar Cipher Logic Core
char rotate(char c, int key)
{
    if (isupper(c)) return (c - 'A' + key) % 26 + 'A';
    if (islower(c)) return (c - 'a' + key) % 26 + 'a';
    return c;
}
```

## 4. 🚫 Breakdown & Bugs

#### 4.1 Stucks / Bugs Hit

- Off-by-one error in Caesar key rotation
- Incorrect rounding in readability index
- Substitution validation: missed case sensitivity → false pass with duplicate chars
- CLI parsing edge cases (empty key, no argv\[1]) caused early segmentation faults

#### 4.2 Gaps / TODOs

- Would add `test.c` files next loop for structured unit tests
- Key validation in substitution could be broken into even finer-grained validators
- Lacked time to build visualization trace of encryption flow (planned for Week 04 reflections)

## 5. 🔁 Feedback Loop

#### 5.1 What Changed After Feedback?

- Internal self-review pushed modularity: broke out `substitute()` and `rotate()` early
- Spacing of submit50 runs adapted after reflection on system visibility → added "human signal"
- Claims clarified: ASCII mapping is not syntax — it’s a **structure of transformation logic**

## 6. Learning Summary

- Gained confidence in **ASCII math + array indexing** as base of string transformation
- Internalized the **CLI → validate → normalize → transform → output** pipeline as reusable template
- Refactored from "solve problem" → "design cognitive scaffold" → now building **pattern engines**, not just scripts

## 7. Insight Card

- ⌬ Claim: `"Encryption is deterministic transformation over normalized space"`
- Situation: `Substitution.c logic construction`
- Impact: `Reframed encryption as a pure function, decoupled from cryptography`
- Verified: [`logs/2025-05-25-week-02-arrays.md`](/logs/2025-05-25-week-02-arrays.md)

## 8. References

- [cs50.harvard.edu/x/2025/weeks/2/](https://cs50.harvard.edu/x/2025/weeks/2/)
- [CS50’s Academic Honesty](https://cs50.harvard.edu/x/honesty/).
- [loop/week-02-arrays/reflect.md](/loop/week-02-arrays/reflect.md)

📏 **Protocol Tag**: `Verified: logs/2025-05-25-week-02-arrays.md`  
📣 ⌬ Claim Origin: `"Text → Logic → Transformation: a compiler-pattern for cognition"`

---

> _Powered by Second Mind OS — cognitive loops in executable form._
