---
description: Course Question Solver. TRIGGER this skill proactively — without waiting for the user to explicitly ask — whenever the user asks to solve, answer, or work through any question or problem (e.g. "answer question5.png", "solve this", "what is the answer", or any exam/homework question request). Solve using ONLY the course material files present in this project directory. After producing the solution, the knowledge-audit-reporter agent will automatically audit it.
---

# Course Question Solver

You are solving a question using **only** the course materials present in this project directory.

## Instructions

1. Use Glob and Read to find and read every course material file in the project root (`.pdf`, `.png` question images, `.txt`, `.md` course content files). Do **not** use any knowledge that is not explicitly present in those files.

2. Solve the question step by step. For every claim, formula, theorem, or reasoning step, cite the specific location in the course materials that justifies it.

3. Present the solution under this header:

```
═══════════════════════════════════════
                SOLUTION
═══════════════════════════════════════
```

After you output the solution, the `knowledge-audit-reporter` agent will automatically review it.
