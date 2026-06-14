# Samsen

Building **CIE Copilot**, an evidence-grounded learning runtime for Cambridge A-Level STEM.

I work on learning systems where AI is not just a chat layer, but part of a structured study loop: paper-aware workspaces, exam evidence, server-side marking, review scheduling, and durable learning state.

## Current Focus

### CIE Copilot

[CIE Copilot](https://github.com/Samsen879/ciecopilot-home) is a syllabus-aware learning OS for Cambridge International A-Level preparation, starting with 9709 Mathematics.

The project is built around a narrower but deeper problem:

- map past-paper work into paper, topic, and question-type contexts;
- answer from exam-grounded evidence instead of generic prompts;
- keep learning sessions, artifacts, review tasks, and mastery signals as structured state;
- separate released scoring paths from fallback behavior;
- use production gates before treating exam data as reliable product surface.

Current public README covers the product direction, architecture, data assets, and release posture.

## Selected OSS Contributions

I also contribute focused fixes to open-source developer tools.

- [yamadashy/repomix#1622](https://github.com/yamadashy/repomix/pull/1622) - fixed an ignore-file edge case so `.gitignore`, `.ignore`, and `.repomixignore` rules remain active while the control files stay out of packed output.
- [yamadashy/repomix#1618](https://github.com/yamadashy/repomix/pull/1618) - fixed multi-root duplicate relative paths so files like `README.md` or `src/index.ts` from different roots are preserved correctly in output.
- [yamadashy/repomix#1631](https://github.com/yamadashy/repomix/pull/1631) - proposed a remote-mode fix for copying split output files after remote packing.

## What I Care About

- Evidence before claims.
- Narrow, well-bounded product surfaces.
- Runtime state that survives beyond a single AI response.
- Tests and release gates that make product behavior inspectable.

## Links

- Main project: [CIE Copilot](https://github.com/Samsen879/ciecopilot-home)
- GitHub: [@Samsen879](https://github.com/Samsen879)
