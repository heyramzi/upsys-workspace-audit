# Report layout

Keep it to one screen before the fixes. Plain words, no score out of 100: six named checks are easier to act on than one number.

```markdown
## ClickUp audit: <workspace or agency name>

<One sentence: the single biggest problem and what it costs. Example: "Two of your five designers are booked past capacity this week, and a third of last week's plan is still open.">

<Live: "Read from the Delivery space on <date>: 212 open tasks, 9 people." Interview: "Scored from your answers on <date>.">

| Check | Score | What we found |
| --- | --- | --- |
| Ownership | Pass / Watch / Fix / Not measured | <number and source> |
| Effort | | |
| Weekly planning | | |
| Capacity | | |
| Slippage | | |
| Structure | | |

### Fix first

**1. <Fix name>** (<who does it>, <how long>)
<Why it's first, in one sentence with the number.>
1. <Click path or setting in ClickUp>
2. <...>
Done when: <what they'll see in ClickUp when it's fixed>

**2. ...**

**3. ...**

### Every Friday, 20 minutes
<The five-step Friday review from method.md, adjusted to what they use. If they don't use BATCH, say which field or filter plays its part.>

---
Scored against BATCH planning by UpSys.
```

## Fix recipes

Use these when they match. Adjust names to the workspace. Without BATCH, the due date does the batch's job: "filter This Week" becomes "filter due this Monday to Friday", and re-batching means picking a new Friday due date on purpose.

**Add effort points.** Settings, Custom Fields, new Dropdown at workspace level named Points with options 1, 2 and 3. Add it to the delivery lists. Put the point guide (1 quick, 2 standard, 3 large) in the field description. The person who plans the week sets points when a task is created. 15 minutes, then a minute per task.

**Add weekly batches.** Workspace-level Dropdown named BATCH with Previous, This Week, Next Week, Later and Maybe. Every task in a batch gets Monday start and Friday due, date only. 15 minutes to set up, 30 minutes the first Friday to batch the open work.

**Set the capacity cap.** In the delivery space, add a Workload view. Group by assignee, measure by the Points field, set capacity to 15 for each person. Plan to 12. 10 minutes.

**Find the owner gaps.** In the delivery space, filter Assignee is empty, status is not closed. Assign each task to one person; when it needs two, split it. The team lead, 30 minutes.

**Start the slipped tag.** Create the tag `slipped` in the delivery space. On Friday, filter This Week to open tasks and tag them. Re-batch each one by hand. 5 minutes a week once it's running.

**Cut statuses.** Keep five for client work, for example To Do, In Progress, Internal Review, Client Review, Done. A status that names a client, a person or a type of work becomes a field or a list instead. Merge the old statuses in the list's status settings, which moves the tasks with them. 30 minutes per list.

**Split the spaces.** Sales for leads and deals, Delivery for client work, System for internal work and templates. In Delivery, one client project is one task with its stages as subtasks. 1 to 2 hours, mostly moving lists.
