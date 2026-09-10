# Modeling Decisions

## Scope

The model starts when an application is received and ends when the license is issued or the case is otherwise closed. Activities outside that boundary are referenced only when they affect the process state.

## Abstraction level

The detailed model captures the operational activities, responsible roles and alternative paths required by the software flow. The repository overview groups these details into major stages so the complete process remains easy to follow.

## Gateways

Exclusive gateways represent decisions with one selected outcome, such as complete or incomplete. Parallel gateways represent independent reviews that can proceed concurrently and must be reconciled before the process advances.

## Rework

Correction is modeled as an explicit loop. This keeps the normal path readable and shows where reassessment occurs.

## End states

Issued, rejected and withdrawn are separate end states. They are not treated as interchangeable versions of completion.

## Assumptions

- A valid application must pass an initial completeness check.
- Some technical reviews can be performed in parallel.
- Inspection may create a correction and reinspection loop.
- Final authorization occurs after required reviews are complete.

These assumptions summarize the main process logic shown in the portfolio overview. The detailed model contains the activity-level rules used during analysis and implementation.
