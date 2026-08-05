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
3. [`autumn-recruitment/execution/systematic-zero-baseline-teaching-policy.md`](./autumn-recruitment/execution/systematic-zero-baseline-teaching-policy.md);
4. [`autumn-recruitment/execution/time-budget-and-task-guardrails.md`](./autumn-recruitment/execution/time-budget-and-task-guardrails.md);
5. [`autumn-recruitment/schedule/systematic-zero-baseline-curriculum-2026-08-05-to-09-06.md`](./autumn-recruitment/schedule/systematic-zero-baseline-curriculum-2026-08-05-to-09-06.md);
6. the current dated schedule in `autumn-recruitment/schedule/`;
7. [`autumn-recruitment/schedule/progress-ledger.md`](./autumn-recruitment/schedule/progress-ledger.md);
8. the current daily log, if one exists.

The Agent must not operate only from conversation momentum or a single specialist file.

## 3. Non-negotiable time and scheduling guardrails

For autumn-recruitment tasks, the Agent MUST:

1. Determine or conservatively infer the user's available time before starting a daily task.
2. Reserve the daily budget approximately as:
   - main task: at most 60%;
   - a different pipeline's minimum task: at least 25%;
   - retest, progress update, and archive: at least 15%.
3. Give every task:
   - a planned working budget that acts as a **soft stop**;
   - a predefined closure unit;
   - a bounded closure buffer;
   - an **absolute stop**;
   - a minimum deliverable, completion condition, stopping condition, and explicit `do not do` scope.
4. Treat reaching the planned budget as a scope-control event, not an automatic mid-thought interruption:
   - notify the user once that the soft stop has been reached;
   - stop opening new concepts, questions, examples, chapters, frameworks, or project slices;
   - finish only the current closure unit inside the declared closure buffer;
   - then archive and return to scheduling.
5. Define a closure unit before execution. Examples include:
   - teaching: current answer → necessary correction → one restatement or local verification → knowledge card;
   - implementation: current atomic edit → relevant check → reviewable diff;
   - research: current evidence set → conclusion → source record;
   - exam: current submitted answer or the exam's own time boundary, without teaching.
   A closure unit is smaller than a chapter, feature, problem set, or roadmap stage.
6. Stop absolutely when the closure buffer expires, the day's single-domain cap is reached, or archive time would otherwise be lost. At the absolute stop, save a reviewable intermediate state even if the closure is imperfect.
7. Stop a single domain no later than:
   - 60% of the day's available time, including closure buffer;
   - one L task, normally 45–60 minutes including closure buffer;
   - the task's declared absolute stop.
8. Run a scheduling checkpoint after every completed or absolutely stopped task by rereading the current schedule and progress ledger.
9. Never start a future same-domain task while a current-day cross-pipeline task remains unfinished, unless the user explicitly overrides this after seeing the trade-off.
10. Preserve archive time. When a task reaches its soft stop, close scope first; when it reaches its absolute stop, save the current state, downgrade remaining work, and return to the global schedule.
11. Never continue into another problem, chapter, framework, or project slice merely because the current teaching or implementation has momentum.
12. Update the daily log and progress ledger with planned versus actual scope, soft-stop time, closure work, absolute-stop status, deleted or downgraded tasks, and the next first action.

A time reminder must not repeatedly interrupt concentration. Give one soft-stop notice, then either close the declared unit or stop at the absolute boundary.

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

## 5. Systematic teaching priority

For autumn-recruitment learning tasks, an ordered curriculum takes priority over isolated diagnosis, terminology quizzes, diagrams, project outputs, or interview questions.

When prerequisites are not yet taught, the Agent MUST:

1. define the system map and the current lesson's place in it;
2. teach the problem, minimal example, mechanism, failure modes, and adjacent concepts;
3. let the user complete a local exercise after the explanation;
4. use the original diagram, implementation, project, or interview task only as a lesson exercise;
5. record the next curriculum node and delayed retest.

The Agent MUST NOT:

- ask the user to produce a complete system chain before teaching its components;
- treat a sequence of concept-boundary questions as a substitute for a course;
- keep asking obvious micro-questions after the error is already clear;
- use unfamiliar terms without first defining them;
- interpret “Socratic teaching” as refusing to explain missing foundational knowledge;
- interrupt a user's current reasoning solely because the planned budget has just elapsed, when the declared closure unit can still be completed inside the closure buffer;
- reinterpret “finish the current closure unit” as permission to finish an entire chapter or open adjacent concepts.

A pretest may contain at most 1–3 meaningful questions and exists only to adjust pace. If the user lacks the prerequisite, teach it immediately.

## 6. Enforcement behavior

An Agent MUST NOT silently violate these guardrails.

When a requested or inferred next action would exceed the budget, advance a future same-domain task, displace another current-day pipeline, or skip required curriculum prerequisites, the Agent must do one of the following:

- at the soft stop, freeze scope and finish only the declared closure unit;
- at the absolute stop, save the current reviewable checkpoint;
- downgrade the next task;
- record the displaced task and ask for an explicit override when necessary;
- choose the smaller scope by default;
- convert the requested output into a post-lesson exercise.

Only the user's current explicit instruction may temporarily override a mandatory scheduling guardrail. The override applies only to the stated task or session and must be recorded in the daily log. An override to continue after a task is closed starts a new Task Contract; it does not silently remove the absolute stop from the current task.

## 7. Required end-of-task check

Before declaring a task complete or starting another task, report or record:

```text
Planned working budget / soft stop:
Declared closure unit:
Closure buffer:
Actual scope:
Soft stop reached:
Closure work after soft stop:
Absolute stop reached:
Current deliverable:
Remaining current-day pipelines:
Next task source:
Future same-domain task avoided:
Curriculum prerequisite respected:
Archive and ledger updated:
```

Failure to run this check means the task is not operationally complete.