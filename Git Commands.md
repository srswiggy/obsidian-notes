
1. **Git add** ->Moves the changes from the working directory to the staging area
2. **Git status ->** shows the tracked and untracked files in the staging area
3. **Git init** -> initialize a git repository. It creates a .git folder which tracks all the changes.
4. **Git reset** -> remove the staged files (used often)
5. **Git commit ->** saves the file in the timeline
6. **Git rm <file name>** -> remove the staged files
7.  **Git branch ->** To list all the available branches and the branch where the HEAD is pointing towards
8. **Git branch <branch name> ->** creates a new branch but doesn’t checkout to that branch
9. **Git branch -d/-D <branch name> ->** this deletes the branch. Former one is safe delete but the latter one is not
10. **Git branch -m <branch name> ->** this renames the current branch to <branch name>
11. **Git log —oneline ->** shows the history of git commits
12. **Git checkout <sha1 hash> ->** redirects the head to point to the git
13. **Git revert HEAD ->** creates an inverse commit of the last commit
14. **Git reset —hard <SHA1 Hash> ->** goes back to the given commit and deletes the commits done after that commit
15. **Git checkout <branch name> ->** points the head to point to the <branch name>
16. **Git checkout -b <branch name> ->** creates a new <branch> and points the head to that branch as well
17. **Git clean -f ->** deletes all the untracked files (not staged files)
18. **Git merge <branch name> ->** merges the branch <branch name> to current branch (checkout to receiver branch before merging)
19. **Git push ->**  Pushes the commits to the remote repository
20. **Git clone ->** creates a local clone of the commits
21. **Git pull ->** Pulls the latest commit from remote repository and merges them into the local (git pull = git fetch + git merge)
22. **Git fetch ->** Pulls the latest commit from remote repository but do not merge, requires separate git merge command