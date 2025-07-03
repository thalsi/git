# ✅ Git Mastery Checklist (Beginner → Advanced)

---
🟢 Beginner

## 🧩 1. Setup & Configuration
- [ ] Install Git
- [ ] git config --global user.name "Your Name"
- [ ] git config --global user.email "you@example.com"
- [ ] Set default branch: `init.defaultBranch main`
- [ ] Set default editor: VS Code, Vim, etc.
- [ ] Enable color UI
- [ ] View current config: `git config --list`

---

## 📁 2. Git Basics
- [ ] git init
- [ ] git status
- [ ] git add <file> / git add .
- [ ] git commit -m "message"
- [ ] git log / git log --oneline
- [ ] git diff
- [ ] git show
- [ ] Use .gitignore

---

## 🌿 3. Branching & Merging
- [ ] git branch
- [ ] git checkout <branch> / git switch
- [ ] git checkout -b <branch>
- [ ] git merge <branch>
- [ ] git branch -d <branch>
- [ ] git log --graph
- [ ] Rebase vs Merge (pros/cons)

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
- [ ] git rebase <branch>
- [ ] git rebase -i HEAD~n
- [ ] git rebase --autosquash
- [ ] git rebase --abort / --skip / --continue
- [ ] Resolve conflicts
- [ ] git cherry-pick <commit>
- [ ] git merge --squash

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
