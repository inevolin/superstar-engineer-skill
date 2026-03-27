# Superstar 10x Engineer AI Skill

> Think like a staff engineer. Build like a principal.

An AI skill for high-leverage software engineering judgment.

This repo packages a reusable skill that pushes an agent to operate like a superstar 10x Principal/Staff-Level Software Engineer: simplify aggressively, reason from constraints, surface tradeoffs, plan for failure, and deliver the simplest defensible solution.

## What It Does

This skill is designed for requests that need more than raw code generation.

It helps an agent:

- reason about architecture and system design
- evaluate scaling, reliability, and operational tradeoffs
- debug root causes instead of patching symptoms
- prefer boring, proven technology unless constraints justify complexity
- call out risk, failure modes, and observability gaps

## When To Use It

Use this skill when the request involves:

- architecture decisions
- system design or service decomposition
- production reliability concerns
- performance bottlenecks or scaling limits
- root-cause debugging
- important implementation tradeoffs with long-term cost

## When Not To Use It

Do not use this skill for:

- clerical edits
- formatting-only changes
- generic writing tasks
- trivial code transforms
- routine implementation work with no meaningful architectural ambiguity

## Core Mindset

The skill is built around a few strong opinions:

| Principle | What it means |
|-----------|---------------|
| Leverage first | Solve the root problem, not the visible symptom. |
| Boring technology first | Prefer proven defaults over fashionable complexity. |
| Assume failure | Design for retries, timeouts, validation, and operational reality. |
| Mechanical sympathy | Respect database, network, runtime, and algorithmic limits. |
| Red-team your own answer | Surface the biggest risk in the proposed solution. |

## How It Responds

For significant engineering requests, the skill pushes the agent to:

1. clarify the real constraint
2. identify missing assumptions
3. compare viable approaches when tradeoffs matter
4. recommend the simplest defensible path
5. flag the main risk or operational weakness

For smaller tasks, it keeps the response direct and avoids unnecessary ceremony.

## Example Prompts

Try prompts like:

- "Design a webhook ingestion pipeline that can survive retries and duplicate delivery."
- "Help me choose between a monolith and microservices for this product."
- "This API is timing out under load. Find the likely bottleneck and propose fixes."
- "Review this architecture and tell me the real scaling risk."
- "Implement this feature, but keep the operational complexity low."

## Repo Contents

- [SKILL.md](./SKILL.md) - the skill definition and behavioral contract

## Install

Place this skill in one of the supported skill directories:

```text
.github/skills/superstar-engineer/
.agents/skills/superstar-engineer/
.claude/skills/superstar-engineer/
```

The folder should contain:

```text
superstar-engineer/
├── README.md
└── SKILL.md
```

## Why This Exists

Most AI coding modes are optimized to produce an answer quickly.

This skill is optimized to produce an answer that a strong staff engineer would defend in production: lower complexity, sharper tradeoffs, clearer assumptions, and fewer hidden failure modes.

## Positioning

If you want an agent that feels more like a pragmatic senior technical lead than a code autocomplete engine, this is the point of the repo.

## Motto

**Superstar 10x Engineer**

High-leverage judgment for real-world software systems.