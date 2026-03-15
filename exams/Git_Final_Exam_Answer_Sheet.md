# Git Final Exam Answer Sheet

## Section 1: Multiple Choice

1. Which command initializes a new Git repository?
    - A. `git start`
    - B. `git new`
    - **C. `git init`**
    - D. `git create`

2. What does `git clone <url>` do?
    - A. Creates an empty repo
    - **B. Copies a remote repo to your local machine**
    - C. Downloads only the latest file
    - D. Creates a new branch

3. Which command stages all modified files for the next commit?
    - A. `git stage .`
    - **B. `git add .`**
    - C. `git commit`
    - D. `git push`

4. What does `git status` show?
    - A. The full commit history
    - **B. Staged, unstaged, and untracked files**
    - C. The diff of the last commit
    - D. A list of remote branches

5. Which command downloads remote changes AND merges them into your current branch?
    - A. `git fetch`
    - B. `git sync`
    - C. `git merge`
    - **D. `git pull`**

6. What does `git log` display?
    - A. Files changed since the last commit
    - **B. A history of commits**
    - C. The current branch name
    - D. Remote repository URLs

7. Which command temporarily shelves uncommitted changes so you can switch tasks?
    - A. `git hide`
    - B. `git save`
    - **C. `git stash`**
    - D. `git hold`

8. What does `git checkout <branch>` do?
    - A. Creates and switches to a new branch
    - B. Merges the branch into main
    - **C. Switches to an existing branch**
    - D. Deletes the branch

9. What does `git checkout .` do?
    - A. Creates a new branch from the current commit
    - B. Stages all modified files for the next commit
    - **C. Discards all unstaged changes in the working directory, reverting tracked files to the last commit**
    - D. Switches to the previous branch you were on

10. What does `git show <commit>` display?
    - A. A list of all commits in the repository
    - **B. The diff and metadata of a specific commit**
    - C. The current state of the working directory
    - D. A summary of commits by author

11. What does `git diff` show?
    - A. The full commit history
    - **B. Differences between the working directory and the last commit**
    - C. Differences between two commits
    - D. A list of remote branches

12. What does `git checkout -b <branch>` do?
    - A. Deletes a branch and creates a new one with the given name
    - **B. Creates a new branch and switches to it in one step**
    - C. Switches to an existing branch only if it has no uncommitted changes
    - D. Creates a new branch without switching to it

13. What does `git commit --amend` do?
    - A. Creates a new branch from the last commit
    - B. Reverts the last commit and stages the changes
    - **C. Modifies the most recent commit, allowing you to change its message or add forgotten staged files**
    - D. Copies the last commit onto another branch

14. Which command applies a single specific commit from another branch onto your current branch?
    - A. `git merge`
    - **B. `git cherry-pick <commit>`**
    - C. `git apply`
    - D. `git patch`

15. What is the main difference between `git rebase` and `git merge`?
    - A. Rebase deletes the source branch; merge does not
    - **B. Rebase rewrites commit history to create a linear sequence; merge preserves the branch history**
    - C. Rebase only works on remote branches; merge works on local branches
    - D. They are identical in behavior

16. What does `git reflog` record that `git log` does NOT?
    - A. Commit messages and authors
    - **B. Every movement of HEAD, including resets, rebases, and checkouts**
    - C. Changes to remote branches
    - D. The diff of each commit

17. A developer accidentally ran `git reset --hard` and lost commits. Which command would help them recover?
    - A. `git log`
    - B. `git stash list`
    - **C. `git reflog`**
    - D. `git fetch`

18. What does `git stash pop` do?
    - A. Permanently deletes the most recent stash
    - B. Shows a list of all stashes
    - **C. Restores the most recently stashed changes and removes them from the stash list**
    - D. Saves your current changes to the stash

19. What does `git diff --staged` show?
    - A. Differences between two branches
    - B. Differences between the working directory and the last commit
    - **C. Differences between staged changes and the last commit**
    - D. Differences between local and remote branches

20. What is `git tag` used for?
    - A. Adding labels to files
    - **B. Marking a specific commit with a named label, commonly used for releases**
    - C. Renaming a branch
    - D. Grouping commits together

21. What does `git remote -v` display?
    - A. The current branch's commit history
    - B. A list of all local branches
    - **C. The names and URLs of connected remote repositories**
    - D. Verbose output of the last push

22. What is the difference between `git reset --hard`, `git reset --soft`, and `git reset --mixed`?
    - A. They all do the same thing but operate on different branches
    - **B. `--hard` deletes the commit and all changes; `--soft` keeps changes staged; `--mixed` keeps changes but unstages them**
    - C. `--hard` unstages changes; `--soft` deletes changes; `--mixed` moves them to a new branch
    - D. `--hard` works on remote branches; `--soft` and `--mixed` only work locally

23. What is the purpose of a `.gitignore` file?
    - A. It lists all contributors to the repository
    - B. It stores the commit history locally
    - **C. It specifies files and directories that Git should not track or stage**
    - D. It prevents other users from pushing to the repository

---

## Section 2: Fill in the Blank

24. Save your staged changes with the message "fix bug":
    - `git` **`commit`** `-m "fix bug"`

25. Upload your local commits to the remote repository:
    - `git` **`push`**

26. Create a new branch called `feature-login`:
    - `git branch` **`feature-login`**

27. Check which branch you are currently on:
    - `git` **`status`**

28. Show the differences between your working directory and the last commit:
    - `git` **`diff`**

29. Switch to a branch called `dev` using the older syntax:
    - `git checkout` **`dev`**

30. Switch to a branch called `dev` using the new syntax:
    - `git switch` **`dev`**

31. Show the diff and metadata of commit `a3f5c91`:
    - `git show` **`a3f5c91`**

