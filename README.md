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

