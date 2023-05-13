# CLASS 03: Revisions and the Cloud
## Using git, github, your Terminal & VScode

[Read Git Intro](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)

### What is git? How does it relate to GitHub?

Git allows sharing of code and collaborations with other people. Git is the version control and GitHub is the online code storage

#### Attributes of git:
- has a version control system
- Multiple developers work on the same code
- keeps a history of changes
- You can view, apply and remove changes
- Keeps all your project files in one repository

#### Version Control
- Each “commit” represents each successive version of a file/files
- It’s a type of “save as.” 
- The first one is commit A, then B, etc
- Head = the label meaning “you are here”
- You can assign messages to commits
- The messages give you a caption for the snapshot

#### What is GitHub?
- Not git
- A way to share code with others
- Online place to store code
- It uses git to manage the teams work with version tracking, reviewing changes and keeping changes separate

#### What is a repository? (repo)
- It is usually just for one project
- Really large projects might have multiple repositories for different parts
- Repo’s can live on github and/or your computer

#### Creating a repo on GitHub
- Create a new repo
- Name it
- Give a description
- Check that it’s public
- Add a README file
- Change the branch from none to main (under Pages/build&deployment)
- Then hit save. Your site is now live

#### Linking Repos
Using git clone
In the terminal:
1. Get yourself into the file you want, i.e. code-102
2. Type: git clone (paste your link from github)

*It will look like this if you did it correctly:*
```
Cloning into 'hello-world'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```
3. Run the command in code-102 "ls" then cd hello-world
4. You should now see ➜  hello-world git:(main) if you did it correctly

- Git commands only work in git repositories
- git remote -v : shows you the github links

### GITFLOW:ACP- ADD, COMMIT, PUSH

- “Git status”: will always show you the update
- “Git add README.md” : to save your files (commit) you can use tab to autocomplete the file name.
- “Git add .” : this saves all the files at once- later on may not want to use this if you have multiple projects/files in process.
- “Git commit -m “message in quotes” ” : we want to make the changes and leave a message (-m)
- “Git push origin main” : this will push our changes up to github cloud
- Every single time you are ready to update github you must go through the ACP process!
- First- “git add (your file to save), then “git commit -m (“with a message of why you made changes”)”, then “git push origin main” to push the changes up to github cloud. Be sure to use git status in between each stage to check for problems.




## Answer
- What is Version Control? 
  -  Version control is a way to track the changes made to files without having to save multiple versions. It saves each change of the file so the user can go back and compare, plus see who made the change.
- What is cloning in Git?
  - Cloning in git means that you are making a copy of the existing Git repository from one server in order to add it to your own project files or wherever you need to place it, so you are able to work on it.
- What is the command to track and stage files? 
  - To track and stage one file you would use the command: "git add filename" 
- What is the command to take a snapshot of your changed files?
  - To take a snapshot of the changed file you would use the command: "git commit -a"
- What is the command to send your changed files to Github?
  - To send your changed files to GitHub you would use the command: "git push origin main"
