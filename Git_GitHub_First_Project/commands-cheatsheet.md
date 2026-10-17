# Git Commands Cheat Sheet

| Command | Easy meaning |
|---|---|
| `git --version` | Check that Git is installed |
| `git config --global user.name "Your Name"` | Set the author name for commits |
| `git config --global user.email "you@example.com"` | Set the author email for commits |
| `git init` | Start a new local repository |
| `git status` | See what changed and what is staged |
| `git add index.html` | Put a file's current changes into the staging area |
| `git add .` | Stage changes in the current directory (review status first) |
| `git diff` | Inspect unstaged changes |
| `git diff --staged` | Inspect staged changes |
| `git commit -m "message"` | Save a snapshot of staged changes |
| `git log --oneline` | View compact commit history |
| `git branch` | List local branches |
| `git branch -M main` | Rename the current branch to `main` |
| `git clone URL` | Copy a remote repository to your computer |
| `git remote -v` | Show configured remote repositories |
| `git push -u origin main` | Upload local branch commits to GitHub and set upstream |
| `git pull` | Fetch and integrate remote changes into the current branch |

## Remember the four places

1. **Working directory** — files you edit.
2. **Staging area** — changes selected for the next commit.
3. **Local repository** — commits saved on your computer.
4. **Remote repository** — commits shared on GitHub.

Typical cycle:

```text
Edit file → git status → git diff → git add → git commit → git push
```

A commit is a local checkpoint. `git push` publishes commits to the remote repository.
