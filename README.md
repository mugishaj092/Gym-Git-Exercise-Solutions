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

## Exercises 2

```bash
 1117  git checkout main
 1118  git pull
 1119  git checkout ft/service-redesign
 1120  git checkout -b ft/service-redesign
 1121  git add .
 1122  git commit -m "Will add some changes in service.html"
 1123  git push -u origin ft/service-redesign
 1124  git checkout main
 1125  git add .
 1126  git commit -m "Will add some changes in service.html against created PR"
 1127  git push
 1128  git checkout ft/service-redesign
 1129  git diff
 1130  git log --oneline
 1131  git diff main ft/service-redesign
 1132  git merge main
 1133  git add .
 1134  git commit -m "Will solve the conflict which was caused by the change i made on main"
 1135  git push
```

# Bundle 3
## Exercises 1

```bash
 1149  git checkout -b ft/team-page
 1150  git add .
 1151  git commit -m "Will add team page and it's content"
 1153  git push -u origin ft/team-page
 1154  git checkout main
 1155  git branch ft/contact-page
 1156  git checkout ft/team-page
 1157  git log
 1158  git checkout ft/contact-page
 1159  git cherry-pick 857f0699fa5f107ccaec1b9b4cdf4b648fd0f595
 1160  git status
 1161  git push -u orgin ft/contact-page
 1162  git push -u origin ft/contact-page
 1163  git checkout -b ft/faq-page
 1164  git add .
 1165  git commit -m "Add faq page"
 1166  git push -u origin ft/faq-page
 1167  git log
 1168  git revert 857f0699fa5f107ccaec1b9b4cdf4b648fd0f595
 1169  git push -u origin ft/faq-page
```