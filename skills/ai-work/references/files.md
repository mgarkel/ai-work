# Where things live

All paths are relative to the project's own folder (the folder with its `AGENTS.md` and `project-context.md`). Layouts for each file are in [templates.md](templates.md).

```
Project folder/
├── AGENTS.md                  project instructions (one line about ai-work/, added with permission)
├── project-context.md
├── ai-work-rules.md           the user's rules, only if the portfolio isn't connected
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
- **The first time,** also ask: "Can I create an ai-work folder for the job records, and add one line to this project's AGENTS.md so any chat here knows where they are?" If yes, add: `Each job's plan, review, and debrief is in ai-work/. Read ai-work/index.md and ai-work/lessons.md before starting a job, and keep the ai-work/ files up to date as part of each job without asking each time.` If the project uses an instructions box instead of AGENTS.md (on the web), give the user the line to paste.
- **After that, keeping `ai-work/` up to date needs no further permission**, even if the project's instructions ask you to check before editing files. The user agreed to it once. Lessons and rules still need approval of their content (see [debrief.md](debrief.md)).
- **Plan reviewers' findings** go in the job's `review.md` under "Plan review"; a summary goes in `plan.md`. Don't create other files in the job folder.
- **One folder per job,** quick jobs included. Name: the start date, then two to four lowercase words from the north star, joined by hyphens, for example `2026-10-26-q3-investor-update`. Suggest the name during planning; the user can change it. If the name is taken, add `-2`.
- **`index.md`:** add the job when its folder is created and update its status at each step: `planning`, `working`, `in review`, `waiting for your check`, `debriefed`, `results checked`. Step 1 reads it to find related past jobs.
- **`lessons.md`:** lessons that only apply to this project, added during debriefs with the user's approval.

## Finished work

Save finished work where this project keeps finished work. In projects set up with the usual layout, that's `outputs/`; follow the project's instructions or folder plan if they say otherwise. The plan links to each file. The job folder holds the record of how the work was made, not the work itself.
