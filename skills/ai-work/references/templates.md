# File layouts

Use these layouts. Leave out sections that don't apply (a quick job's plan is much shorter); don't leave empty headings in a finished file.

## `ai-work/index.md`

```markdown
# AI work

| Started | Job | Size | Status | Folder |
| --- | --- | --- | --- | --- |
| 2026-10-26 | Q3 investor update | standard | waiting for your check | [2026-10-26-q3-investor-update](2026-10-26-q3-investor-update/plan.md) |
```

Statuses: `planning`, `working`, `in review`, `waiting for your check`, `debriefed`, `results checked`.

## `ai-work/lessons.md`

```markdown
# Lessons for this project

Read before every job in this project. These override the general rules in ai-work-rules.md for this project.

## [Short title]
- **Lesson:** [one or two specific sentences]
- **When to apply:** [the situation]
- **Confidence:** [low / medium / high], from [job folder name(s)]
```

## `plan.md`

```markdown
# Plan: [job]

**Size:** [quick / standard / important] · **Started:** [date] · **Status:** [status]

## North star
- **Objectives:** …
- **Outcomes:** …
- **Great versus acceptable:** …

## Context
- [Fact or point] (source: …)

## Learned from past jobs
- [What a past debrief or lesson said, and how this plan applies it] (from: [job folder])

## Decisions
| Decision | Chosen over | Why | Decided by |
| --- | --- | --- | --- |

## Assumptions and open questions
- **Assumption:** …
- **Open question:** …

## Steps
1. [Step] → serves [outcome]. [Check-in / stop point, if any]

## Stop points
- …

## Risks (pre-mortem)
| Risk | How we prevent it |
| --- | --- |

## Plan review
- [Reviewer]: [finding] → [what changed, or why not]

## Checklist: what I'd be most embarrassed to get wrong
- [ ] …

## Rules for this kind of work
- …

## How the work will be checked
- **Self-check:** a source for every fact; numbers rechecked; outcomes, definition of done, and checklist gone through line by line.
- **Review:** [reviewers]

## What to check later
- [What result, how we'll know, and when]

## Running log
### [date] [milestone]
- Produced: [what], saved at [path]
- Changed from the plan: [what and why]
- Blocked: …
```

## `review.md`

```markdown
# Review: [job]

## Plan review
[Reviewer] (given [what]): [finding] → [changed / not changed, and why]

## Work reviewers
[Reviewer]: given [what it was given].

## Findings
### Must fix
- **[Title]** ([reviewer]): "[quote]". [What would go wrong.] → [Fixed: … / Asked: …]
### Should fix
### Nice to fix
### Worth knowing
### What's working

## Fixes and rechecks
- [Fix] → recheck: [result]

## For you to check
**Things I was unsure of**
1. "[quote]": [what to check, why it matters, how to check it]

**Critical things to check yourself**
1. …

Come back and discuss any concerns or questions.
```

## `debrief.md`

```markdown
# Debrief: [job]

## First debrief ([date])
1. **What was supposed to happen:** …
2. **What actually happened:** …
3. **Why the difference:** …
4. **Keep / change:** …

### Lessons saved
- [Lesson] → saved to [file]

### What to check later
- [What, when] · Reminder: [scheduled / calendar / none]

## Results debrief ([date])
…
```

## `ai-work-rules.md`

```markdown
# My AI work rules

These are my rules for the ai-work skill. They override its defaults in every project. A project's ai-work/lessons.md overrides these for that project.

## Kinds of work
### [Kind, e.g. Investor update]
- …

## Reviewers
- …

## Planning, work, review, debrief
- …

## About me
- …
```
