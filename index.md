## Welcome to GitHub Pages

Git - Distributed revision control system

## What is GIT?
- VCS - Easy management and collaboration on a project
- Open source
- No centralized connectivity is needed

### A brief history of git

```markdown
In 2002, the Linux kernel project bega used a Distributed VCS called BitKeeper.
In 2005, a commercial company brokedown the free licence of BitKeeper
This prompted the Linux development community to develop their own tool - GIT.
```

### Git Structures

```markdown
- .git
- HEAD/ (A pointer to your current branch)
- config/ (contains all configuration preferences)
- description/ (description of your project)
- Index/ (is used as staging area between working directory and the repo)
- logs/ (keeps the record to changes that are made in ref)
- objects/ (all data are stored here: commits, trees, and tags)
- hooks/ (shell scripts that are invoked after executing a command)
- refs/ (hold your local branch remote branch and tags)
```

### Git Initialization

```markdown
- git init 
- git config –global user.name “”
- git config –global user.email “”
```

### Git basic commands

```markdown
- git init
- git config
- git clone
- git add -p
- git log
- git blame
- git alias
- git status
- git format-patch -1
- git am
- git apply
- patch -Np1 <
- patch -Np1 --dry-run <
- git checkout -b
- git checkout --orphan
- git branch -a
- git reset
- git merge
- git merge conflicts
- git rebase -i
- git fetch
- git pull
- git push
```

### Git Reset

```markdown
--soft: uncommit changes, changes are left staged (index).
--mixed (default): uncommit + unstage changes, changes are left in working tree.
--hard: uncommit + unstage + delete changes, nothing left.
```

### Git add -p

```markdown
- Patch mode allows to stage parts of a changed file, instead of the entire file
```

### Git blame

```markdown
- examine the contents of a file line by line and see when each line was last modified and who the author of the modifications was
```

### Play with Git log

```markdown
- git log -p
- --oneline
- --graph
- --since --until
- --author
```

### Git alias

- Having alias name for the git commands

### Git fetch

1. changes made in the server
2. git fetch in the user
3. git merge origin/<branch>

### Git pull
  
git pull = git fetch + git merge

### Staged to unstaged

Move a changed from staged to unstaged
Using git restore --staged <file-name>

### Git push
  ```markdown
  git push <projectpath> HEAD:refs/heads/<branch>: the local branch commit can now differ from the remote branch commit, because "HEAD" can be detached (not linked to any branch)
git push <projectpath> <branch>: the local branch commit will always be the same as the remote branch commit.

  ```
  
  ### Git LFS
  
```markdown
- Push files larger than 100MB to remote repository
- Git lfs track filename.txt
  
GitHub Free                        2 GB limit
GitHub Pro                         2 GB limit
GitHub Team                        4 GB limit
GitHub Enterprise Cloud            5 GB limit

Check this link for [Reference](https://git-lfs.github.com)

```
