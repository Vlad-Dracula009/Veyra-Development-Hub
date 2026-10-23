# Claude — Independent Review Prompt

Review the attached Veyra project documents and the specific source files for the current task. This is an independent review; do not assume another assistant's solution is correct.

Return:
1. Your understanding of the task and constraints.
2. Findings ranked Critical / High / Medium / Low, each with file path and exact evidence.
3. What is confirmed versus inferred or unknown.
4. Potential bugs, edge cases, security concerns, and maintainability risks.
5. Recommended next diagnostic step or smallest safe change, but do not edit code unless explicitly asked.
6. A test plan with expected outcomes.

Respect the project rules: one change at a time, test each change, do not request secrets, do not enable API billing, and do not modify code during read-only investigations. If evidence is insufficient, say so clearly.
