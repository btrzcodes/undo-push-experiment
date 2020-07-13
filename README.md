# undo-push-experiment

Testing how can I revert an ooopps-push into a develop branch without breaking anything

### Possible fix approaches at branches:

- dev-copy branch: develop branch forked from an specific sha (history has no errored commits). Blank canvas to restart saving all correct commits.
- develop-reverted branch: forked branch with no errored commits + local corrections (before pushing the develop-reverted to remote for the first time). Cleanest commits log but missing commits (even if they are errors).
- rollback branch: forked with errors. Then git reset to the OK commit. Pull from remote (will have fast-fowarded errors that can be solved by moving into a folder the untraked gitignore files) and manually fix the conficts.
- elegant-merge branch: emulates develop branch. Technique is make all git changes into a different branch (rollback approach) and when solved, merge it with develop. Instead of doing changes at develop itself. This way all history commit is accurated but develop branch is more protected from possible errors while rollingback.

More details at each branches README.
