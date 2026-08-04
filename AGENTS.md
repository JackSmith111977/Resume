# Repository-wide Agent Rules

> Scope: this repository and all subdirectories.  
> These rules are mandatory for every Agent working in this repository.

## 1. Rule precedence

When instructions conflict, use this order:

```text
User's current explicit instruction
> this root AGENTS.md
> the nearest descendant AGENTS.md
> current dated schedule and progress ledger
> execution and strategy documents
> historical notes
```

A descendant `AGENTS.md` may add stricter rules, but must not weaken or bypass the mandatory guardrails in this root file.

## 2. Mandatory context for autumn-recruitment work

Before working anywhere under `autumn-recruitment/`, the Agent must read and follow:

1. [`autumn-recruitment/AGENTS.md`](./autumn-recruitment/AGENTS.md);
2. [`autumn-recruitment/execution/zero-baseline-learning-policy.md`](./autumn-recruitment/execution/zero-baseline-learning-policy.md);
3. [`autumn-recruitment/execution/time-budget-and-task-guardrails.md`](./autumn-recruitment/execution/time-budget-and-task-guardrails.md);
4. the current dated schedule in `autumn-recruitment/schedule/`;
5. [`autumn-recruitment/schedule/progress-ledger.md`](./autumn-recruitment/schedule/progress-ledger.md);
6. the current daily log, if one exists.

The Agent must not operate only from conversation momentum or a single specialist file.

## 3. Non-negotiable time and scheduling guardrails

For autumn-recruitment tasks, the Agent MUST:

1. Determine or conservatively infer the user's available time before starting a daily task.
2. Reserve the daily budget approximately as:
   - main task: at most 60%;
   - a different pipeline's minimum task: at least 25%;
   - retest, progress update, and archive: at least 15%.
3. Give every task a maximum duration or hard stop, a minimum deliverable, a completion condition, a stopping condition, and an explicit `do not do` scope.
4. Stop a single domain at the earlier of:
   - 60% of the day's available time;
   - one L task, normally 45–60 minutes;
   - the task's declared stopping condition.
5. Run a scheduling checkpoint after every completed or stopped task by rereading the current schedule and progress ledger.
6. Never start a future same-domain task while a current-day cross-pipeline task remains unfinished, unless the user explicitly overrides this after seeing the trade-off.
7. Preserve archive time. When a task overruns, stop expansion, save a reviewable intermediate state, downgrade remaining work to S, and return to the global schedule.
8. Never continue into another problem, chapter, framework, or project slice merely because the current teaching or implementation has momentum.
9. Update the daily log and progress ledger with planned versus actual scope, overruns, deleted or downgraded tasks, and the next first action.

If exact elapsed time is unavailable, the Agent must use task boundaries as the enforcement mechanism: after one planned main task, it may not open another same-domain task before the scheduling checkpoint.

## 4. Zero-baseline evidence rule

Unless the user has produced current, reproducible, independent evidence, treat knowledge and skills as `TODO / needs learning`.

The following are not sufficient proof of mastery:

- saying a term or framework name;
- prior exposure or historical project participation;
- following an AI explanation;
- AI-generated code or documents;
- completing a task with material prompting.

Do not demand that the user prove existing ability when the current task is to learn from zero. Use job descriptions to derive learning modules, then create evidence through teaching, implementation, testing, and delayed retesting.

## 5. Enforcement behavior

An Agent MUST NOT silently violate these guardrails.

When a requested or inferred next action would exceed the budget, advance a future same-domain task, or displace another current-day pipeline, the Agent must do one of the following:

- stop at the current reviewable checkpoint;
- downgrade the next task;
- record the displaced task and ask for an explicit override when necessary;
- choose the smaller scope by default.

Only the user's current explicit instruction may temporarily override a mandatory scheduling guardrail. The override applies only to the stated task or session and must be recorded in the daily log.

## 6. Required end-of-task check

Before declaring a task complete or starting another task, report or record:

```text
Planned budget:
Actual scope:
Hard stop reached:
Current deliverable:
Remaining current-day pipelines:
Next task source:
Future same-domain task avoided:
Archive and ledger updated:
```

Failure to run this check means the task is not operationally complete.