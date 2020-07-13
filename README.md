# undo-push-experiment

Testing how can I revert an ooopps-push into a develop branch without breaking anything

### This branc approach:

- This branch has been forked from the develop errored one
- We will use git log to find the OK last commit and git reset sha to commit propperly and do not upload the wrong files.
- Then we will push so the head of the branch is updated.
