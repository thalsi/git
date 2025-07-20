# ✅ Git Mastery Checklist (Beginner → Advanced)

---
🟢 Beginner

## 🧩 1. Setup & Configuration
- [x] Install Git
- [x] git config --global user.name "Your Name"
- [x] git config --global user.email "you@example.com"
- [x] Set default branch: `init.defaultBranch main`
- [x] Set default editor: VS Code, Vim, etc.
- [x] Enable color UI
- [x] View current config: `git config --list`
- [x] View current config: `git config --list --global`

---

## 📁 2. Git Basics
- [x] git init
        - Initialize a new Git repository.
- [x] git status
        - Check the status of files — modified, staged, untracked.
- [x] git add <file> / git add .
        - Stage file(s) to be committed.
- [x] git commit -m "message"
        - Commit staged changes with a message.
- [x] git log / git log --oneline
        - View commit history (detailed or short).
- [x] git diff
        - See what’s changed before staging.
- [x] git show
        - Show the details of a specific commit.
- [x] Use .gitignore
        - Ignore files you don’t want Git to track (e.g., node_modules/, env, dist).

---

## 🌿 3. Branching & Merging
1. Branching

- [x] `git branch` – List all local branches  
- [x] `git branch <name>` – Create a new branch  
- [x] `git switch <branch>` – Switch to a branch (newer)  
- [x] `git checkout <branch>` – Switch to a branch (older method)  
- [x] `git checkout -b <name>` – Create and switch to a new branch  
- [x] `git branch -d <name>` – Delete a local branch (safe)  
- [x] `git branch -D <name>` – Delete a local branch (force)  
- [x] `git branch -m <new>` – Rename current branch  
- [x] `git branch -vv` – Show branches with last commit info  
- [x] `git push origin <branch>` – Push branch to remote  
- [x] `git push --set-upstream origin <branch>` – Link local branch to remote
- [x] `git fetch --all` – Fetches all branches from all remotes (usually just origin) but does NOT merge or checkout anything.
- [x] `git fetch -p` – It tells Git to remove (prune) any remote-tracking branches that no longer exist on the remote.

2. Merging
Git Merge is used to combine changes from one branch into another.
Usually, you merge a feature branch into a main/stable branch.

📦 Merge Types in Git

| Merge Type                           | Description                                                 |
| ------------------------------------ | ----------------------------------------------------------- |
| 🟢 Fast-forward Merge                | Simple move of the pointer if there’s no diverging history. |
| 🟡 Recursive Merge                   | The default merge strategy when branches have diverged.     |
| 🔵 No Fast-forward Merge (`--no-ff`) | Always creates a merge commit to preserve history.          |
| 🔴 Manual Merge                      | Required when there’s a **conflict**.                       |

✳️ Common Merge Commands
- [x] `git merge <branch>` – Merge the given branch into the current branch  
- [x] `git merge --no-ff <branch>` – Force a merge commit even on fast-forward  
- [x] `git merge --squash <branch>` – Merge and squash into a single commit  
- [x] `git merge --abort` – Abort a merge in progress  
- [x] `git merge --continue` – Continue merge after resolving conflicts  

---

## 🌐 4. Remote Repositories
- [x] git remote add origin <url>
- [x] git push -u origin main
- [x] git push / git pull
- [x] git clone <url>
- [x] git remote -v
- [x] git push --set-upstream origin <branch>
- [x] git branch -vv
- [x] git branch --set-upstream-to

---

## 🧼 5. Undo & History Fixing
- [x] git reset --soft / --mixed / --hard
- [x] git restore <file>
- [x] git restore . <file>
- [x] git restore --staged <file>
- [x] git commit --amend
- [x] git reflog
- [x] git clean -fd
- [x] git reset --merge (undo merge)

---
🟡 Intermediate

## 🔁 6. Rebase & Cherry-Pick

### 🍒 Cherry-pick
- [x] `git cherry-pick <commit>` – Apply specific commit from another branch  
- [x] `git cherry-pick commit1 commit2 commit3` – You can also cherry-pick multiple commits
- [x] `git cherry-pick A^..B` –  even a range of commits

