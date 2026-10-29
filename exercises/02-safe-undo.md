# Exercise 2: Undo changes while preserving history
Use a disposable local clone for this exercise. Do not run cleanup commands against work you need.
## Inspect before changing anything
- Run `git status` to identify staged and unstaged files.
- Run `git diff` and `git diff --cached` to inspect both areas.
- Use `git log --oneline -5` to identify recent commits.
## Unstage without losing edits
- Run `git restore --staged -- path/to/file` to remove an existing tracked file from the index.
- Verify with `git status`: working-tree edits should remain.
## Revert a shared commit
1. Start from a clean working tree.
2. Identify a normal, non-merge practice commit with `git log`.
3. Run `git revert <commit-sha>` to create a new commit that reverses it.
4. Inspect `git show --stat` and the resulting file content.
5. Push the revert through a separate pull request when collaborating.
## Important boundaries
- Reverting a commit preserves the original history.
- Merge commits need a deliberate mainline choice; they are outside this exercise.
- Avoid hard resets, forced pushes and destructive cleanup during beginner practice.
- If conflicts occur, inspect them before continuing; `git revert --abort` cancels an unfinished revert.
AI assistance was used to draft this practice material.
