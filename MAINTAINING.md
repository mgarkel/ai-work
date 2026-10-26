# Maintaining ai-work

## Releasing a new version

1. **Raise the version** in `.claude-plugin/plugin.json` and in the "This version" line of `skills/ai-work/SKILL.md`. Installed copies only update when the version changes. Don't set a version in `marketplace.json`; the one in `plugin.json` wins.
2. **Write "What's new"** in `CHANGELOG.md`, in plain words.
3. **Sync discernment-nudge:** compare `skills/discernment-nudge/` with the latest in [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/discernment-nudge). If it changed, copy it unchanged (SKILL.md and LICENSE.txt) and update the commit in `CREDITS.md` and `CHANGELOG.md`.
4. **Run the release check** below, in ChatGPT and in Claude.
5. Commit, tag (`v0.2.0`), and push.

## Release check

Use a test project (not a real client's), with an `AGENTS.md`, a `project-context.md`, and a portfolio folder containing `ai-work-rules.md` with one rule.

1. **The loop:** run one standard job end to end (the October 24 test task works: a one-page plan for a 45-minute AI workshop for small-business owners). Check that the plan, review, and debrief files are written in `ai-work/`, reviewers are fresh, the user's rule is applied, and "For you to check" appears.
2. **Time and pauses:** note how long it took and how many times it stopped for the user; compare with earlier runs.
3. **Updates don't touch user files:** install the previous version, create a job and a rule, update to the new version, and check that `ai-work/`, `lessons.md`, and `ai-work-rules.md` are unchanged.
4. **The update arrives:** an installed copy shows the new version after updating.

## Feedback

Suggestions marked "share it with your coach" in learners' debriefs are candidates for the next version. Add them to the plugin only if they'd help anyone, not just one person.