### Rebase
git rebase moves or reapplies commits from one branch on top of another.
It rewrites history to create a cleaner, linear commit history.

🎯 When to Use Rebase
✅ Clean up history
✅ Avoid extra merge commits
✅ Keep project history linear
✅ Re-apply your local feature branch on top of main

- [x] `git rebase <branch>` – Reapply current branch commits on top of `<branch>`  
- [x] `git rebase -i <branch>` – Interactive rebase: squash, reword, drop commits  
- [x] `git rebase -i HEAD~n` – Interactively edit the last `n` commits  
- [x] `git rebase --autosquash` – Auto-squash commits marked with `fixup!` or `squash!`  
- [x] `git rebase --continue` – Continue rebase after resolving conflicts  
- [x] `git rebase --abort` – Abort the rebase and return to the previous state  
- [x] `git rebase --skip` – Skip the current conflicting commit during rebase  
- [x] `git pull --rebase` – Pull latest changes using rebase instead of merge  
- [x] `git status` – Check status during rebase (conflicts, progress)  
- [x] `git log` – Review commit history before/after rebase  
- [x] Resolve conflicts manually – Fix file conflicts and mark as resolved  

| Command  | `git rebase -i <branch>` Meaning                  |
| -------- | ------------------------------------------------- |
| `pick`   | Keep commit as-is                                 |
| `reword` | Change commit message                             |
| `edit`   | Pause to change content                           |
| `squash` | Combine with previous commit (keep both messages) |
| `fixup`  | Combine with previous, discard this message       |
| `drop`   | Delete this commit                                |
---

## 🏷️ 7. Tags & Releases
- [x] git tag <name>
- [x] git tag -a <name> -m "message"
- [x] git show <tag>
- [x] git push origin <tag>
- [x] git push --tags

---

## 📦 8. Stashing & Cleaning

- [x] `git stash` – Stash tracked modified files
- [x] `git stash -u` – Stash tracked + untracked files (not ignored)
- [x] `git stash -a` – Stash all (tracked + untracked + ignored)
- [x] `git stash list` – View list of stashes
- [x] `git stash show` – Show summary of latest stash
- [x] `git stash show -p` – Show patch/diff of latest stash
- [x] `git stash pop` – Apply stash and delete it
- [x] `git stash apply` – Apply stash but keep it
- [x] `git stash drop` – Delete latest stash
- [x] `git stash clear` – Delete all stashes
- [x] `git stash push -m "message"` – Stash with custom message

---

## 🔍 9. Git Inspection Tools
- [x] git log with formatting
- [x] git diff --cached
- [x] git blame <file>
- [x] git describe
- [x] git shortlog
- [x] git shortlog -sn

---

## 👥 10. Team Collaboration
- [x] Use Pull Requests / Merge Requests
- [x] Feature branch workflow
- [x] Gitflow workflow
- [x] Code review & approvals
- [x] Protected branches
- [x] Squash commits before merge

---

## 🛠️ 11. Git Hooks & Automation
- [x] Setup Husky for hooks
- [x] Use pre-commit, commit-msg, post-merge
- [x] Use lint-staged for auto formatting
- [x] Create .husky/ scripts
- [ ] Use `git commit --no-verify` (with caution)

---

## 🗂️ 12. Aliases & Tools
- [ ] Create git aliases
- [ ] Use Git GUI tools
- [ ] Use .gitattributes
- [ ] Try https://learngitbranching.js.org
- [ ] Use GitLens in VS Code
- [ ] Use `diff-so-fancy` for better diffs

---

## ⚙️ 13. Git Internals (Advanced)
- [ ] Understand .git/ structure
- [ ] Git Object Types: blob, tree, commit, tag
- [ ] Learn about HEAD, refs, index
- [ ] Learn SHA-1 and commit IDs

---

## 🐞 14. Debugging & Recovery
- [ ] Conflict resolution
- [ ] Detached HEAD fixes
- [ ] Use reflog to recover lost commits
- [ ] git bisect start / bad / good (binary search debugging)

