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
- [ ] `git merge <branch>` – Merge the specified branch into the current branch  
- [ ] `git merge --no-ff <branch>` – Always create a merge commit (no fast-forward)  
- [ ] `git merge --squash <branch>` – Combine changes into one commit before merging  
- [ ] `git merge --commit` – Perform the merge and commit immediately (default)  
- [ ] `git merge --no-commit` – Merge but don’t automatically create a commit  
- [ ] `git merge --edit` – Edit the merge commit message before committing  
- [ ] `git merge --no-edit` – Use default commit message without editing  
- [ ] `git merge --strategy=<strategy>` – Use a specific merge strategy (e.g., recursive, ours, theirs)  
- [ ] `git merge --strategy-option=<option>` – Pass options to the merge strategy  
- [ ] `git merge --abort` – Abort the merge and return to pre-merge state  
- [ ] `git merge --continue` – Continue merge after conflicts are resolved  
- [ ] `git merge --skip` – Skip the current conflicting commit during merge  
- [ ] `git log --merge` – Show commits causing the merge conflict  
- [ ] `git diff --name-only --diff-filter=U` – Show files with merge conflicts  
- [ ] Resolve conflicts manually – Edit conflicting files and mark them as resolved  
- [ ] `git status` – See current merge state and conflicted files  
- [ ] `git commit` – Complete merge after resolving conflicts (if auto-commit is disabled)  

---

## 🌐 4. Remote Repositories
- [ ] git remote add origin <url>
- [ ] git push -u origin main
- [ ] git push / git pull
- [ ] git clone <url>
- [ ] git remote -v
- [ ] git push --set-upstream origin <branch>
- [ ] git branch -vv
- [ ] git branch --set-upstream-to

---

## 🧼 5. Undo & History Fixing
- [ ] git reset --soft / --mixed / --hard
- [ ] git restore <file>
- [ ] git commit --amend
- [ ] git reflog
- [ ] git clean -fd
- [ ] git reset --merge (undo merge)

---
🟡 Intermediate

## 🔁 6. Rebase & Cherry-Pick

### 🍒 Cherry-pick
- [ ] `git cherry-pick <commit>` – Apply specific commit from another branch  

### Rebase
git rebase moves or reapplies commits from one branch on top of another.
It rewrites history to create a cleaner, linear commit history.

🎯 When to Use Rebase
✅ Clean up history
✅ Avoid extra merge commits
✅ Keep project history linear
✅ Re-apply your local feature branch on top of main

- [ ] `git rebase <branch>` – Reapply current branch commits on top of `<branch>`  
- [ ] `git rebase -i <branch>` – Interactive rebase: squash, reword, drop commits  
- [ ] `git rebase -i HEAD~n` – Interactively edit the last `n` commits  
- [ ] `git rebase --autosquash` – Auto-squash commits marked with `fixup!` or `squash!`  
- [ ] `git rebase --continue` – Continue rebase after resolving conflicts  
- [ ] `git rebase --abort` – Abort the rebase and return to the previous state  
- [ ] `git rebase --skip` – Skip the current conflicting commit during rebase  
- [ ] `git pull --rebase` – Pull latest changes using rebase instead of merge  
- [ ] `git status` – Check status during rebase (conflicts, progress)  
- [ ] `git log` – Review commit history before/after rebase  
- [ ] Resolve conflicts manually – Fix file conflicts and mark as resolved  

---

## 🏷️ 7. Tags & Releases
- [ ] git tag <name>
- [ ] git tag -a <name> -m "message"
- [ ] git show <tag>
- [ ] git push origin <tag>
- [ ] git push --tags

---

## 📦 8. Stashing & Cleaning
- [ ] git stash
- [ ] git stash list
- [ ] git stash apply / pop
- [ ] git stash drop / clear

---

## 🔍 9. Git Inspection Tools
- [ ] git log with formatting
- [ ] git diff --cached
- [ ] git blame <file>
- [ ] git shortlog
- [ ] git describe
- [ ] git shortlog -sn

---

## 👥 10. Team Collaboration
- [ ] Use Pull Requests / Merge Requests
- [ ] Feature branch workflow
- [ ] Gitflow workflow
- [ ] Code review & approvals
- [ ] Protected branches
- [ ] Squash commits before merge

---

## 🛠️ 11. Git Hooks & Automation
- [ ] Setup Husky for hooks
- [ ] Use pre-commit, commit-msg, post-merge
- [ ] Use lint-staged for auto formatting
- [ ] Create .husky/ scripts
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
- [ ] Use Conventional Commits (feat:, fix:, chore:, etc.)
- [ ] Install commitlint
- [ ] Use Commitizen (cz) for commits
- [ ] Validate commits with hooks

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
