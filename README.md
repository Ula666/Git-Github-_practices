# Git/Github practices
## Stages of git on local host
- Every project under the distributed version control system Git, goes through three stages — Modified, Staged, and Committed.  
![image](https://user-images.githubusercontent.com/47173937/116371517-6bb00c80-a803-11eb-8068-377b3b71a4a6.png)  

• **Modified:**
In Git we can create a repository, a repository is a directory that contains all the files related to your code. In the repository we can write code, and maintain it. Once, the code is written, anyone willing to make some modification can make those changes in their own remote repository. A remote repository is a local copy (one that you create on your local machine) of the original project that is being maintained via Git. **Basically you can make changes to your copy of the project without hampering the original code. This is called Modification, i.e. making some additions to the original project.**  

• **Staged:**
The second stage in Git, is "staged". We use the commands in the Git command line — `git add .` So, this command tracks the new changes and pushes it to the staging area. The staging area is place prior to the actual implementation of changes (this area contains all the added files that contain new code, which are ready to be joined to the remote repository) All the new files are first pushed to the staging area.
- An analogy example. in a race, before, the race begins, we hear three words, Get, Set…, Go! Now, we can think of ‘Set’ as the staging area. So, this is an indication that make yourself ready, as the race is about to start. Similarly, staging area is a place where all the new files are finally ready to be joined to the remote repository.  

• **Commit:**
This is the final stage, as this stage finally applies the new changes to the remote repository. Looking at the previous analogy, this is your ‘Go’ position. So, a commit is a set of new files that are being added to a project as part of the modification. Each commit represents the changes made to project in the past, with the details about the time at which commit was made and the author of the code. So, finally when you make a commit, and it gets committed, then this simply means that you have successfully applied a certain modification to the code.


## How can you reset/cancel if you have already run git add . command
- there are 3 options in Git to undo your local changes:
- first we can use `git status` to view the changes that have been made in your working directory  
1. Undoing changes with git stash:
- to discard all local changes, but also save them for later use, we can use `git stash` command 
2. Undoing changes with git checkout
- To discard local changes to a file pernamently, we can use `git checkout --<file>`
3. Undoing changes with git reset
- To discard all local changes to all the files pernamnetly, we can do `git reset --hard`   

## Git staging area
- Imagine a box. You can put stuff into the box. You can take stuff out of the box. This box is the staging area of Git. You can craft commits here. Committing is like sealing that box and sticking a label on it. The contents of that box are your changes. 
- ![image](https://user-images.githubusercontent.com/47173937/116440698-a5573680-a848-11eb-8546-5beedc540b49.png)

## Git merge and merge conflicts
- `git merge` command is used to merge the branches
- we can use it to merge the specified commit to currently active branch
- or, to merge commits into the master branch
- or, merge the whole branch in another branch  
- Git Merger Conflict - When two branches are trying to merge, and both are edited at the same time and in the same file, Git won't be able to identify which version is to take for changes. If such a situation occurs, it stops just before the merge commit so that you can resolve the conflicts manually.  
- first we can try `git fetch orgin` and `git pull orginin master`
- if the conflic is still there we can use GIT GUI `git mergetool`  

## Best practices of git and git-hub
- Don’t leak secrets into source control - Secrets, or secret keys or secret credentials, include things like account passwords, API keys, private tokens, and SSH keys. You should not check them into your source code. Instead, we recommend you inject secrets as environment variables externally from a secure store.
- Commit early and often - It would be best if you commit your changes early and often. Early commit helps to cut the risk of conflicts between two concurrent changes. Additionally, having periodic checkpoints means that you can understand how you broke something.
- Write useful commit messages - Creating useful commit messages is one of the best things you can do every day.
The right commit message helps other developers in many ways. They can understand the code better even without looking at it.  
