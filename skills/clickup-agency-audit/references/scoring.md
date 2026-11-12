# Scoring

Open task: any task not in a closed or done status. Scheduled task: an open task with a due date or a batch. Overdue: an open task whose due date is before today.

Round each share to a whole percent before you compare it with a threshold, and show the share in the report: 89.8% is 90% and passes.

| Check | Measure | Pass | Watch | Fix |
| --- | --- | --- | --- | --- |
| 1. Ownership | Open tasks with at least one assignee, as a share of open tasks | 95% or more | 80 to 94% | Under 80% |
| 2. Effort | Scheduled tasks with Points, or any effort estimate (time estimate, sprint points), as a share of scheduled tasks | 90% or more | 50 to 89% | Under 50% |
| 3. Weekly planning | Open tasks in This Week, Next Week or Later, or due between today and 14 days from now, as a share of open tasks that aren't Maybe or backlog. Overdue tasks and open tasks left in Previous don't count as planned | 80% or more | 50 to 79% | Under 50% |
| 4. Capacity | People planned past 12 points (or past the hours they gave you) this week | Nobody | Someone between 12 and 15 | Someone at 15 or more |
| 5. Slippage | Slippage rate (see notes), and the overdue count | Under 10% and fewer than 5 overdue | 10 to 30%, or 5 to 20 overdue | Over 30%, or more than 20 overdue |
| 6. Structure | Delivery space exists and holds client work; 7 statuses or fewer per list; no status used as a client name or person | All three | One misses | Two or more miss |

## Notes per check

**Ownership.** A task assigned to three people is owned by nobody. Count tasks with more than one assignee and report them beside the score, but don't fail the check for it alone.

**Effort.** Without effort numbers there's no capacity check. If effort is missing on most tasks, check 4 is Not measured, and say that's why.

**Weekly planning.** A due date three months out isn't a plan. A task with no date in a backlog list is fine; leave backlog and Maybe out of the count.

**Capacity.** With Points, add each person's open This Week points. With time estimates, add hours and compare to the hours they told you. With neither on most tasks, capacity is Not measured: a task count isn't a capacity score. Put the busiest person's task count in the row as a warning sign, and make adding effort the fix.

**Planned window.** "Between today and 14 days from now" includes both days.

**Slippage.** Use the first of these the workspace supports, name it in the report, and word the finding to match:

1. **The `slipped` tag is in use.** Open scheduled tasks tagged `slipped` or still sitting in Previous, as a share of open scheduled tasks. Report it as "X of Y open tasks have slipped at least once". The tag stays on a task after it's re-batched, so this is the share of open work that has missed a week, which is what the method's slippage rate tracks over time. Count separately the tagged tasks still in This Week or Previous with a past due date: those slipped and nobody re-batched them.
2. **BATCH without the tag, or no BATCH.** The last full Monday to Friday before today. Tasks due in that window that are still open, against all tasks due in it, closed ones included.
3. **Interview mode.** The share they gave for question 7.

In live mode, if the denominator is under 10 tasks, the rate is too small to score. Say so, score slippage on the overdue count alone, and give the rate as context only. Never score Fix from one or two tasks.

**People.** Capacity counts the team members you read or were told about. A task assigned to someone who isn't on the member list, or to a bot or shared account, still counts as owned for check 1. Report those tasks by count in the ownership row and leave them out of capacity.

**Structure.** A space named for client work counts as the delivery space: Delivery, Clients, Projects, Production, or what they tell you holds client projects. Statuses can be set per list; if you can only read the space's statuses, say the lists are assumed to inherit them.

**Structure.** Read space, folder and list names, and the statuses on the busiest delivery list. In interview mode, score it from questions 1 and 2.

## Ranking the fixes

Give up to three fixes, taken only from Fix and Watch checks. If only two qualify, give two; don't pad with a Pass. A fix can also come from a finding the checks surfaced on the way (a duplicate list, lists missing the fields), as long as it has a number behind it. Side findings rank after every Fix and Watch check, ordered by how many open tasks they touch, and fill the list up to three.

Rank the Fix and Watch checks by what they cost a delivery team, in this order when two tie:

1. Capacity (people burn out and client dates slip)
2. Slippage (the plan isn't believed)
3. Ownership (work falls between people)
4. Effort (capacity can't be measured)
5. Weekly planning
6. Structure

Fixing effort before capacity is often the right order in practice, because capacity can't be measured without it. When check 2 is Fix and check 4 is Not measured, put effort first and say why.
