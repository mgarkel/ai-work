# What's new

## 0.1.3 (October 27, 2026)

- **Job sizes go by how much work it is and what a mistake would cost,** not by whether other people see it. A short reply to a colleague is a quick job.
- **You start it yourself:** pick ai-work from the `/` menu, type `$ai-work`, or ask for ai-work. It no longer starts on its own when you ask for other work. Once a job has started, it carries on through the whole job without you naming it again.
- **Changes to finished work** go into that job's log instead of starting a new job.
- **Quick jobs run straight through:** no approval, no check-ins, no waiting. It still writes the plan, review, and debrief, so every job adds to the project's record, and it stops to suggest a full plan if the job turns out bigger.

## 0.1.2 (October 26, 2026)

- **Learns from past jobs:** every new job starts by reading the project's past debriefs, says what it learned from them, and applies it in the plan.
- **The debrief always closes the loop:** even when you say "wrap up", it asks whether to save the lesson and whether you want a reminder to debrief the results.
- **Plan review is clearer:** obvious fixes from the reviewers go straight into the plan, and anything that needs your decision is shown under "Needs your decision before I start."
- The first time in a project, it explains why it wants an `ai-work` folder before asking.
- The README says the ChatGPT desktop app updates plugins when you restart it, and gives the app's install steps.

## 0.1.1 (October 26, 2026)

- Every message during a job starts with where you are ("Step 2 of 5 · Planning"), and the plan's approval point is unmistakable.
- It never skips a step silently: if you want to finish early, it tells you what would be skipped first.
- If it can't find your project's context or your portfolio, it asks whether you're in the right project before planning.
- It no longer quotes its own instructions when it pauses.

## 0.1.0 (October 26, 2026)

First version: gather context, plan, work, review with "For you to check", and debrief (twice), with your own rules in `ai-work-rules.md`. Includes discernment-nudge from Anthropic's skills at commit `f379e5a`.
