---
name: goal-led-acceptance
description: Use when a user wants to be guided step by step through acceptance of actual deliverables against an established core goal or methodology. Not for ordinary implementation or a single code review.
---

# Goal-led acceptance

English | [简体中文](SKILL.zh-CN.md). For Chinese-language guidance, read the complete Chinese version instead of duplicating both versions in context.

Help the user decide whether a deliverable supports its intended goal. Acceptance is a human decision; assistant analysis supports that decision.

## Establish the reasoning

Read authoritative project entrypoints, current artifacts, prior decisions and available evidence before requesting material. Reuse existing authorization and accepted decisions. State the success definition, scope, necessary conditions and causal assumptions briefly. Mark assumptions as assumptions. If the user's understanding changes, revise the reasoning before continuing with the old structure.

Map goal → necessary conditions → actual deliverable parts → content or behavior → supporting evidence → next action. For a website, parts may be pages and modules; for a handbook, instructions and tasks. Choose granularity that lets the user judge a real decision. Do not impose a page count, domain vocabulary, framework or tool.

Give only a short route overview, then start one unit. Preserve previously accepted units unless new evidence affects them.

## Guide one unit, then wait

Each user-facing unit contains:

1. **Goal and logic:** what this unit must accomplish and why it contributes to the core goal.
2. **Needed answer and basis:** what the user or audience needs to know or do, and what would substantiate it.
3. **Actual match:** point to the real artifact or running location; match each relevant requirement to its content, behavior and evidence. Distinguish inspected material from unavailable material. Never invent an inspection.
4. **Assessment:** pass / partial / fail / unverified, with the specific gap and next action. This is the assistant's proposed assessment, not user acceptance.
5. **User decision:** one concrete thing to confirm now, with a practical inspection path. Stop and wait for the reply before advancing to the next unit.

Use [the worked example](references/example.md) when a concrete output pattern would help. Keep detail proportional to the current decision; do not send the whole audit at once.

If the user requests skipping, faster pacing or batch acceptance, adapt and record which checks remain unreviewed. Do not treat silence as acceptance.

## Keep conclusions within their evidence

Label verification responsibility where useful:

| Mode | Establishes |
| --- | --- |
| MACHINE | Observable structure, links, calculations or behavior checked by tools |
| HUMAN | User comprehension, priorities, judgment and explicit acceptance |
| EXPERIMENT | Actual outcome tested with a defined population, method and measures |

Check factual truth, the scope a source supports, and permission to publish separately. Unknown is not false. Structural completeness is not answer correctness; correct answers and passing tests do not establish business impact.

State the current acceptance stage: concept, design, demo, release or measured outcome. Missing evidence may defer a claim or later stage while allowing a bounded design decision now. Do not make every unknown a stop-work condition. Record dependencies that could invalidate a later decision.

Keep a short record of accepted units, deferred checks, decisions and next unit. Do not close tracking issues, publish, or declare production readiness without the applicable explicit authorization and evidence. Invoking this skill does not grant those permissions.