---

## 🚀 15. CI/CD Integration
- [ ] Setup GitHub Actions or GitLab CI
- [ ] Configure .github/workflows/
- [ ] Use CI for test/lint/build
- [ ] Auto deployment with git tags
- [ ] Test GitHub Actions locally with `act`

---

## ✏️ 16. Commit Message Standards
- [x] Use Conventional Commits (feat:, fix:, chore:, etc.)
- [x] Install commitlint
- [x] Use Commitizen (cz) for commits
- [x] Validate commits with hooks

---

## 📁 17. Monorepo & Submodules
- [ ] git submodule add
- [ ] git submodule update --init
- [ ] Learn subtrees (optional)
- [ ] Use Nx or Lerna for monorepo

---
🔴 Advanced

## 🔐 18. Security & Best Practices
- [ ] Use .env files and gitignore
- [ ] Install git-secrets
- [ ] GPG sign commits
- [ ] Enable 2FA on GitHub
- [ ] Remove secrets from history (BFG or git filter-branch)

---

## 🏢 19. Git in Teams
- [ ] Simulate team workflows
- [ ] Use pair programming tools (git-duet)
- [ ] Create/merge PRs
- [ ] Trunk-based development
- [ ] Fork vs shared branch model

---

## 🌍 20. Git Hosting Platforms
- [ ] GitHub
- [ ] GitLab
- [ ] Bitbucket
- [ ] Azure Repos

---

## 🧪 21. Extra Git Tools
- [ ] git worktree (multiple working dirs)
- [ ] git archive (create zip/tar)
- [ ] git format-patch / git apply / git am (email-based flow)
- [ ] git fame (contribution analytics)
- [ ] git LFS for large files

---

## 📚 22. Learning Resources
- [ ] https://git-scm.com/book
- [ ] https://learngitbranching.js.org
- [ ] https://ohmygit.org
- [ ] Git cheatsheets from GitHub

---

## ✍️ BONUS: Aliases to Save Time
```bash
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.cm commit
git config --global alias.lg "log --oneline --graph --all"
```

---

## 🧠 23. Advanced History & Commit Management
- [ ] git commit --fixup and git rebase --autosquash
- [ ] git notes – add metadata/comments to commits
- [ ] git revert -n (stage multiple reverts)
- [ ] Understand orphan branches: git checkout --orphan newbranch

---

## 🗃️ 24. Repo Size & History Optimization
- [ ] git gc (garbage collection to optimize repo)
- [ ] git repack (compress objects)
- [ ] git verify-pack / git count-objects -v (inspect storage)
- [ ] Use BFG Repo-Cleaner for large repos

---

## 🛡️ 25. Git & Compliance
- [ ] Audit history for secrets (truffleHog, gitleaks)
- [ ] Enforce signed commits via branch protection
- [ ] Enforce linear history in main branch
- [ ] Use branch naming conventions and enforce them

---

## ⚡ 26. Git Performance & Scaling
- [ ] Use git sparse-checkout (large monorepos)
- [ ] Partial clone (--filter=blob:none) for huge projects
- [ ] Split large repos with git subtree split

---

## 🔧 27. Custom Git Workflows
- [ ] Setup custom merge drivers
- [ ] Setup .mailmap to unify commit authors
- [ ] Use .git/info/exclude for local-only ignores
- [ ] Custom diff drivers (e.g., for .psd files)

---

## 📈 28. Git Analytics & Stats
- [ ] Generate contributor graphs (git shortlog, git fame)
- [ ] Generate churn stats (git log --stat)
- [ ] Track contribution activity with git log --since or GitHub Insights

---

## 🔁 29. Git Replace & Filter Branch
- [ ] git replace to swap objects in history
- [ ] git filter-branch for complex rewriting
- [ ] Use with caution — avoid on shared history

---

## 🌐 30. Git Across Environments
- [ ] Use Git with GitHub CLI (gh)
- [ ] Use Git in CI runners and scripts
- [ ] Use Git in Docker images for automation
- [ ] Access GitHub/GitLab via REST API
