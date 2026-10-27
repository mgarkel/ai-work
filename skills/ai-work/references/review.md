# Step 4: Review, then the user's check

The work is checked by reviewers who didn't do it, then by the user. For a **quick** job, skip the reviewers: do your own check (the "Check yourself" list in [work.md](work.md)), save "For you to check" in `review.md`, and go straight into step 5 without waiting. The list goes in the final message, with the debrief.

## The reviewers

Use the briefs in [reviewer-briefs.md](reviewer-briefs.md), section "Work reviewers":

| Reviewer | Runs |
| --- | --- |
| Reader test | Always |
| Checklist and done check | Always |
| Fact and source check | Always |
| Audience and sensitivity | Always |
| Devil's advocate | Only when the work recommends or decides something |

Add any reviewers the user's rules ask for.

**Fresh means no chat history.** Start each reviewer as a separate helper (a sub-agent) without this conversation's history. In ChatGPT, helpers get the conversation by default, so ask for a clean one that doesn't. In Claude, helpers start without it. A fresh reviewer can still see the project's files; that's fine. What it must not have is this conversation.

Give each reviewer only what its brief lists, and tell it exactly what it was given. Reviewers only read; they don't change any files.

**If you can't start helpers,** tell the user. Do each review yourself as a clearly separate pass, and offer the reader test as a brief the user can paste into a new chat (with the finished work) to get a truly fresh reader.

## Combine the findings

Save every reviewer's findings in `review.md` (layout in [templates.md](templates.md)), then combine them:

- **Keep only real findings.** Each must quote the passage it's about and say what would go wrong for the reader. Drop anything you can disprove from the plan or the sources, and preferences with no real benefit.
- **Merge duplicates.** When reviewers disagree, check the disagreement against the plan and the evidence before asking the user. Disagreement alone doesn't prove a problem.
- **Sort:** must fix (would cause real harm or miss an outcome), should fix (a meaningful improvement), nice to fix (polish). Concerns a reviewer couldn't verify go under "Worth knowing".
- **Say what's working,** briefly.

## Fix

- **Clear fixes:** one right answer that stays inside the approved plan (a wrong number, a missing source, an unclear sentence). Make them, and list what you changed.
- **Judgment calls:** a fix that changes the meaning or the scope, or that needs the user's preference. Ask, with your recommendation.
- **Recheck.** After fixing, have a fresh reviewer check the changed parts. Repeat until nothing new turns up. If a must-fix is still open after two rounds, stop and ask the user.

Record the fixes and rechecks in `review.md`.

## For you to check

Then give the user a short list: usually three to seven items, the most important first, in two groups.

- **Things I was unsure of:** from your confidence check and the "Worth knowing" list.
- **Critical things to check yourself:** items from the job's checklist, the most important facts and numbers, and judgment calls you made.

For each item: where it is in the work (quote a few words), what to check, why it matters, and how to check it ("open the Q3 report, page 4, and compare the total"). End with: **"Come back and discuss any concerns or questions."**

Save the list at the end of `review.md` and set the job's status to `waiting for your check`.

**In the chat,** your message at the end of the review has two parts:

1. **A short wrap-up** (three to five lines): what was produced and where, what changed from the plan, what the reviewers found and fixed, and your confidence check in a sentence or two.
2. **The full "For you to check" list, exactly as saved,** with the quotes and the what, why, and how for each item. Don't shorten it in the chat; it's the user's part of the review.

Then wait for the user. When they respond, discuss or fix what they raise (rechecking any changed parts), then start step 5.
