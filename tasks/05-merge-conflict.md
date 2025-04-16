# Task 05: Resolve a Merge Conflict

## Objective
Learn to handle merge conflicts during a rebase or merge.

## Scenario
We've created two versions of the same file:
- `misc/conflict-demo.md` (main branch)
- `misc/conflict-demo-feature.md` (your branch)

Each file contains a conflicting change to the same line.

## Steps

1. Create a new branch: `git checkout -b yourname/conflict-branch`
2. Replace the file with `conflict-demo-feature.md` content
3. Commit your changes
4. Switch back to main and merge your branch: `git merge yourname/conflict-branch`
5. Git will report a conflict. Open the file and resolve it manually.
6. After resolving, add the file and complete the merge.

## Deliverable
Comment on your PR describing the conflict and how you resolved it.
