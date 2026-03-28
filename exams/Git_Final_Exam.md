# Git Final Exam

## Section 1: Multiple Choice

1. Which command initializes a new Git repository?
    - A. `git start`
    - B. `git new`
    - C. `git init`
    - D. `git create`

2. What does `git clone <url>` do?
    - A. Creates an empty repo
    - B. Copies a remote repo to your local machine
    - C. Downloads only the latest file
    - D. Creates a new branch

3. Which command stages all modified files for the next commit?
    - A. `git stage .`
    - B. `git add .`
    - C. `git commit`
    - D. `git push`

4. What does `git status` show?
    - A. The full commit history
    - B. Staged, unstaged, and untracked files
    - C. The diff of the last commit
    - D. A list of remote branches

5. Which command downloads remote changes AND merges them into your current branch?
    - A. `git fetch`
    - B. `git sync`
    - C. `git merge`
    - D. `git pull`

6. What does `git log` display?
    - A. Files changed since the last commit
    - B. A history of commits
    - C. The current branch name
    - D. Remote repository URLs

7. Which command temporarily shelves uncommitted changes so you can switch tasks?
    - A. `git hide`
    - B. `git save`
    - C. `git stash`
    - D. `git hold`

8. What does `git checkout <branch>` do?
    - A. Creates and switches to a new branch
    - B. Merges the branch into main
    - C. Switches to an existing branch
    - D. Deletes the branch

9. What does `git checkout .` do?
    - A. Creates a new branch from the current commit
    - B. Stages all modified files for the next commit
    - C. Discards all unstaged changes in the working directory, reverting tracked files to the last commit
    - D. Switches to the previous branch you were on

10. What does `git show <commit>` display?
    - A. A list of all commits in the repository
    - B. The diff and metadata of a specific commit
    - C. The current state of the working directory
    - D. A summary of commits by author

11. What does `git diff` show?
    - A. The full commit history
    - B. Differences between the working directory and the last commit
    - C. Differences between two commits
    - D. A list of remote branches

12. What does `git checkout -b <branch>` do?
    - A. Deletes a branch and creates a new one with the given name
    - B. Creates a new branch and switches to it in one step
    - C. Switches to an existing branch only if it has no uncommitted changes
    - D. Creates a new branch without switching to it

13. What does `git commit --amend` do?
    - A. Creates a new branch from the last commit
    - B. Reverts the last commit and stages the changes
    - C. Modifies the most recent commit, allowing you to change its message or add forgotten staged files
    - D. Copies the last commit onto another branch

14. Which command applies a single specific commit from another branch onto your current branch?
    - A. `git merge`
    - B. `git cherry-pick <commit>`
    - C. `git apply`
    - D. `git patch`

15. What is the main difference between `git rebase` and `git merge`?
    - A. Rebase deletes the source branch; merge does not
    - B. Rebase rewrites commit history to create a linear sequence; merge preserves the branch history
    - C. Rebase only works on remote branches; merge works on local branches
    - D. They are identical in behavior

16. What does `git reflog` record that `git log` does NOT?
    - A. Commit messages and authors
    - B. Every movement of HEAD, including resets, rebases, and checkouts
    - C. Changes to remote branches
    - D. The diff of each commit

17. A developer accidentally ran `git reset --hard` and lost commits. Which command would help them recover?
    - A. `git log`
    - B. `git stash list`
    - C. `git reflog`
    - D. `git fetch`

18. What does `git stash pop` do?
    - A. Permanently deletes the most recent stash
    - B. Shows a list of all stashes
    - C. Restores the most recently stashed changes and removes them from the stash list
    - D. Saves your current changes to the stash

19. What does `git diff --staged` show?
    - A. Differences between two branches
    - B. Differences between the working directory and the last commit
    - C. Differences between staged changes and the last commit
    - D. Differences between local and remote branches

20. What is `git tag` used for?
    - A. Adding labels to files
    - B. Marking a specific commit with a named label, commonly used for releases
    - C. Renaming a branch
    - D. Grouping commits together

21. What does `git remote -v` display?
    - A. The current branch's commit history
    - B. A list of all local branches
    - C. The names and URLs of connected remote repositories
    - D. Verbose output of the last push

22. What is the difference between `git reset --hard`, `git reset --soft`, and `git reset --mixed`?
    - A. They all do the same thing but operate on different branches
    - B. `--hard` deletes the commit and all changes; `--soft` keeps changes staged; `--mixed` keeps changes but unstages them
    - C. `--hard` unstages changes; `--soft` deletes changes; `--mixed` moves them to a new branch
    - D. `--hard` works on remote branches; `--soft` and `--mixed` only work locally

23. What is the purpose of a `.gitignore` file?
    - A. It lists all contributors to the repository
    - B. It stores the commit history locally
    - C. It specifies files and directories that Git should not track or stage
    - D. It prevents other users from pushing to the repository

---

## Section 2: Fill in the Blank

24. Save your staged changes with the message "fix bug":
    - `git __________ -m "fix bug"`

25. Upload your local commits to the remote repository:
    - `git __________`

26. Create a new branch called `feature-login`:
    - `git branch __________`

27. Check which branch you are currently on
    - `git __________`

28. Show the differences between your working directory and the last commit:
    - `git __________`

29. Switch to a branch called `dev` using the older syntax:
    - `git checkout __________`

30. Switch to a branch called `dev` using the new syntax:
    - `git switch __________`

31. Show the diff and metadata of commit `a3f5c91`:
    - `git show __________`

32. Change the message of your last commit to "correct message":
    - `git commit --amend -m "__________"`

33. Apply the commit with hash `a3f5c91` onto your current branch:
    - `git cherry-pick __________`

34. Reapply your current branch's commits on top of `main`:
    - `git rebase __________`

35. Undo this command `git add .` using the modern syntax
    - `git __________ --staged`

36. Discard uncommitted changes to `index.html` and restore it to its last committed state:
    - `git checkout -- __________`

37. View the full local history of HEAD movements:
    - `git __________`

38. After finding a lost commit hash `b4d2a11` in the reflog, restore your branch to it:
    - `git reset --hard __________`

39. Show the differences between your staged changes and the last commit:
    - `git diff __________`

40. Create a tag named `v1.0` on the current commit:
    - `git tag __________`

41. View the URLs of your remote repositories:
    - `git __________`

42. Restore your most recently stashed changes and keep them on the stash:
    - `git stash __________`

43. Restore your most recently stashed changes and remove them from the stash:
    - `git stash __________`

44. Undo a `git add .` operation (unstage all staged changes):
    - `git __________ --staged .`

---

## Section 3: Short Answer

45. What is the difference between `git fetch` and `git pull` in detail?

46. What is the difference between `git revert` and `git reset`?

47. Give a practical example of when you would use `git cherry-pick` instead of `git merge`.

48. When would you choose `git rebase` over `git merge`, and what risk does rebase carry?

49. Explain what `git reflog` is and describe a scenario where it could save you from losing work.

50. Describe the typical workflow from editing a file to pushing it to a remote repo (list the commands in order).

51. You have a project with a `node_modules/` folder and a `.env` file containing secrets. What would you put in your `.gitignore`, and why is it important to do this before the first commit?

52. What does `git rebase -i HEAD~5` do? Give one example of why you might use it.

53. When would using `git log --graph` be helpful?
