# Bundle 1
## Exercise 1

```bash
git init
git branch -m main
git add -A
git commit -m "Initial commit"
git remote add origin https://github.com/mugishaj092/Gym-Git-Exercise-Solutions.git
git push -u origin main
git branch dev
git checkout dev
git branch test
git checkout dev
git branch -D test 
```


## Exercise 2
```bash
git stash list
git stash push -u -m "Will remove home page file"
git stash list
git stash push -u -m "Will remove about page file"
git stash push -u -m "Will remove team page file"
git stash list
git stash pop stash@{1}
git stash list
git stash pop stash@{1}
git add .
git commit -m "Will add about and home pages"
git push
git stash pop
git reset --hard
```

# Bundle 2
## Exercises 1

```bash
git checkout -b ft/bundle-2
git add .
git commit -m "Will add service page"
git push -u origin ft/bundle-2
```
