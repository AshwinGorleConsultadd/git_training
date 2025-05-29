
## Git Commands

### Basic Setup 

| Purpose       | Command                                        | Description                          |
|---------------|------------------------------------------------|--------------------------------------|
| Set Name      | git config --global user.name "Your Name"      | Sets the global username for commits |
| Set Email     | git config --global user.email "you@example.com" | Sets the global email for commits    |
| Check Config  | git config --list                              | Lists all config settings            |
| Set Editor    | git config --global core.editor "code"         | Sets default editor (e.g., VS Code)  |



### Repo management
| Purpose       | Command                | Description                          |
|---------------|------------------------|--------------------------------------|
| Initialize    | git init               | Create a new Git repository          |
| Clone Repo    | git clone <url>        | Clone a remote repository            |
| Check Status  | git status             | Show changed files and current branch |
| Check Logs    | git log                | View commit history                  |
| Short Log     | git log --oneline      | Compact commit history               |
| Repo Info     | git remote -v          | Show remotes linked to repo          |

### Staging & Committing
| Purpose         | Command                         | Description                                    |
|-----------------|----------------------------------|------------------------------------------------|
| Stage File      | git add <file>                  | Add specific file to staging area             |
| Stage All       | git add . or git add -A         | Add all changes                               |
| Commit          | git commit -m "message"         | Commit staged changes with message            |
| Amend Commit    | git commit --amend              | Modify last commit (message or staged changes)|
| Unstage File    | git reset <file>                | Remove file from staging                      |

### Branching & Merging

| Purpose         | Command                           | Description                                     |
|-----------------|------------------------------------|-------------------------------------------------|
| List Branches   | git branch                        | Show all local branches                         |
| Create Branch   | git branch <name>                 | Create a new branch                             |
| Switch Branch   | git checkout <name>               | Switch to an existing branch                    |
| Create+Switch   | git checkout -b <name>            | Create and switch to new branch                 |
| Rename Branch   | git branch -m <new-name>          | Rename current branch                           |
| Delete Branch   | git branch -d <name>              | Delete local branch                             |
| Merge Branch    | git merge <branch>                | Merge specified branch into current             |
| Abort Merge     | git merge --abort                 | Cancel an ongoing merge                         |


### Remote Repositories
| Purpose         | Command                            | Description                                      |
|-----------------|-------------------------------------|--------------------------------------------------|
| Add Remote      | git remote add origin <url>        | Link local repo to remote                        |
| Fetch Changes   | git fetch                          | Download from remote (but don’t merge)           |
| Pull Changes    | git pull                           | Fetch and merge changes from remote              |
| Push Changes    | git push                           | Push committed changes to remote                 |
| Push Branch     | git push -u origin <branch>        | Push and set upstream                            |
| Remove Remote   | git remote remove <name>           | Remove a remote repository                       |

### Undo & Reset
| Purpose         | Command                            | Description                                      |
|-----------------|-------------------------------------|--------------------------------------------------|
| Discard Changes | git checkout -- <file>             | Revert file to last commit state                 |
| Unstage File    | git reset <file>                   | Remove from staging                              |
| Soft Reset      | git reset --soft HEAD~1            | Undo last commit, keep changes staged            |
| Mixed Reset     | git reset --mixed HEAD~1           | Undo last commit, keep changes unstaged          |
| Hard Reset      | git reset --hard HEAD~1            | Remove commit + all changes                      |
| Clean Untracked | git clean -fd                      | Delete untracked files and folders               |


| Purpose              | Command                              | Description                               |
|----------------------|---------------------------------------|-------------------------------------------|
| Compare Files        | git diff                             | Show unstaged changes                     |
| Compare Staged       | git diff --cached                    | Show staged vs last commit                |
| Compare Branches     | git diff branch1..branch2            | Show diff between branches                |
| Show File History    | git log <file>                       | Show commit history for a file            |
| Blame                | git blame <file>                     | Show who edited each line of a file       |


| Purpose         | Command                | Description                            |
|-----------------|-------------------------|----------------------------------------|
| Save Stash      | git stash              | Save uncommitted changes               |
| List Stashes    | git stash list         | Show stash list                        |
| Apply Stash     | git stash apply        | Apply most recent stash                |
| Apply + Drop    | git stash pop          | Apply and remove most recent stash     |
| Drop Stash      | git stash drop         | Delete specific stash                  |
| Clear All       | git stash clear        | Remove all stashes                     |

| Purpose               | Command                                                                                          |
|-----------------------|--------------------------------------------------------------------------------------------------|
| Create Pull Request   | gh pr create --base "base-branch" --head "feature-branch" --title "title" --body "description"  |


## Also have experince with resole merge conflicts.
