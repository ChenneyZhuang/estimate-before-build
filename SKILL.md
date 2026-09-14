---
name: estimate-before-build
description: |
  Scope before building: turn the request into a bounded task list with
  assumptions named, estimate each task in size bands (S/M/L/XL) with the
  uncertainty driver named for M and above, present the scope-vs-budget
  options (full scope / reduced scope / timeboxed spike) instead of picking
  one silently, and record the estimate so the finish-line comparison
  calibrates the next one. Use when the user asks for a feature, script,
  migration, or any build whose size is not yet known, when "quick change"
  requests arrive with no scope discussion, or when a previous task ran
  far over its imagined size.
  触发词：先估后做 / 工作量评估 / 范围确认 / estimate。
license: MIT
metadata:
  version: "0.1.0"
---

# Estimate Before Build: make the scope decision explicit

The expensive failure is not a wrong estimate; it is the unmade decision —
building starts, the true size surfaces mid-way, and stopping then reads as
failure. An estimate before the first edit turns the slide into a choice.

## Rules

1. **Bound the request into tasks.** The task list is the scope: each task
   is a checkable unit of work, and what is out of scope is stated. A scope
   nobody wrote down is not a scope.
2. **Estimate in bands, not hours.** S = one sitting, no unknowns; M = a few
   sittings or one unknown; L = multiple unknowns or cross-system; XL =
   needs its own plan first. Hours invite false precision; bands
   communicate shape.
3. **Name the uncertainty driver.** Every M-and-above estimate names what
   makes it uncertain — the driver is where the risk lives and where a
   spike belongs.
4. **Surface the choice; do not pick silently.** Full scope at the
   estimate, a reduced scope that fits the budget, or a timeboxed spike on
   the unknown first — the user decides with the options on the table.
5. **Record and reconcile.** The estimate lands in the session notes (or
   issue) with a date; at the finish line, estimate meets actual per task.
   The comparison is the only mechanism that calibrates the next estimate.
6. **Re-estimate on discovery.** New information that moves a task a full
   band triggers a re-estimate and a re-surface of the choice —
   mid-build scope growth without a decision is the failure mode itself.

## Steps

1. **Decompose.** Break the request into a task list with out-of-scope
   stated and assumptions named. Done when: every task is checkable and
   the exclusions are explicit.
2. **Band each task.** Assign S/M/L/XL with the uncertainty driver named
   for M and above. Done when: no task above S lacks its driver.
3. **Present options.** Full scope total, a reduced-scope alternative, and
   the spike option where drivers dominate. Done when: the user received
   the choice, not a started build.
4. **Record.** Save the estimate with its date and the chosen option.
   Done when: the record exists where the finish line will find it.
5. **Reconcile at the finish.** Compare estimate vs actual per task; write
   one calibration lesson into the next estimate's context.
   Done when: the comparison exists, whatever it says.

## Done when

The work started with a bounded task list and banded estimates, the
scope-vs-budget decision was made by the user with options on the table,
the estimate is recorded, and the finish-line comparison exists to teach
the next one.
