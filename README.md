# ai-work

Plan, do, review, and debrief real work with AI, step by step, in ChatGPT or Claude.

Most AI work goes wrong in predictable ways: the wrong goal, hidden assumptions, facts nobody checked. Professionals have answered these for decades with briefs, pre-mortems, checklists, independent review, and after-action reviews. This plugin packages that method so you don't have to remember every step yourself.

## What it does

| Step | What happens |
| --- | --- |
| 1. Gather context | Reads your project, your rules, past jobs, and relevant email, calendar, and files, then summarizes what matters |
| 2. Plan | Agrees the north star with you, lays out approaches and decisions, talks them through, imagines what could go wrong, has five fresh reviewers check the plan, and waits for your approval |
| 3. Work | Does the work, citing a source for every fact and checking itself as it goes, with check-ins at milestones |
| 4. Review, then you | Fresh reviewers check the work; then you get a short "For you to check" list |
| 5. Debrief | Saves what it learned, after the work and again once the result is in |

Each job's plan, review, and debrief are saved in your project's `ai-work/` folder. Finished work goes where your project keeps finished work.

## Use it

In a chat inside one of your projects:

- **"Plan [the job]"** starts a new job.
- **"Review [the job]"** reviews work that has a plan.
- **"Debrief [the job]"** runs a debrief.
- **"Add a rule: …"** customizes it. **"Show my rules"** lists your rules.
- **"Where were we?"** picks up a job where it left off.

## Make it yours

Your rules live in `ai-work-rules.md`: in your personal context portfolio if it's connected to the project, otherwise in the project's folder. Your rules override the plugin's defaults, and a project's `ai-work/lessons.md` overrides your rules for that project. Updates to the plugin never touch these files.

## Install

1. Before installing any plugin, check: who made it, what it does, what it can reach, anything surprising, and whether it's maintained. You can ask your AI to read this repository and answer those questions.
2. Add this repository as a plugin source in your app and install **ai-work**.
3. Turn on auto-update for it if your app offers that.

It includes a copy of Anthropic's [discernment-nudge](https://github.com/anthropics/skills/tree/main/skills/discernment-nudge) skill, so you don't need to install that separately.

## What it can reach

It reads your project's files, your personal context portfolio, and, if connected, your email, calendar, and cloud files, read-only. It writes only in your project's folder and your portfolio's `ai-work-rules.md`. It never sends, publishes, deletes, or writes to connected apps without your approval, and never installs software unless an approved plan calls for it. It may save documents it finds (a report, a PDF) to your project's sources folder, noting where each came from. To check its own work it may use what's already on your computer (counting words, adding up numbers, previewing a page), read-only, and it tells you what it checked.

See [CHANGELOG.md](CHANGELOG.md) for what's new and [CREDITS.md](CREDITS.md) for where the ideas come from.

## License

MIT (see [LICENSE](LICENSE)). The included discernment-nudge skill is Anthropic's, under the Apache License 2.0 (see `skills/discernment-nudge/LICENSE.txt`).
