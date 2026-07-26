# Agent operating instructions

This repository has Addy Osmani's `agent-skills` pack installed in `.agents/` for coding agents that can read project instructions.

## How to use the installed skills

1. Before starting any non-trivial task, read `.agents/skills/using-agent-skills/SKILL.md` and select the matching workflow.
2. Load only the skill(s) needed for the current task from `.agents/skills/<skill-name>/SKILL.md`; do not load the entire pack into context unless explicitly asked.
3. Treat each skill as a workflow, not as optional reference material. Follow its process, verification gates, and anti-rationalization guidance unless a higher-priority system/developer/user instruction conflicts.
4. If a skill points to `references/<file>.md`, resolve that path as `.agents/references/<file>.md` in this repository.
5. If a skill points to `agents/<persona>.md`, resolve that path as `.agents/agents/<persona>.md` in this repository.
6. Keep scope disciplined: do not modify unrelated files just because a skill mentions a broader lifecycle step.
7. Always provide verification evidence before saying work is complete.

## Intent-to-skill quick map

- Unclear requirements or "interview me" requests: `interview-me`
- Vague idea refinement: `idea-refine`
- New feature or significant change: `spec-driven-development` then `planning-and-task-breakdown`
- Multi-file implementation: `incremental-implementation` plus `test-driven-development`
- UI work: `frontend-ui-engineering`
- API or module boundary design: `api-and-interface-design`
- Framework/library correctness: `source-driven-development`
- High-stakes or unfamiliar code decisions: `doubt-driven-development`
- Broken tests/build/runtime behavior: `debugging-and-error-recovery`
- Code review: `code-review-and-quality`
- Refactoring for clarity: `code-simplification`
- User input/auth/secrets/third-party integrations: `security-and-hardening`
- Performance work: `performance-optimization`
- Git/commits/releases: `git-workflow-and-versioning`
- CI/CD automation: `ci-cd-and-automation`
- Migrations/deprecations: `deprecation-and-migration`
- Documentation/ADRs: `documentation-and-adrs`
- Logs/metrics/tracing/alerts: `observability-and-instrumentation`
- Launch/deploy readiness: `shipping-and-launch`

## Installed files

- Skills: `.agents/skills/`
- Supplemental references: `.agents/references/`
- Specialist personas: `.agents/agents/`
- Skill lockfile: `skills-lock.json`
- Upstream license: `.agents/agent-skills-LICENSE`
