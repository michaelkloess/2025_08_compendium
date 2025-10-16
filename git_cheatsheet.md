## Git Cheat Sheet

| Command                                             | Description                                         |
| --------------------------------------------------- | --------------------------------------------------- |
| `git init`                                          | Start a new repo                                    |
| `git clone <url>`                                   | Clone an existing repo                              |
| `git add <file>`                                    | Add untracked file or unstaged changes              |
| `git add .`                                         | Add all untracked files and unstaged changes        |
| `git add -p`                                        | Choose which parts of a file to stage               |
| `git mv <old> <new>`                                | Move file                                           |
| `git rm <file>`                                     | Delete file                                         |
| `git rm --cached <file>`                            | Tell Git to forget about a file without deleting it |
| `git reset <file>`                                  | Unstage one file                                    |
| `git reset`                                         | Unstage everything                                  |
| `git status`                                        | Check what you added                                |
| `git commit`                                        | Make a commit (open editor for message)             | 
| `git commit -m 'message'`                           | Make a commit                                       |
| `git commit -am 'message'`                          | Commit all unstaged changes                         |
| `git switch <name>`                                 | Switch branches                                     |
| `git checkout <name>`                               | Switch branches (alt syntax)                        |
| `git switch -c <name>`                              | Create a branch                                     |
| `git checkout -b <name>`                            | Create a branch (alt syntax)                        |
| `git branch`                                        | List branches                                       |
| `git branch --sort=-committerdate`                  | List branches by most recent commit                 |
| `git branch -d <name>`                              | Delete a branch                                     |
| `git branch -D <name>`                              | Force delete a branch                               |
| `git diff HEAD`                                     | Diff all staged and unstaged changes                |
| `git diff --staged`                                 | Diff just staged changes                            |
| `git diff`                                          | Diff just unstaged changes                          |
| `git show <commit>`                                 | Show diff between commit and parent                 |
| `git diff <commit> <commit>`                        | Diff two commits                                    |
| `git diff <commit> <file>`                          | Diff one file since a commit                        |
| `git diff <commit> --stat`                          | Show summary of a diff                              |
| `git show <commit> --stat`                          | Show commit summary with stats                      |
| `git restore <file>`                                | Delete unstaged changes to one file                 |
| `git checkout <file>`                               | Same as above (alt syntax)                          |
| `git restore --staged --worktree <file>`            | Delete all staged and unstaged changes to file      |
| `git checkout HEAD <file>`                          | Same as above (alt syntax)                          |
| `git reset --hard`                                  | Delete all staged and unstaged changes              |
| `git clean`                                         | Delete untracked files                              |
| `git stash`                                         | Stash staged and unstaged changes                   |
| `git reset HEAD^`                                   | Undo last commit (keep working dir)                 |
| `git rebase -i HEAD~6`                              | Squash last 5 commits into one                      |
| `git reflog BRANCHNAME`                             | Undo a failed rebase                                |
| `git reset --hard <commit>`                         | Reset branch to a specific commit                   |
| `git commit --amend`                                | Change last commit message or add file              |
| `git log main`                                      | View branch history                                 |
| `git log --graph main`                              | View branch history (graph)                         |
| `git log --oneline`                                 | Compact one-line log                                |
| `git log <file>`                                    | Show commits that modified a file                   |
| `git log --follow <file>`                           | Show commits before file was renamed                |
| `git log -G <text>`                                 | Find commits adding/removing text                   |
| `git blame <file>`                                  | Show who last changed each line                     |
| `git switch banana` + `git rebase main`             | Combine diverged branches (rebase)                  |
| `git switch main` + `git merge banana`              | Combine diverged branches (merge)                   |
| `git switch main` + `git merge --squash banana` + `git commit` | Combine diverged branches (squash merge) |
| `git switch main` + `git merge banana`              | Fast-forward merge                                  |
| `git cherry-pick <commit>`                          | Copy one commit onto current branch                 |
| `git checkout <commit> <file>`                      | Restore old file version                            |
| `git restore <file> --source <commit>`              | Restore old file version (alt syntax)               |
| `git remote add <name> <url>`                       | Add a remote                                        |
| `git push origin main`                              | Push main branch to origin                          |
| `git push`                                          | Push current branch                                 |
| `git push -u origin <name>`                         | Push branch first time                              |
| `git push --force-with-lease`                       | Force push safely                                   |
| `git push --tags`                                   | Push tags                                           |
| `git fetch origin main`                             | Fetch without merge                                 |
| `git pull --rebase`                                 | Pull with rebase                                    |  
| `git pull origin main`                              | Pull and merge                                      |
| `git pull`                                          | Pull (short form)                                   |
| `git config user.name 'Your Name'`                  | Set config option                                   |
| `git config --global ...`                           | Set option globally                                 |
| `git config alias.st status`                        | Add an alias                                        |
| `man git-config`                                    | Show all config options                             |
| `.git/config`                                       | Local git config file                               |
| `~/.gitconfig`                                      | Global git config file                              |
| `.gitignore`                                        | List of ignored files                               |
