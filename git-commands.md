# Notes for Class 3 (6/3/20)


## Git Commands


### Setting up a Git Repository


**Importing**
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

1.Switch to the target project’s directory
  -  Example:
`$ cd test (cd = change directory)`
1. Use the git init command
`$ git init`
_Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced._


To start **tracking** these repository files, perform an initial commit by typing the following:
1. `$ git add *.c`
1. `$ git add LICENSE`
1. `$ git commit -m “any message here”`
Now, your files are tracked and there’s an initial commit. 


### Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

`$ git clone https://github.com/test`

By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project. The command also automatically checks out — or retrieves for editing — a copy of the newest version of the project.

**To clone a repository into a directory with another name of your choosing, use the following command format:**

`$ git clone https://github.com/test mydirectory`
The command above makes a copy of the target repository in a directory named “mydirectory.”

### Local Repository Structure
The local Git repository has three components:

- **Working Directory**: The actual files reside here.
- **Index**: The area used for staging
- **Head**: Points to the most recent commit

### Saving Changes
**All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.**

- Tracked
  + Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

- Untracked
  + Untracked files were not in the last snapshot and do not currently reside in the staging area.

**After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.**

### The Life Cycle of File Status
1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
1. You stage the modified file.
1. Then, you commit staged changes.

### Check File Status
**To determine the state of files, utilize the git status command:**

- $ git status
  + On branch master

`nothing to commit, working directory clean`

**This information indicates which branch you’re on and states “working directory clean,” which means that files have tracked or modified status at the moment. Also, no untracked files are present because Git has not listed any.**


### Tracking and Staging a New File
**Single File**
Track one file only by using the following format:

`git add filename`
All Files

Track all files in a repository by using the following command:

`$ git add *`
**After using these commands, files are tracked and staged for committing.**

After adding a new file called EXAMPLE, you would see information regarding changes to be committed when using the git status command:

`$ git status`

On branch master

Changes to be committed:

  (use `git reset HEAD (file)` to unstage)
new file: EXAMPLE
This information tells us that there are changes to be committed and that the file has been staged.

Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:

`$ git commit -m “made change x,y,z”`
**This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.**

Committing All Changes
`$ git commit -a`
**This command commits a snapshot of all modifications to tracked files in the working directory.**

Pushing Changes
Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

Example:

`$ git push origin master`
**This command pushes changes from the local “master” branch to the remote repository named “origin”.**

*For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.
             
- Stashing Changes
**When you are not ready to commit changes but do not want to lose them either, git stash is a great option. This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the git stash apply command to retrieve the hidden changes.**

- Remote Repositories
**In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.**

- Cloned Repositories
**For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.**
