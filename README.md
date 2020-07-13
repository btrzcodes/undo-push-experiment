# undo-push-experiment

Testing how can I revert an ooopps-push into a develop branch without breaking anything

### This branch approach:

- Forked branch from the errored head.
- Pushed to remote (so that commits are registered)
- Revert last push from the last OK commit and push the correct branch status without the ooops file.
- When doing this gives a rejection error because this branch is behind remote head (fast-forward error). To solve make again git pull and manual fix the conflicts.

- Nope. When pull form origin rollback gives an error. "he following untracked working tree files would be overwritten by merge". So instead of pull im going to merge with develop branch.

- Nope. Not working either, same untraked files for merging error.

- It says I have to move or remove them... let's move the conflict to another folder!

- Yep, this worked! Now I just have to manually fix the merge conflict done by my rollback pulling and that's it!
