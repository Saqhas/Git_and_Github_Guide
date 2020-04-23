# **GIT & GITHUB GUIDE**

## **CREATING A GITHUB REPOSITORY** :-
   - ###  Creating a New Repository
    - `git init name_of_repository`
   - ### Make a Existing Folder Repository
    - Step 1 ->  `cd into the Folder`
    - Step 2 ->  `run git init`


## **CHECKING THE STATUS OF THE REPOSITORY** :-
  - `git status`

## **ADDING FILES TO THE STAGING AREA** :-

- ### Adding all files in single Step(use any one of these)
    - `git add --all`
    - `git add "*"`
- ## Adding files one by one
    - `git add file_name`
- ## Adding files more than one but selected
    - `git add file_name1 file_name2`

## **COMMITING THE CHANGES** :-
- ### With the commiting message in one line
    - `git commit -m "commit message"`
- ### Write the commiting message in the Git Default editor
    -  `git commit`
- ### Change a commit message
	- `git commit --amend`

## **Dropping all teh changes done after a pull.** :-
- `git stash`

## **Git Log**
- ### View Log
- `git log`

## **Git Branch**
- ### Make Branch/Reset/Checkout
- #### New Branch
- `git branch new_branch_name`
- #### Git checkout to new branch
- `git checkout new_branch_name`
- #### Check in which branch you are in now type->
- `git branch`
- #### Reset Commit  //this can be used to a previous commit in your history
- `git reset SHA`

## **Git Clone**
- `git clone remote_location clone_name`
- ### List of Git's project's remote->
- `git remote -v`
- ### Git Fetch
- `git fetch`
- ### After Git Fetch we merge local master to remote master
- `git merge origin/master`
- ### Change the remote url
- `git remote set-url <url>`

## **Get the Remote Url**
- `git config --get remote.origin.url`

## Get just one file from different Branch
- `git checkout experiment -- app.js`

## Replace master with a branch
- ### On local
	- `git checkout feature_branch`
	- `git merge -s ours --no-commit master`
	- `git commit      # Add a message regarding the replacement that you just did`
	- `git checkout master`
	- `git merge feature_branch`
- ### To rewrite local branch
	- `git branch -f master dev_branch`
- ### To rewrite remote branch
	- `git push remote +dev_branch:master`

## Remove a branch
- `git push --delete origin <branch_name>`
- `git branch -d <branch_name>`

## Adding the description to a git branch
- `git config branch.<branch-name>.description` "<description message>"

## View the description of a branch
- `git config branch.<branch-name>.description`

## List all the information of the remote
- `git remote <remote-name> show`

## List info of all the branches
- `git branch -a`

## List all the remote branches
- `git branch -r`

## List all the remote refs
- `git ls-remote origin`

## Problems 
- **If the branch is in remote branches but you are not able to checkout, then it means that it is not added in Local refs**
- **Solution:** Add the remote branch in local refs using this command: `git branch <branch-name> <remote-name>/<branch-name>`
## Study Images->

![Alt text](https://raw.github.com/shauryauppal/Git_and_Github_Guide/master/Git%20Guide/1.jpg)

![Alt text](https://raw.github.com/shauryauppal/Git_and_Github_Guide/master/Git%20Guide/2.jpg)

![Alt text](https://raw.github.com/shauryauppal/Git_and_Github_Guide/master/Git%20Guide/3.jpg)

![Alt text](https://raw.github.com/shauryauppal/Git_and_Github_Guide/master/Git%20Guide/4.jpg)

![Alt text](https://raw.github.com/shauryauppal/Git_and_Github_Guide/master/Git%20Guide/5.jpg)

![Alt text](https://raw.github.com/shauryauppal/Git_and_Github_Guide/master/Git%20Guide/6.jpg)

## Thank You

