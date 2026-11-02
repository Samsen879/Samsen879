# Samsen

I build AI systems for learning and tools for running coding agents, and I work on an open problem in additive number theory on the side.

## Projects

### CIE Copilot

*Private, in active development.*

A study product for Cambridge International A-Level Mathematics (9709, with 9231 Further Mathematics in progress). It is organised around a method map: each question type is linked to the trigger that signals it and the procedure that solves it. Practice, marking and review then point a student to the specific method they have not mastered yet, rather than to a whole topic. Answers and marking are grounded in real exam evidence instead of generic prompting.

### [ao-pilot](https://github.com/Samsen879/ao-pilot)

A control plane for running several AI coding agents in parallel on one repository. It keeps durable state for tasks, ownership and handoffs, reconciles that state against GitHub PR / CI / review results, and parks work as `blocked` or `ambiguous` when the sources disagree instead of guessing.

I use it to build CIE Copilot. It runs unattended overnight and has completed more than 100 issues end to end, from issue to reviewed, merged PR.

### [a303656](https://github.com/Samsen879/a303656)

Work on Zhi-Wei Sun's open conjecture [OEIS A303656](https://oeis.org/A303656): every integer n > 1 is a sum a² + b² + 3ᶜ + 5ᵈ.

- Two independently written C++ scanners checked all 1.6 billion consecutive integers just beyond the previously verified bound of 2.4 × 10¹¹ and found no counterexample.
- The repository also maps which proof strategies fail and why, with a theorem index separating what is proved, conditional, finite, or still open.

The conjecture itself remains open.

## Open-source contributions

Merged into [yamadashy/repomix](https://github.com/yamadashy/repomix), a tool that packs a repository into a single AI-friendly file:

- [#1646](https://github.com/yamadashy/repomix/pull/1646) — added a cwd-relative output path style.
- [#1631](https://github.com/yamadashy/repomix/pull/1631) — copy split output files correctly after remote packing.
- [#1622](https://github.com/yamadashy/repomix/pull/1622) — keep `.gitignore` / `.ignore` / `.repomixignore` rules active while leaving the control files out of the packed output.
- [#1618](https://github.com/yamadashy/repomix/pull/1618) — preserve files with the same relative path (e.g. `README.md`) when packing multiple roots.
