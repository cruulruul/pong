# Issue tracker: GitHub

Issues and specs live at https://github.com/cruulruul/pong/issues.
Use the gh CLI, explicitly targeting cruulruul/pong.

Before creating issues, verify the target repository.
Use a temporary file and --body-file for multiline bodies.
Use full issue and pull request URLs in descriptions.

When a skill says "publish to the issue tracker", create a GitHub issue.
When it says "fetch the relevant ticket", read the issue and its comments.

Use native GitHub sub-issues for parent-child relationships and native
issue dependencies for blocking relationships. Check installed CLI
support before choosing commands. If unavailable, record full parent
and blocker URLs in the issue body and child links in the parent.

A ticket is unblocked when all blockers are closed.
Post a closing explanation as a comment before closing an issue.

## Pull requests as a triage surface

PRs as a request surface: no.

## Wayfinding

Keep the map in an issue labelled wayfinder:map.
Link child tickets to the map and label them wayfinder:<type>, where
type is research, prototype, grilling, or task.
Choose the first unassigned child in map order with no open blockers.
Claim it by assigning yourself. On resolution, comment with the result,
close the ticket, and add a result summary and link to the map.
