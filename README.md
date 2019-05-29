# Bash Scrips

#### making a script executable from any directory
- save with no extension
- make file executable
- add to path
eg 
$ export PATH=$PATH:'/c/Users/User/Programming/Bash-Workspace/BashScripts/'

# iuvo
A script to automate common git operations

## Functions
#### begin 
Performs initial set up of local repo and makes first commit to remote.
- Makes a directory at current location
- Calls git init
- Adds blank README
- Adds blank .gitignore
- Asks user for remote location and calls git remote add origin with this
- Stages changes
- Makes initial commit with message "Initial Commit"
- Calls git push -u origin master

#### update
Stages all changes, commits changes, option to push these to current branch.

#### help
Provides user with some documentation

# Git Log Graphs
can call 
	git log --graph

for pretty git log graph in bash
insert the following into .gitconfig file (found in home directory)
[alias]
	lg = !"git lg3-specific --all"
	lg3-specific = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset) %C(bold cyan)(committed: %cD)%C(reset) %C(auto)%d%C(reset)%n''          %C(white)%s%C(reset)%n''          %C(dim white)- %an <%ae> %C(reset) %C(dim white)(committer: %cn <%ce>)%C(reset)'