32. Change the message of your last commit to "correct message":
    - `git commit --amend -m "` **`correct message`** `"`

33. Apply the commit with hash `a3f5c91` onto your current branch:
    - `git cherry-pick` **`a3f5c91`**

34. Reapply your current branch's commits on top of `main`:
    - `git rebase` **`main`**

35. Undo `git add .` using the modern syntax:
    - `git` **`restore`** `--staged`

36. Discard uncommitted changes to `index.html` and restore it to its last committed state:
    - `git checkout --` **`index.html`**

37. View the full local history of HEAD movements:
    - `git` **`reflog`**

38. After finding a lost commit hash `b4d2a11` in the reflog, restore your branch to it:
    - `git reset --hard` **`b4d2a11`**

39. Show the differences between your staged changes and the last commit:
    - `git diff` **`--staged`**

40. Create a tag named `v1.0` on the current commit:
    - `git tag` **`v1.0`**

41. View the URLs of your remote repositories:
    - `git` **`remote -v`**

42. Restore your most recently stashed changes and keep them on the stash:
    - `git stash` **`apply`**

43. Restore your most recently stashed changes and remove them from the stash:
    - `git stash` **`pop`**

---

## Section 3: Short Answer

44. What is the difference between `git fetch` and `git pull` in detail?

`git fetch` downloads changes from the remote repository into your local remote-tracking branches (e.g. `origin/main`) but does NOT touch your working directory or current branch. You can inspect what changed before deciding to integrate it. `git pull` is essentially `git fetch` followed by `git merge` — it downloads the changes and immediately merges them into your current branch. `git fetch` is safer when you want to review changes first; `git pull` is more convenient when you trust the remote and just want to stay up to date.

45. What is the difference between `git revert` and `git reset`?

`git revert <commit>` creates a **new commit** that undoes the changes from a specified commit. It is safe to use on shared/public branches because it does not rewrite history — it simply adds a new "undo" commit on top. `git reset`, on the other hand, **moves the branch pointer backwards**, effectively removing commits from the history. This rewrites history, which can cause problems for collaborators if used on a shared branch. Use `git revert` for public branches and `git reset` for local, private cleanup.

46. Give a practical example of when you would use `git cherry-pick` instead of `git merge`.

Imagine you are working on a `feature` branch that is not yet ready to merge into `main`, but it contains one specific bug fix commit that needs to go to production immediately. Rather than merging the entire unfinished feature branch (which would pull in incomplete work), you can use `git cherry-pick <commit-hash>` to apply just that one fix commit onto `main`. This lets you ship the fix without merging unrelated in-progress changes.

47. When would you choose `git rebase` over `git merge`, and what risk does rebase carry?

You would choose `git rebase` when you want a clean, linear commit history — for example, before opening a pull request, you might rebase your feature branch onto `main` so your commits sit neatly on top of the latest work, without a merge commit cluttering the log. The key risk is that rebase **rewrites commit hashes** — every rebased commit gets a new SHA. If you have already pushed your branch and others have based work on it, rebasing will cause conflicts and confusion for your collaborators. The golden rule is: never rebase a branch that others are working on.

48. Explain what `git reflog` is and describe a scenario where it could save you from losing work.

`git reflog` is a local log of every position HEAD has been at — including branch switches, commits, resets, rebases, and merges. Unlike `git log`, it records movements that don't appear in the normal commit history. Scenario: you run `git reset --hard HEAD~3` intending to remove the last 3 commits, then realise you deleted important work. Running `git reflog` shows the SHA that HEAD pointed to before the reset. You can then run `git reset --hard <that-sha>` to restore your branch exactly as it was before the mistake.

49. Describe the typical workflow from editing a file to pushing it to a remote repo (list the commands in order).

```bash
# 1. Edit your file(s) in your editor

# 2. Check what has changed
git status

# 3. Stage the changes
git add .

# 4. Commit with a message
git commit -m "your message here"

# 5. Push to the remote repository
git push
```

50. You have a project with a `node_modules/` folder and a `.env` file containing secrets. What would you put in your `.gitignore`, and why is it important to do this before the first commit?

```text
node_modules/
.env
```

`node_modules/` should be ignored because it contains thousands of dependency files that can be regenerated at any time with `npm install` — committing them bloats the repository unnecessarily. `.env` must be ignored because it contains secrets such as API keys, database passwords, and tokens. If these are committed and pushed to a public (or even private) repository, they can be exposed and exploited. It is critical to add these to `.gitignore` **before the first commit** because once a file is committed, it enters the Git history — even if you delete it in a later commit, the secret remains accessible in the history and must be considered compromised.

51. What does `git rebase -i HEAD~5` do? Give one example of why you might use it.

`git rebase -i HEAD~5` opens an interactive rebase for the last 5 commits. It presents a list of those commits in a text editor, each prefixed with a command (`pick`, `squash`, `reword`, `drop`, etc.) that you can change to control what happens to each commit. Example: you have been working on a feature and made 5 messy commits with messages like "wip", "fix typo", "actually fix typo". Before merging, you can use `git rebase -i HEAD~5` to squash them all into a single clean commit with a meaningful message, keeping the project history readable and professional.

52. When would using `git log --graph` be helpful?

`git log --graph` is most useful when you need to understand the shape of the repository's history rather than just a flat list of commits. It is helpful when visualising where branches diverged and where they were merged back in, reviewing whether a branch has been rebased cleanly before a pull request, debugging merge conflicts by tracing which branch introduced which changes, onboarding to a new codebase to understand how the team works, or spotting accidental orphaned branches. It is most powerful combined with `--oneline --all --decorate`: `git log --graph --oneline --all --decorate`.
