# Where things live

All paths are relative to the project's own folder (the folder with its `AGENTS.md` and `project-context.md`). Layouts for each file are in [templates.md](templates.md).

```
Project folder/
├── AGENTS.md                  project instructions (one line about ai-work/, added with permission)
├── project-context.md
├── ai-work-rules.md           the user's rules, only if the portfolio isn't connected
├── sources/                   documents saved as sources (or wherever this project keeps them)
├── outputs/                   finished work (or wherever this project keeps finished work)
└── ai-work/
    ├── index.md               one line per job
    ├── lessons.md             lessons for this project only
    └── YYYY-MM-DD-short-name/ one folder per job
        ├── plan.md            the plan, then the running log
        ├── review.md          reviewers' findings, fixes, rechecks, and "For you to check"
        └── debrief.md         the first debrief, then the results debrief
```

## The user's rules: `ai-work-rules.md`

How this skill should work for this user, in any project: rules for kinds of work, extra reviewers, changes to a step, preferences.

1. **Find the personal context portfolio.** The project's instructions usually say where it is (look for "portfolio" or "my context"). It's connected when you can read files in that folder.
2. **If the portfolio is connected,** the rules file is `ai-work-rules.md` in the portfolio folder. Create it from the template the first time a rule is added.
3. **If it isn't,** the rules file is `ai-work-rules.md` in the project's own folder. Same name, same layout.
4. **If both exist,** the portfolio's file is the main one. Offer once to move the project's rules into it, then delete the project copy only after the user agrees.

Lessons about the user that aren't rules for this skill (writing style, where authoritative numbers live) belong in the portfolio file they fit, such as `communication-style.md` or `tools-and-systems.md`, with the user's approval. If the portfolio isn't connected, put them in `ai-work-rules.md` under "About me".

## The `ai-work/` folder

- **Create it** the first time a job is planned in this project, with `index.md` and `lessons.md` from the templates.
- **The first time,** explain why before asking, in words like these: "Since this is the first time you're using me in this project, may I create an `ai-work` folder? I'll keep a record of every job in it (the plan, the review, and what we learned), so you have a record of everything that was done and the next job starts from what we learned. I'd also add one line to this project's AGENTS.md so any chat here knows where those records are. I'll only ask this once." If yes, add: `ai-work/ holds the records of jobs done with the ai-work plugin. Read ai-work/lessons.md before starting work in this project. When the user is running a job with ai-work, keep its ai-work/ files up to date without asking each time; otherwise don't create or change them.` If the project uses an instructions box instead of AGENTS.md (on the web), give the user the line to paste.
- **After that, keeping `ai-work/` up to date needs no further permission**, even if the project's instructions ask you to check before editing files. The user agreed to it once. Lessons and rules still need approval of their content (see [debrief.md](debrief.md)).
- **Plan reviewers' findings** go in the job's `review.md` under "Plan review"; a summary goes in `plan.md`. Don't create other files in the job folder.
- **One folder per job,** quick jobs included. Name: the start date, then two to four lowercase words from the north star, joined by hyphens, for example `2026-10-26-q3-investor-update`. Suggest the name during planning; the user can change it. If the name is taken, add `-2`.
- **`index.md`:** add the job when its folder is created and update its status at each step: `planning`, `working`, `in review`, `waiting for your check`, `debriefed`, `results checked`. Step 1 reads it to find related past jobs.
- **`lessons.md`:** lessons that only apply to this project, added during debriefs with the user's approval.

## Sources

Documents you save while researching (a report, a PDF, a dataset) go where the project keeps material from others: `sources/` in the usual layout. Record each one in the plan's context with where it came from and the date. Saving a document is fine; opening or running it as a program never is.

## Finished work

Save finished work where this project keeps finished work. In projects set up with the usual layout, that's `outputs/`; follow the project's instructions or folder plan if they say otherwise. The plan links to each file. The job folder holds the record of how the work was made, not the work itself.
