# Idempotent hit scenario

The automation merge action is meant to sit in `queued` on the approval gate while this
pull request is merged by someone else, so the drain reaches the idempotent branch.
