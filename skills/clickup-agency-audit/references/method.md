# BATCH planning, the method behind the audit

The method rests on two fields, one tag and one number. It's built for agencies with a delivery team, past solo scale, before a dedicated ops hire. The job it does: a clear read on the team's capacity every week, without hiring a project manager to keep it up.

## The two fields

**BATCH**, a dropdown with five options. Every scheduled task sits in exactly one week.

| Batch | Dates |
| --- | --- |
| Previous | Done or past work, left as it is |
| This Week | Start Monday, due Friday of this week |
| Next Week | Monday and Friday of next week |
| Later | Monday and Friday two weeks out |
| Maybe | No dates |

Every task in a batch shares one start date and one due date, date only, no time. The due date is the source of truth and the batch follows from it.

**Points**, a dropdown of 1, 2 or 3. Points measure effort, not hours.

- 1: a quick task, a review, a plan, a short edit.
- 2: a standard deliverable, a demo, a testimonial.
- 3: a large or multi-part deliverable, a keynote, a full edit.

Both fields are created at workspace level so every space shares the same field.

## The number: 15 points per person per week

15 is the line a person must never reach. Plan to 80% of it, which is 12, because a week planned at 100% goes red the first time anything moves. Fill This Week and Next Week to 12 each, then overflow into Later.

When someone is over:

1. Client work wins. Rank started work first, then client-facing work (a client date, or waiting on review), then other client work, internal work last.
2. Before pushing a client task out a week, check whether a teammate under 12 can take it. Reassigning beats delaying.
3. Work already in progress keeps its dates. Move the lowest-ranked, largest not-started tasks down a batch first.

In ClickUp the cap lives on the Workload view: group by assignee, measure by the Points field, capacity 15. It's a setting in the view, not something the API can set.

## The tag: slipped

A task that was planned into a week and isn't done on Friday gets the `slipped` tag. Slipped work never rolls forward by itself. On Friday a person looks at each open task and asks one question: is it done? Part done counts as not done.

A batch is the plan, so a slipped task is late by design. Overdue and slipped are one signal, not two.

The number that matters is the **slippage rate**: the share of the week's batch still open on Friday. One slipped task is a task. 30% slipping week after week is the system.

## The Friday review, 20 minutes

1. Filter This Week to open tasks. Tag each one `slipped`.
2. Re-batch each slipped task on purpose: back into Next Week, or down to Later, or out to Maybe.
3. Move Next Week to This Week and set the dates.
4. Open the Workload view and bring everyone to 12 points or under for both weeks.
5. Write down the slippage rate. Watch the trend, not one week.

## Structure

Three spaces cover a delivery agency: **Sales** (leads and deals), **Delivery** (client work) and **System** (internal ops, SOPs, templates). Marketing and Admin are extra spaces an agency adds when it gets to them.

In Delivery, one client project the agency sells is one task. Its stages are subtasks, and BATCH and Points sit on the stages, because a stage is what fits in a week.

Five statuses are enough for client work. More than seven usually means statuses are doing a field's job (a client name, a type of work, a person).
