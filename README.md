# Goal-led Acceptance

A reusable agent skill for guiding a user through acceptance of actual deliverables against a core goal, one decision at a time. It works with websites, handbooks, reports and other artifacts. It is not a substitute for implementation review, user judgment or outcome measurement.

## Use

Copy `skills/goal-led-acceptance` into your agent's supported skills directory (for Codex, `~/.codex/skills/`), then invoke:

```text
Use $goal-led-acceptance to guide me through acceptance of this deliverable against its core goal. Start with one unit and wait for my decision.
```

Provide the goal and locations of authoritative artifacts if they are not already available. The agent should reuse existing decisions and evidence, inspect actual work, distinguish tool checks from human acceptance and experiments, and keep each conclusion within its evidence. You can request faster pacing, skipping or batch review.

The skill does not grant permission to publish or close tasks, guarantee outcomes, or require particular tools or other skills. Design acceptance, release readiness and measured effects remain distinct decisions.

## Contents and maintenance

- [Skill instructions](skills/goal-led-acceptance/SKILL.md)
- [Fictional worked example](skills/goal-led-acceptance/references/example.md)
- [Behavioral validation](tests/validation.md)

This repository is the sole maintenance source. Installed copies are distributions; update them from this repository. All examples and test materials are fictional and contain no customer or private project data.

Licensed under the MIT License.
