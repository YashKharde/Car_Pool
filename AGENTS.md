# Project working agreement

The user wants a gradual learning workflow and found the complete PDF overwhelming.

- Before EACH implementation step, give a short chat update with the step ID, user-visible impact, technical backend/frontend/infrastructure changes, and planned verification.
- Work in understandable increments. Do not silently jump across milestones or implement the entire roadmap in one turn. Honor any later explicit request to continue multiple steps.
- Explain new concepts in plain language using one concrete example.
- Keep backend, frontend, infrastructure, contracts and documentation together in this repository.
- Update docs/progress.md, the relevant docs/steps/Sxx.md record and CHANGELOG.md for completed work. Record actual changes, affected files, checks, limitations and the next action.
- Commit each completed step, including all relevant backend and frontend changes, after appropriate verification. The user has explicitly authorized step commits. Stage only intended project files; never blindly stage unrelated changes or secrets.
- Use step-labelled messages such as `docs(S01): define FareShare scope and ride rules` or `feat(S02): initialize backend and frontend`.
- Push completed step commits to the configured project remote when authenticated access is available. Do not claim a push succeeded without verifying it.
- Keep documentation decisions distinct from implemented behavior and manual reviews distinct from automated tests.
- Add comments that explain business invariants and non-obvious decisions, not every line. Add useful structured logs without credentials or sensitive personal data.
- Do not add scaffolding, framework versions or unimplemented security claims merely to make the repository appear complete.
- Do not spawn subagents unless the user explicitly requests them.

The full roadmap is a reference. The live progress and step record are the concise working guide.
