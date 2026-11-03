# Proof Autopsy

Proof Autopsy is a practice app where students dissect short proofs one step at a time. In Autopsy Mode they reveal a proof step by step, flag the first step that cannot be accepted, and name the error from a fixed set of four: False premise, Division by zero, Circular reasoning, and Algebraic error. Some proofs in the bank are sound, so deciding that a proof is valid is part of the practice. In Sort Mode they classify short arguments as inductive or deductive and judge whether each argument actually settles its claim for all cases.

Math 2201 Unit 7: Inductive and Deductive Reasoning (indicators 2.8, 2.7)

## How students use it

- Autopsy Mode: read the claim, then use Next step to reveal the proof one step at a time. The moment a step cannot be accepted, choose Flag this step and pick the error name. If every step holds up, reveal all steps and choose This proof is valid. Feedback responds to both the step flagged and the error name chosen, and gives the correction, or explains why the proof needed none.
- Sort Mode: read the argument, pick Inductive or Deductive, then pick whether the argument settles its claim or does not settle it. Feedback confirms or corrects both choices and explains why.
- Nothing is recorded by the app and nothing leaves the page. It is practice only.

## Printable autopsy report

The Autopsy Report at the bottom of the page fills in as students work: each completed autopsy adds the proof title, the step the student flagged, the first step that actually breaks, the error name chosen versus the accepted one, and the correction text, and each completed sort adds a summary line. There is a free-text notes box, and the Print button prints just the report sheet, so students can submit it to an assignment folder if the teacher asks.

## Tech note

Single HTML file, no dependencies, works offline. All content and logic are inline in index.html. A Node harness (harness.js) checks the proof bank by evaluating the equation steps at their test assignments, checks the sort bank for consistency, and exercises the serving functions across thousands of seeded draws: run `node harness.js`.

GitHub topics when published: math-2201, inductive-deductive-reasoning, draft (draft removed after QA).
