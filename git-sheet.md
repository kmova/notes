## Setting up local version
```
cd <code-base-dir>
git clone <git-project-url>
cd git-project
git config --global user.name "kiranmova"
git config --global user.email "kiran.mova@cloudbyteinc.com"
git config --global core.pager "less -r" 
git config -l
```

## List and switch to remote branch
```
git fetch
git branch -r
git checkout <branch-name>
git branch
```

## Push the modified changes to remote branch
```
git status
git commit -a -m "<comment for checkin>"
git push
```
## Clear dirty/temporary changes
```
git stash
git stash clear
git stash show
```
