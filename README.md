# git-tricks
A collection of git tricks/commands I find useful


## Deleting git commit history, while keeping the repo
[Source](https://stackoverflow.com/questions/9683279/make-the-current-commit-the-only-initial-commit-in-a-git-repository)
```
rm -rf .git
git init
git checkout main
git add .
git commit -m "Removed history"
git remote add origin github.com:yourhandle/yourrepo.git
git push -u --force origin main
```
