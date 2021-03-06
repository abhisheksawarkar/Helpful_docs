## GIT COMMANDS

git init .		-> Make a new folder and write
				This initializes the git repository.

git status		-> Gives status about the directory

git add 'filename'	-> Add the filename to staging area. Not committed yet!

git commit -m 'message'	-> Commits to changes. -am will add and commit with a message.

git diff 'filename'	-> will find what new is added in the file. This will be before the commit.

git log			-> Will find previous commits and changes.

**Branches**

When working on the code, when the thing is working properly and we want to test out some changes,
we branch out from the main code, test the new thing. If it works, we merge it with the earlier master branch.
Code from one branch does not get mixed with code from other branch.
Great for collaborative working.


git branch 'branch_name'-> Will make a new branch with name branch_name

git branch		-> Will print name of created branches.

git checkout 'branch_name' -> Will shift to other branch.


**Merging**

After developing various branches, we need to merge it in a single code base.


git checkout 'master'	-> Go to master branch

git merge 'branch_name'	-> branch to merge with

git branch -d 'branch_name'	-> Deletes the branch

**Reverting**

To revert to committed changes

git reset --hard <Hash>	-> Will DELETE all other commits and change to Hash commit.

git checkout <Hash>	-> Will only checkout the commit instead of deleting the other commits.

git checkout master 	-> To go back to the master branch

**Remote repo**

git remote 	-> List remote repository

git remote -v	-> List repo with url

git remote add <name> <url>	->  name:- shortcut for url,	url:- repo link from github 

git remote <name> --all		-> uploads all branches to remote repository


## Tmux Commands

**_CTRL + b, then ?_** - List all key bindings. 

CTRL + b, then c - Create new window.
CTRL + b, then , - Rename window.
CTRL + b, then n - Move to the next window.
CTRL + b, then p - Move to the previous window.
CTRL + b, then & - Kill current window.
CTRL + b, then % - Split current pane into two (vertically).
CTRL + b, then " - Split current pane into two (horizontally).
CTRL + b, then o - Switch to next pane.
CTRL + b, then q - Show pane numbers (then type a # to switch to it).
CTRL + b, then d - Detach from current session.

tmux list-sessions - List existing tmux sessions.
tmux new -s session-name - Create a new tmux session named session-name.
tmux attach -t session-name - Connect to an existing tmux session named session-name.
tmux switch -t session-name - Switches to an existing tmux session named session-name.


## Bash Commands
Reducing current directory address size in Bash: PS1='\u:\W\$ '
