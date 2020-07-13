# undo-push-experiment

Testing how can I revert an ooopps-push into a develop branch without breaking anything

### Possible fix approaches at branches:

- Fork smart-merge from develop with errored commit (this branch is going to emulate a develop branch).
- Push smart-merge.
- Merge ok branch (rollback) without the "fix operation" commits: *git merge --squash rollback*.
- Solve merge conflicts. And push!

More details at each branches README.
