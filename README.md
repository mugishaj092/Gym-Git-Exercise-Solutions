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
