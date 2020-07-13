# undo-push-experiment

Testing how can I revert an ooopps-push into a develop branch without breaking anything

### Possible fix approaches at elegant-merge branch:

- Forked from errored-commit develop head. This is going to emulate develop branch (as in this repo develop branch is the one with the problem so we dont want to solve it there.)
- Merged with the rollback branch solution.

Why this way? If you prefer "modularize" the commits fixed in a different branch in order to take care of the develop branch and make this as a "hotfix" of the commits.

