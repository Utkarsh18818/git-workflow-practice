# Exercise 1: Branches and pull requests
This sandbox records Git workflow practice, not production work.
## Goal
Make a focused change on a branch, inspect the diff, and merge through a pull request.
## Steps
1. Clone the repository and run `git switch main`.
2. Update the starting point with `git pull --ff-only`.
3. Create a branch: `git switch -c practice/describe-change`.
4. Make one useful documentation change.
5. Inspect `git diff` and `git status`.
6. Stage the intended file; inspect `git diff --cached`.
7. Commit with a descriptive message and push the branch.
8. Open a pull request explaining the change and verification.
9. Inspect Files changed before merging.
10. Update local main after the merge.
## Review checklist
- Include only the intended change.
- Exclude secrets, tokens and private data.
- Check commands and links.
- Follow existing review and CI requirements in production repositories.
AI assistance was used to draft this practice material.
