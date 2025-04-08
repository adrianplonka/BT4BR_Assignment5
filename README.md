# BT4BR_Assignment5 

**Adrian Plonka**

Date: **08.04.2025**   
*Repository for* **BT4BR** Assignment#5


## *Mini* Git Guide

![Like emote](images/gitimg.png)

## Table of contents
 - [First file](#Adding-your-first-file)
 - [Branching](#Branching)
 - [Summary](#Summary-and-other-useful-git-commands)
 
***

### Adding your first file


```bash
touch Hello_World.py
```

 > This command will create a Hello_World.py file
 > Now you edit this file with editors like gedit, nano etc.
 
 ```bash
 gedit Hello_World.py
 ```
 
 > Now you have to use *git add* command to add your script to the **staging area**
 
 ```bash
 git add -u "Hello_World.py"
 ```
 > Now you have to commit your changes
 > - *git commit* 
 > - *-m* flag to name your commit
 
 ```bash
 git commit -m "My first commit"
 ```
 
 > Finally you will push changes to GitHub repository
 
 ```bash
 git push origin
 ```
 
### **Good Job!**  
 **You have succesfully added your first python script to your repository!**
 
 ***
 
 ***
 
### Branching 

Branching allows to diverge from the main branch. After that you can merge your branches (*beware merging conflict*) or if you like your new branch you can make it the main one!

1. Create a new branch

```bash
git branch new_branch
```

2. Change workplace to the *new_branch*

```bash
git checkout new_branch
```

> Now you are working in the *new_branch*
>> Try editing a file, for example *Hello_World.py*
>> Just add some additional code such as 
>```python
>print("This is your new branch")
>```
> After that push the changes to GitHub

3. After commiting and pushing, compare your 2 branches

```bash
git diff main..new_branch
```

4. Go back to the main branch and merge *new_branch* to *main* 

```bash
git checkout main
git merge new_branch
git push origin
```

- Now your *main* branch contains changes made in *new_branch*

***

## Summary and other useful git commands

1. Configuration
 - `git config --global user.name "Your Name"` - set your Git username
 - `git config --global user.email "your.email@example.com"` - set your Git email address.
2. Basic commands
 - `git clone [url]` - clone an existing repository from GitHub
 - `git add [file]` - add a file to the staging area
 - `git add .` - add **all** changes to the staging area
 - `git commit -m "name of your commit"` - commit changes in that are currently in the staging area and name your commit
 - `git push origin` - push your commits to repository on GitHub
 - `git pull` - pull changes from remote repository to local machine
 - `git log` - display commit history
 3. Branching
 - `git branch` - list all branches
 - `git branch [branch name]` - create a new branch
 - `git checkout [branch name]` - move to a particular branch
 - `git merge [branch name]` - merge a branch into the current branch
 - `git fetch` - download changes from repository on GitHub without changing (merging) local repository
 
##**That's it, now you can work with GitHub**  
## Good luck!

***











 
 
 
 
 
 
