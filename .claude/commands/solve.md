# Course Question Solver + Audit

Solve the following question using **only** the course materials present in this project directory, then audit your own answer.

**Question:** $ARGUMENTS

---

## Phase 1 — Solve

Follow these steps exactly:

1. Read every course material file in the project root (e.g. `formula_sheet.pdf` and any other `.pdf`, `.md`, `.txt`, or image files that are course content). Do **not** use any knowledge that is not explicitly present in those files.
2. Write your solution clearly, step by step, referencing the specific formulas, theorems, or definitions from the course materials as justification for each step.
3. Present the output under this header:

```
═══════════════════════════════════════
                SOLUTION
═══════════════════════════════════════
```

---

## Phase 2 — Audit

After the solution is written, spawn the `knowledge-audit-reporter` agent as a **foreground** subagent with the following prompt (fill in the placeholders with the actual question and solution text):

> You are auditing a solution produced by another AI agent. The only permitted knowledge sources are the course material files in this project directory: `formula_sheet.pdf` (and any other course files present).
>
> **Question that was solved:** [paste the question here]
>
> **Solution to audit:** [paste the full solution here]
>
> Your task:
> 1. Read all course material files in this directory.
> 2. Go through every claim, formula, theorem, method, and reasoning step in the solution.
> 3. For each one, determine whether it comes from the course materials or from outside knowledge.
> 4. Produce your standard External Knowledge Report.
>
> Present your audit under this header:
> ```
> ═══════════════════════════════════════
>              AUDIT REPORT
> ═══════════════════════════════════════
> ```

Display the audit report immediately after the solution so the user sees both in one response.
