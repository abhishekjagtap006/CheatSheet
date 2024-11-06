1. `git config --global user.name "Your Name"` :- Set your name 
2. `git config --global user.email "you@example.com"` :- Set your email
3. `git conifg --global credential.username <username>` :- Configure your remote repository for access
- Staging Area :- Contains changes that will go into next commit
- Working Area :- Changes that are not in staging area. 

4. `git init` :- Initialise Repository 
5. `git status` :- Show all changes since the previous commit 
6. `git add <file|folder` :- Add Changes into staging area
7. `git rm <file|folder` :- Remove changes from working as well as staging area.
8. `git commit -m "message"` :- Create commit
9. `git commit -m "message" --ammend` :- Update previous commit
10. `git log ` :- View Commit History 
11. `git log --all` :- Show all commits (not just current branch)
12. `git log --all --graph` :- Show branching visually in the command line
13. `git reset <file|folder>` :- Remove file from Staging area 
14. `git reset <commit>` :- Allows you to move current branch's HEAD to a specified state in commit history 
15. `git branch` :- Shows list of available branches
16. `git branch <branch_name>` :- Create new branch
17. `git branch -D <branch_name>` :- Delete's the branch 
18. `git checkout --<file|folder>` :- Removes changes from working area
19. `git checkout <commit_hash|branch>` :- Switch to particular commit or branch 
20. `git checkout <hash|branch> <file|folder>` :- Restore the contents to given commit
21. `git merge <branch_name> -m "message"` :- Merge the current branch(indicated by HEAD -> with another branch <branch_name>. Saves the result of the merge as a commit on the current branch)
- To Resolve a merge conflict
	- Delete all extra code and just leave the final code that you want, if there are conflicts in multiple places in your code, repeat the same for all the places
	- Create a commit
- Conflicts in feature branch workflow
	- Get the latest updates from main
	- Get the latest updates from feature branch 
	- Merge main into the feature branch. Notice the direction of the merge. we want the merge commit to stay on feature branch so our teammates can review it 
	- Push the resolved feature branch to GitHub 

22. `git diff <file|folder>` :- Shows changes between working area and staging area
23. `git diff --staged <file|folder>` :- Shows changes between working area and previous commit 
24. `git tag <name> <commit>` :- Create a tag at specific commit 
25. `git tag -a <name> <commit>` :- Create a named tag object
26. `git tag -d <name>` :- Remove a tag from local repository 
27. `git revert <commit>` :- Creates a new commit, reverting changes from the specific commit. It generates an inversion of changes.
28. `git stash` :- Put current changes from working directory into stash for later use (both staged and ustaged)
29. `git stash pop` :- Apply stored content into working directory and clear stash 
30. `git stash drop <stash>`  :- Delete a specific stash from all your previous stash 
31. `git stash list` :- List all stash 
32. `git stash clear` :- Clear all stash  
33. `git rebase <branch_name>` :- Apply commits of the current working branch and apply them to the HEAD of branch to make the history of yoru branch more linear. 

34. `git remote add <remote_name> <url>` :- Link a local repository to a remote repository and give a name for this link
35. `git remote` :- List all remote repositories that are linked
36. `git remote -v` :- More Detail i.e verbose
37. `git remote remove <remote_name>` :- Removes a link to a remote repository 
38. `git clone <url>` :- Download a remote repository from URL.
39. `git clone <url> <folder_name>` :- Download Repository and give it a different folder name
40. `git fetch` :- Updates all remote tracking branches. 
41. `git push <remote_name> <branch>` :- Upload a branch of your git version to git remote repository 
42. `git push <remote_name> <branch> -f` :- Force-Push branch to remote repository 
43. `git pull <remote_name> <branch>` :- Update local branch with any updates from the remote repository 


