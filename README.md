# UpSys Workspace Audit for Claude

Audit how an agency runs client work in ClickUp. Claude scores 6 checks, shows the number behind each score, and gives the fix for the 3 that cost the team most:

1. Ownership: every open task has one owner.
2. Effort: open tasks carry an effort estimate.
3. Weekly planning: open work sits in a week, not just a far-off due date.
4. Capacity: nobody is planned past their weekly limit.
5. Slippage: how much of last week's plan is still open, and what's overdue.
6. Structure: spaces, lists and statuses match how client work moves.

If ClickUp is connected in Claude, the audit reads your spaces, lists and tasks and works from real counts. If it isn't, Claude asks you 8 questions about your team and scores the answers. It never changes anything in your workspace.

The audit is built on BATCH planning, the method UpSys installs for agencies of 5 to 50 people: one-week batches, effort points from 1 to 3, a cap of 15 points per person per week, and a Friday review of what slipped.

## Install

```
/plugin marketplace add heyramzi/upsys-workspace-audit
/plugin install upsys-workspace-audit@upsys-workspace-audit
```

## Try

- "Audit my agency's ClickUp workspace."
- "My team keeps missing deadlines in ClickUp. What's wrong?"
- "Is anyone on the team overbooked this week?"
- "How should an agency set up ClickUp for client delivery?"

## Help

[upsys-consulting.com/en/clickup-audit](https://www.upsys-consulting.com/en/clickup-audit) or admin@upsys-consulting.com. Privacy: [upsys-consulting.com/en/privacy](https://www.upsys-consulting.com/en/privacy).

## Source

This folder lives at `tools/chatgpt-plugin/claude-plugin/` in the UpSys monorepo. `skills/clickup-agency-audit` there is a link to the ChatGPT plugin's skill, so both plugins ship the same text. Publish it with the link followed:

```bash
rsync -aL --delete --exclude .git tools/chatgpt-plugin/claude-plugin/ <clone of heyramzi/upsys-workspace-audit>/
```
