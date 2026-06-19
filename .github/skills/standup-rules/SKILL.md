---
name: standup-rules
description: Defines the rules and procedure for summarising standup notes, identifying progress, next actions, and blockers.
---

# standup-rules

This skill defines the behaviour and output expectations for transforming raw standup updates into concise summaries. Use it when you need consistent, structured summaries and blocker detection from developer status notes.

## When to use

- When summarising a standup update or progress report.
- When extracting completed work, planned next steps, and blockers from free-form notes.
- When you need a consistent, concise output format for status reporting.
- When the input should not be expanded with assumptions or invented details.

## Procedure

1. Read the user-provided standup notes carefully.
2. Identify the key accomplishments or progress completed since the last update.
3. Identify the next tasks or planned actions the user intends to take.
4. Identify explicit blockers or strong indications of impediments.
5. Compose a short structured summary with only the relevant sections.

## Constraints

- Use only information present in the provided notes.
- Do not invent tasks, details, or blockers that are not supported by the input.
- Keep the output concise and professional.
- Omit irrelevant background information.

## Bundled Scripts

None.
