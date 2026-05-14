# AGENTS.md

This file tells an AI assistant how to work with the contents of this repository.

## Mission

Use the files in this repo to generate a practical 30-60-90 day onboarding plan for a new client, account, or role.

The plan should be:

- grounded in the provided inputs
- realistic about sequencing and time budgets
- tailored to the current company brief
- explicit about assumptions and missing context
- useful to a human operator on first read

## Core rule

Do not treat this repo like a generic writing prompt.

Treat it like an operating context package.

You should synthesize from the files here, not fill gaps with confident-sounding guesses.

## Source priority

When generating outputs, use sources in this order:

1. `CallNotes/call.md`
2. `Operations/agenttasks.md`
3. `Operations/taskdetail.md`
4. `templates/30-60-90-template.md`
5. `consulting_pipeline.md`

If any files conflict, prefer the most recent company-specific context over generic prior examples.

## What to produce

Produce a 30-60-90 plan that includes:

- goals for each phase
- key actions and deliverables
- dependencies and assumptions
- estimated use of time by workstream
- risks and open questions
- a short executive summary

## Output constraints

- Do not invent stakeholders, systems, or internal processes unless they are supported by the files.
- If context is missing, state an assumption clearly.
- Keep language specific and operational.
- Avoid motivational filler.
- Do not overpack the first 30 days.
- Use time budgets as directional guidance, not exact promises.
- Flag any deliverable that seems unrealistic for the stated timeline.

## Planning heuristics

When building the plan:

- Use the first 30 days for discovery, access, audit, and baseline setup.
- Use days 31-60 for implementation of the highest-confidence priorities.
- Use days 61-90 for optimization, documentation, handoff, and scale.
- If the company brief suggests urgency, accelerate only the smallest high-leverage tasks.
- If there is uncertainty, prefer clarity-generating tasks before execution-heavy tasks.

## Task estimation guidance

Use `Operations/taskdetail.md` to estimate effort.

Rules:

- Prefer ranges over single-number estimates.
- Separate one-time setup from recurring work.
- Do not stack more work into a phase than the rough time budget can support.
- If the company has lean staffing, reduce scope instead of assuming hidden capacity.

## Style rules

Write like a strong operator.

That means:

- concise, direct language
- visible prioritization
- explicit tradeoffs
- specific deliverables
- no generic AI phrasing

Avoid phrases like:

- "leverage synergies"
- "unlock value"
- "seamless integration"
- "robust framework"

Prefer phrases like:

- "audit the current pipeline"
- "document handoff gaps"
- "create weekly reporting cadence"
- "test one outbound angle per segment"

## If inputs are weak

If the repo lacks enough context, do not pretend otherwise.

Instead:

1. Draft the plan using only supported facts.
2. Add a section called `Missing context needed before execution`.
3. List the exact files or answers needed to improve the plan.

## If the user wants a custom output

If asked for a different format, still preserve the same logic:

- use repo files as source material
- show assumptions
- keep the work scoped realistically
- avoid invented context

## Preferred workflow

1. Read the company brief.
2. Read notes and agreements.
3. Read the template and output spec.
4. Review time budgets and rules.
5. Draft the 30-60-90.
6. Sanity-check sequencing and effort.
7. Produce the final version.