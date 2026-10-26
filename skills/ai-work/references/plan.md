# Step 2: Plan

Planning is most of the work. Go top-down: agree where you're going first, then the decisions that get you there, then talk each one through. Be a thinking partner, not a form: suggest, challenge assumptions, and offer alternatives, but leave the decisions to the user.

Before you start, suggest the job's size (quick, standard, or important; see [SKILL.md](../SKILL.md)) in one line with your reason, and the job folder's name. The user can change either. Create the job folder and add it to `ai-work/index.md` with status `planning` (see [files.md](files.md)).

For a **quick** job, do A, a short C if anything is unclear, and E with only the north star, steps, and checklist, then F.

## How to ask (all of this step)

- **One topic at a time, in rounds.** A round is a few related questions that can be decided together. Number them so the user can answer "1 yes, 2 no, 3 …".
- **Every question comes with your recommended answer**, drawn from the context, and worded so "yes" accepts it. Say briefly why.
- **Offer options when they help.** Two to four realistic options, with the tradeoff of each. If you'd be straining to fill the options, ask an open question instead, and make it specific enough to answer ("What's the most concrete thing that's gone wrong with this before?", not "Any thoughts?").
- **Keep a running list of decisions.** Don't reopen a settled decision unless a new fact changes it, and say so when that happens. A new question that comes up goes onto the list rather than expanding the current topic.
- **When the user can't judge a topic.** If they say they don't know the area, or answer "I don't know" or "you decide" twice in a row on questions that need judgment, offer to lay out the choices first: the decisions in that area, the realistic options for each, and what you'd pick. Then they choose rather than guess. If they decline, use your recommended answers and record them as assumptions.
- **How many rounds.** No fixed number. It depends on the size of the job and how much the context already settles. Stop when the remaining questions wouldn't change the plan. Don't ask what the files already answer; state it as settled and move on.

## A. North star

Agree these before anything else:

- **Objectives:** what this job must achieve, and for whom.
- **Outcomes:** what exists at the end (files, a sent message, a decision made, a meeting held).
- **Great versus acceptable:** what a great result looks like compared with one that's merely acceptable. This is the definition of done. Make it measurable where you can, with the current baseline and the target, and where the number comes from.

Draft them from the context and ask the user to confirm or change them.

## B. Approaches and the decisions

1. **Test the job itself,** briefly, and raise only the gaps you actually find:
   - Is this the real problem, or a symptom of another one?
   - What's the smallest version that still delivers the outcomes?
   - What happens today without it, and what does that cost?
   - Who exactly is it for, and what changes for them?
2. **Approaches.** If more than one way could work, describe two or three, including one that isn't obvious (do the opposite of the usual, drop a constraint, or borrow how another field does it). For each: what it is, pros and cons, and the main risk. **Show all of them before recommending one,** then recommend the one that meets the north star with the least extra work. If one is clearly best, just say so and why.
3. **The list.** Write out the decisions and discussion points needed to reach the north star, plus the open questions, constraints, people involved and what each cares about, and the tensions and gaps you see. Show the list; this is the agenda for C.

## C. Talk it through

Work through the list from B, one topic at a time, using the rules above. For standard and important jobs, make sure these are covered somewhere (most may already be settled by the context):

- Who it's for and what they need from it.
- The constraints: time, budget, politics, what can't change.
- **Stop points:** where the work must stop for the user's approval, for example before anything is sent or shared.
- What's been tried before, and how this kind of work usually goes wrong.
- **"What would you be most embarrassed to get wrong?"** Ask this one directly. The answers become the job's checklist, which the review checks against.
- What to check later, and when: how and when you'll know whether the work achieved its goal (a reply, a decision, a meeting's result). This sets up the results debrief.

## D. Pre-mortem and plan reviewers

**Pre-mortem.** "Imagine it's done and it went badly. Why?" Suggest the top risks, the most likely and the most damaging, each with how to prevent it. The user adds, removes, or changes them, and you discuss how to prevent each one.

**Plan reviewers** (standard and important jobs). Draft the plan first (E), save it, then have five fresh reviewers critique it before any work starts. Use the briefs in [reviewer-briefs.md](reviewer-briefs.md), section "Plan reviewers": devil's advocate, scope guardian, consistency check, fact check, and audience lens.

- Start each reviewer as a separate helper (a sub-agent) **without this conversation's history**, so it judges the plan on its own. In ChatGPT, helpers get the conversation by default, so ask for a clean one that doesn't. In Claude, helpers start without it. Give each one only its brief, the plan file, and the sources it needs.
- If you can't start helpers, do each review yourself as a clearly separate pass, and tell the user it isn't independent.
- Combine their findings: merge duplicates and drop anything you can disprove from the plan or sources. Save the full findings in the job's `review.md` under "Plan review".
- **Sort what's left into two groups:**
  - **Obvious fixes:** one right answer that doesn't change anything the user decided (a missing step, an unclear sentence, a wrong number, a gap such as "explain how to use this for their own business"). **Make these in `plan.md` yourself.**
  - **Needs the user's decision:** anything that would change the goal, the scope, the topic, a decision the user made, or that depends on their preference. **Don't change these; ask.** For each, give the realistic options and your recommendation.
- In `plan.md`'s "Plan review" section, list what you added and what was left for the user to decide.
- Then go to F. The findings and the approval question go in one message.

## E. Write the plan

Save `plan.md` in the job folder using the layout in [templates.md](templates.md). It must be complete enough that a different chat could do the work from it alone:

- The north star (objectives, outcomes, great versus acceptable).
- The context, with sources: what step 1 found that matters.
- Decisions: each with the alternative it was chosen over, why, and who decided (the user chose it, or the user agreed to your suggestion).
- Assumptions and open questions, labeled as such.
- Steps, each linked to the outcome it serves, with check-ins at milestones and the stop points.
- Risks, how each is prevented, and what the plan reviewers found and what changed.
- The job's checklist.
- The rules for this kind of work (from [kinds-of-work.md](kinds-of-work.md) and the user's rules).
- How you'll check your own work as you go (see [work.md](work.md)), and how the work will be reviewed.
- What to check later, and when.
- An empty running log, filled in during the work.

## F. Approval

Make it unmistakable that planning is finished and this is the approval point. Open with: **"The plan is ready for your approval."** Then give a short "here's what we agreed": the north star, the approach, the main decisions, the stop points, the checklist, and what happens next (the work, then the review, then your check), in a few lines, with the plan file's path.

For standard and important jobs, then report the plan review in two clearly separate parts:

- **"The reviewers suggested [N] improvements. I've already added these to the plan:"** one line each.
- **"⚠ Needs your decision before I start:"** numbered, each with the options and your recommendation. Make it impossible to miss: put it last, just before the question, and say that the work can't start until these are answered. If nothing needs a decision, say "Nothing needs your decision."

Then ask the user to:

1. approve it,
2. change something,
3. add context you missed, or
4. make the job bigger or smaller.

If anything needs a decision, the question asks for those answers first: "Reply with your choice for each decision above, and whether you approve the plan." Don't treat a plain "approved" as answering them; if they reply without choosing, use your recommendation only after confirming it in one line.

End your message with that question. Don't add anything after it, and don't explain why you're asking.

Wait for their approval before doing the work. When they approve, update the index to `working` and go straight into step 3.
