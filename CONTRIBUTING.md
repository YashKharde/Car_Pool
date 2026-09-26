# Working one step at a time

## Before the change

Post a short explanation in the conversation:

1. Step and outcome: what will work or become clear.
2. Impact: why this matters to a rider or to reliability.
3. Technical changes: backend, frontend, data and infrastructure involved.
4. Checks: how the result will be verified.

## During the change

Implement one coherent step, update the related contracts and comments, and run checks appropriate to its impact. Explain meaningful decisions without a stream of low-level command details.

## After the change

Update the step record, progress tracker and changelog. State what changed, what passed, what was not tested and what comes next. Commit all related backend/frontend/documentation changes together for the step; the initial step has documentation only.

Commit format: `type(Sxx): concrete result`. Reference the commit in the chat after it exists. A step record cannot include the hash of the commit that contains itself; record its commit subject and put the resolved hash in the chat or a later log entry.

Push normal commits to the project remote when authentication is available. Never force-push, rewrite history, commit secrets or discard someone else's work without specific authorization.

## Plan updates

The current live record is docs/progress.md. Detailed evidence belongs in docs/steps/. The roadmap PDF is a versioned snapshot, not proof that a feature exists. Preserve earlier snapshots and carry saved PDF notes into later versions.

No application version is fixed until compatibility is checked during S02. No cloud resource is provisioned in the documentation step.
