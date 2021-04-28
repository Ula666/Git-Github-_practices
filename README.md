# Git-Github-_practices
### Stages of git on local host
### Every project under the distributed version control system Git, goes through three stages — Modified, Staged, and Committed.  
![image](https://user-images.githubusercontent.com/47173937/116371517-6bb00c80-a803-11eb-8068-377b3b71a4a6.png)  

• **Modified:**
In Git we can create a repository, a repository is a directory that contains all the files related to your code. In the repository we can write code, and maintain it. Once, the code is written, anyone willing to make some modification can make those changes in their own remote repository. A remote repository is a local copy (one that you create on your local machine) of the original project that is being maintained via Git. **Basically you can make changes to your copy of the project without hampering the original code. This is called Modification, i.e. making some additions to the original project.**  

• **Staged:**
The second stage in Git, is "staged". We use the commands in the Git command line — `git add .` So, this command tracks the new changes and pushes it to the staging area. The staging area is place prior to the actual implementation of changes (this area contains all the added files that contain new code, which are ready to be joined to the remote repository) All the new files are first pushed to the staging area.
- An analogy example. in a race, before, the race begins, we hear three words, Get, Set…, Go! Now, we can think of ‘Set’ as the staging area. So, this is an indication that make yourself ready, as the race is about to start. Similarly, staging area is a place where all the new files are finally ready to be joined to the remote repository.  

• **Commit:**
This is the final stage, as this stage finally applies the new changes to the remote repository. Looking at the previous analogy, this is your ‘Go’ position. So, a commit is a set of new files that are being added to a project as part of the modification. Each commit represents the changes made to project in the past, with the details about the time at which commit was made and the author of the code. So, finally when you make a commit, and it gets committed, then this simply means that you have successfully applied a certain modification to the code.



## how can you reset/cancel if you have already run git add . command
- there are 3 options in Git to undo your local changes:
- first we can use `git status` to view the changes that have been made in your working directory  
1. Undoing changes with git stash:
- to discard all local changes, but also save them for later use, we can use `git stash` command 
2. Undoing changes with git checkout
- To discard local changes to a file pernamently, we can use `git checkout --<file>`
3. Undoing changes with git reset
- To discard all local changes to all the files pernamnetly, we can do `git reset --hard`   

## what is a git staging area
## workflow and the stages
## git merge and merge conflicts
## best practice to resolve git merge conflicts
## research around best practices of git and git-hub
