###Useful Git Commands -> Quick Summary 

`git config --global user.name "Your Name"` :- Set your name 
`git config --global user.email "you@example.com"` :- Set your email
`git conifg --global credential.username <username>` :- Configure your remote repository for access

Staging Area :- Contains changes that will go into next commit
Working Area :- Changes that are not in staging area. 

`git init` :- Initialise Repository 
`git status` :- Show all changes since the previous commit 
`git add <file|folder` :- Add Changes into staging area
`git rm <file|folder` :- Remove changes from working as well as staging area.
`git commit -m "message"` :- Create commit
`git commit -m "message" --ammend` :- Update previous commit
`git log ` :- View Commit History 
`git log --all` :- Show all commits (not just current branch)
`git log --all --graph` :- Show branching visually in the command line
`git reset <file|folder>` :- Remove file from Staging area 
`git reset <commit>` :- Allows you to move current branch's HEAD to a specified state in commit history 
`git branch` :- Shows list of available branches
`git branch <branch_name>` :- Create new branch
`git branch -D <branch_name>` :- Delete's the branch 
`git checkout --<file|folder>` :- Removes changes from working area
`git checkout <commit_hash|branch>` :- Switch to particular commit or branch 
`git checkout <hash|branch> <file|folder>` :- Restore the contents to given commit
`git merge <branch_name> -m "message"` :- Merge the current branch(indicated by HEAD -> with another branch <branch_name>. Saves the result of the merge as a commit on the current branch)
1. To Resolve a merge conflict
	1. Delete all extra code and just leave the final code that you want, if there are conflicts in multiple places in your code, repeat the same for all the places
	2. Create a commit
2. Conflicts in feature branch workflow
	1. Get the latest updates from main
	2. Get the latest updates from feature branch 
	3. Merge main into the feature branch. Notice the direction of the merge. we want the merge commit to stay on feature branch so our teammates can review it 
	4. Push the resolved feature branch to GitHub 

`git diff <file|folder>` :- Shows changes between working area and staging area
`git diff --staged <file|folder>` :- Shows changes between working area and previous commit 
`git tag <name> <commit>` :- Create a tag at specific commit 
`git tag -a <name> <commit>` :- Create a named tag object
`git tag -d <name>` :- Remove a tag from local repository 
`git revert <commit>` :- Creates a new commit, reverting changes from the specific commit. It generates an inversion of changes.
`git stash` :- Put current changes from working directory into stash for later use (both staged and ustaged)
`git stash pop` :- Apply stored content into working directory and clear stash 
`git stash drop <stash>`  :- Delete a specific stash from all your previous stash 
`git stash list` :- List all stash 
`git stash clear` :- Clear all stash  
`git rebase <branch_name>` :- Apply commits of the current working branch and apply them to the HEAD of branch to make the history of yoru branch more linear. 

`git remote add <remote_name> <url>` :- Link a local repository to a remote repository and give a name for this link
`git remote` :- List all remote repositories that are linked
`git remote -v` :- More Detail i.e verbose
`git remote remove <remote_name>` :- Removes a link to a remote repository 
`git clone <url>` :- Download a remote repository from URL.
`git clone <url> <folder_name>` :- Download Repository and give it a different folder name
`git fetch` :- Updates all remote tracking branches. 
`git push <remote_name> <branch>` :- Upload a branch of your git version to git remote repository 
`git push <remote_name> <branch> -f` :- Force-Push branch to remote repository 
`git pull <remote_name> <branch>` :- Update local branch with any updates from the remote repository 


#### Reference Documents 
[SuperSimpleDev Cheatsheet](docs/SuperSimpleDev-GitCheatSheet.pdf)
[GitLab-Git Cheatsheet](GitCheatsheet.pdf)
