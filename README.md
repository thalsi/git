# 🧠 Git Mastery Checklist (Beginner → Advanced)

Master Git step-by-step from beginner to advanced. Check off tasks as you complete them!

---

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

---

## 🌐 4. Remote Repositories
- [ ] git remote add origin <url>
- [ ] git push -u origin main
- [ ] git push / git pull
- [ ] git clone <url>
- [ ] git remote -v

---

## 🧼 5. Undo & History Fixing
- [ ] git reset --soft / --mixed / --hard
- [ ] git restore <file>
- [ ] git commit --amend
- [ ] git reflog
- [ ] git clean -fd

---

## 🔁 6. Rebase & Cherry-Pick
- [ ] git rebase <branch>
- [ ] git rebase -i HEAD~n
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

---

## 👥 10. Team Collaboration
- [ ] Use Pull Requests / Merge Requests
- [ ] Feature branch workflow
- [ ] Gitflow workflow
- [ ] Code review & approvals
- [ ] Protected branches

---

## 🛠️ 11. Git Hooks & Automation
- [ ] Setup Husky for hooks
- [ ] Use pre-commit, commit-msg, post-merge
- [ ] Use lint-staged for auto formatting
- [ ] Create .husky/ scripts

---

## 🗂️ 12. Aliases & Tools
- [ ] Create git aliases
- [ ] Use Git GUI tools
- [ ] Use .gitattributes
- [ ] Try https://learngitbranching.js.org

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
- [ ] git reset --merge to undo merge

---

## 🚀 15. CI/CD Integration
- [ ] Setup GitHub Actions or GitLab CI
- [ ] Configure .github/workflows/
- [ ] Use CI for test/lint/build
- [ ] Auto deployment with git tags

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

## 🔐 18. Security & Best Practices
- [ ] Use .env files and gitignore
- [ ] Install git-secrets
- [ ] GPG sign commits
- [ ] Enable 2FA on GitHub

---

## 🏢 19. Git in Teams
- [ ] Simulate team workflows
- [ ] Use pair programming tools (git-duet)
- [ ] Create/merge PRs
- [ ] Squash commits before merge

---

## 🌍 20. Git Hosting Platforms
- [ ] GitHub
- [ ] GitLab
- [ ] Bitbucket
- [ ] Azure Repos

---

## 📚 21. Learning Resources
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
