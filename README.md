# undo-push-experiment

Testing how can I revert an ooopps-push into a develop branch without breaking anything

### This branch approach:

- Forked branch from the errored head.
- Pushed to remote (so that commits are registered)
- Revert last push from the last OK commit and push the correct branch status without the ooops file.
- When doing this gives a rejection error because this branch is behind remote head (fast-forward error). To solve make again git pull and manual fix the conflicts. 
