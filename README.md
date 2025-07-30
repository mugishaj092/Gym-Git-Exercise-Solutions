# Bundle 1
## Exercise 1

```bash
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
Initialized empty Git repository in /Users/walmond/Documents/The-gym/Gym-Git-Exercise-Solutions/.git/

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git branch -m main

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git add -A

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git commit -m "Initial commit"
[main (root-commit) 12e3e14] Initial commit
 1 file changed, 11 insertions(+)
 create mode 100644 index.html

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git remote add origin https://github.com/mugishaj092/Gym-Git-Exercise-Solutions.git

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 372 bytes | 186.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/mugishaj092/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git branch dev
 
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git checkout dev
Switched to branch 'dev'

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git branch test
   
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git checkout dev  
Already on 'dev'

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git branch -D  test
Deleted branch test (was 12e3e14).

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % 
```


## Exercise 2
```bash
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash list   

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash push -u -m "Will remove home page file"

Saved working directory and index state On main: Will remove home page file

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash list                                   
stash@{0}: On main: Will remove home page file

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash push -u -m "Will remove about page file"
Saved working directory and index state On main: Will remove about page file

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash push -u -m "Will remove team page file"
Saved working directory and index state On main: Will remove team page file

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash list
stash@{0}: On main: Will remove team page file
stash@{1}: On main: Will remove about page file
stash@{2}: On main: Will remove home page file

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash pop stash@{1}
Already up to date.
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{1} (802515d43addcee23c208cc8f32b1311344a6f24)

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash list         
stash@{0}: On main: Will remove team page file
stash@{1}: On main: Will remove home page file

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash pop stash@{1}
Already up to date.
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{1} (32659abfd40b80cfa9921936da4471564bdc3a74)

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git add .

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git commit -m "Will add about and home pages"
[main 6144d3c] Will add about and home pages
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 534 bytes | 534.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/mugishaj092/Gym-Git-Exercise-Solutions.git
   da87ba5..6144d3c  main -> main

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git stash pop                                
Already up to date.
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped refs/stash@{0} (0a17ea707401ce3b9a9e14feb376e61734cd8bb3)

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git reset --hard
HEAD is now at 6144d3c Will add about and home pages
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % 
```

# Bundle 2
## Exercises 1

```bash
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git add .                  

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git commit -m "Will add service page"
[ft/bundle-2 ab6ff90] Will add service page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % git push -u origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 436 bytes | 436.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/mugishaj092/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/mugishaj092/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
walmond@Walmonds-MacBook-Pro Gym-Git-Exercise-Solutions % 
```