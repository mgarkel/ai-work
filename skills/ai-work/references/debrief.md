# Step 5: Debrief

Every debrief opens with this exact sentence: **"Debriefing is how I learn from mistakes and do a better job for you next time."**

**In the chat,** show the debrief itself, not just the lessons: your answers to the four questions (a line or two each), then each suggested lesson with when to apply it, how sure you are, and where you suggest saving it. The user can't approve lessons well without seeing why you're suggesting them.

There are two: the first debrief, after the user's check, and the results debrief, once the real-world result is in. For a **quick** job, debrief only if something went wrong or the user corrected you; otherwise set the status to `debriefed` and stop.

## The first debrief

Read the plan (including the running log), `review.md`, and every correction the user made in this conversation. The user's corrections are often the most useful lesson.

**Answer the four after-action questions,** briefly:

1. What was supposed to happen? (The north star.)
2. What actually happened? (The log, the review findings, the user's check.)
3. Why the difference? For each gap: was it the planning, the work, or a wrong assumption?
4. What do we keep, and what do we change next time?

**Suggest lessons.** Usually one to three; more only if each is truly distinct. Each lesson:

- Is about the work, the audience, the sources, or the way of working. Never about this skill or the tool.
- Is specific: "Fund numbers come from the quarterly report, not the website, which lags a quarter", not "use the right data".
- Stands on its own, so it makes sense months later in another chat.
- Says when to apply it.
- Says how sure you are: low after one job, higher once it has held up more than once.
- Is one of: what worked; what failed and how to prevent it; a correction (a wrong assumption or a bad source fixed); a preference; a reusable template; rules for a kind of work.
- Has a suggested home (see below).

If nothing is worth saving, say so; don't invent lessons.

**The user decides.** They approve, edit, skip, or add each lesson. Save nothing without approval.

**Before saving,** check the existing lessons and rules. If a similar one exists, update it instead of adding a copy. If the new lesson contradicts an older one, show both and ask whether to update or remove the old one.

### Where each lesson goes

| Lesson | Home |
| --- | --- |
| About this project only | `ai-work/lessons.md` |
| About the user, in any project (style, where to find things) | The portfolio file it fits, such as `communication-style.md` or `tools-and-systems.md`; or `ai-work-rules.md` under "About me" if the portfolio isn't connected |
| How this skill should work for them (a kind of work and its rules, an extra reviewer, a change to a step) | `ai-work-rules.md` (see [files.md](files.md)) |

**Suggest changes, not just lessons.** If the review caught something the plan should have prevented, suggest a rule ("For investor updates, check every date against the calendar"). If this job used new rules for a kind of work, offer to save them. If a change would help anyone using this skill, not just this user, save it to their rules now and add: "This may help other people: consider sharing it with your coach."

### Close the first debrief

**Always ask these two questions, even if the user said "wrap up" or "let's finish."** Wrapping up makes the debrief shorter; it never skips them. Without the first, nothing is learned; without the second, the results debrief rarely happens. Ask both in one message:

> **Two quick questions before we finish:**
> 1. **Save this lesson?** [the lesson, one line] (yes / no / change it)
> 2. **Want a reminder to come back and debrief the results** once [the result] is in? (yes / no)

If you suggested more than one lesson, number them under question 1. If there are no lessons worth saving, skip question 1 and say so.

Then:

1. Add what to check later, and when, from the plan.
2. If they want a reminder and you can create scheduled tasks:
   - Set it for the date in the plan, with a prompt like: "Debrief the results of the job in `ai-work/[job folder]` in the [project] project."
   - Ask for each run to open a new chat.
   - Ask the user to confirm it appears in their scheduled tasks. In ChatGPT, it may only exist after they click **Create scheduled task**.
   - Mention that scheduled runs need the computer on and the app open, so a calendar reminder is the dependable backup.

   If you can't create scheduled tasks, suggest a calendar reminder with the same words. Adding it to a connected calendar is writing to a connected app: say which calendar and what the event will say, and create it only after the user says yes. Otherwise give them the text to add themselves.
3. Save `debrief.md` (layout in [templates.md](templates.md)) and set the job's status to `debriefed`.

## The results debrief

When the user says "debrief [job]" and the first debrief is done:

- Ask what happened: the reply, the decision, how the meeting went, the numbers. One round of questions, with what you'd expect as the recommended answer where you can.
- Answer the four questions again, now about the result: did the work achieve its goal?
- Suggest lessons the same way, with the same approval and duplicate checks. Lessons about real-world results are usually the most valuable.
- Add a "Results debrief" section to the job's `debrief.md` (not a new file) and set the status to `results checked`.
