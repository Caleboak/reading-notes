## All about Git and its commands
### What is Git?
##### Git is a version-control system for tracking changes in computer files and coordinating work on those files among multiple people. Git is a Distributed Version Control System. 

-Git helps you keep track of the changes you make to your code: Git keeps the history of changes made on a file. If you make errors, you can easily back track through the history of changes to find any error

-Git also helps you synchronise code between multiple people: If a group of people are working on the same project file. Git can take all the changes and add them to the master branch. This way everyone is working with the most recent changes.

### Fundamentals of a git workflow
#### Local Repo
#### Remote Repo
#### Staging Area
#### Working Directory

*A file in your working directory can be staged(files are added to the staging area, but not commited), modified(files with the updated changes are not yet stored in the local repo ) or commited(files are now stored in your local repo and are ready to be pushed to your remote repo)*

## Command and its uses
#### Git add - adds files to the staging area, *git add .* adds all the updated file to the staging area
#### Git commit - adds those files to the local repo. *git commit -a -m 'message'* - a stands for all and m stands for the message attached to the commit, usually you want to add what changes you made.
#### Git push - adds all the committed files from the local repo to the remote repo. Without the push command, the changes wont be made on the remote server, just the local repo. *git push origin master* - origin is the name of the remote and master is the branch you are pushing to
#### Git fetch - gets the files from the remote repository to the local repository but not into the working directory.
#### Git merge - gets the files from the local repo and merges it to the working directory.
#### Git pull- is command used to get files from the remote repository directly into the working directory. It is equivalent to a git fetch and a git merge .

## Steps to get all of this working
#### Get github and git downloaded
#### Tell git your details --  git config --global user.name "YOUR_USERNAME"   git config --global user.email "your email"   git config --global --list 
#### Create a repo on github
#### cd into the directory for your working directory
#### touch README.md to create a read me file and then *git init* - if you created the files from repo, skip this
#### *git status*- to check the status
#### After making changes on the file *git add .* to update all changes to the staging area
#### *git commit -a -m "message"* so all other collaborators can see your changes
#### *git reset HEAD~1* incase you made an error and what to retract your last commit
#### *git remote add origin 'remote_repository_URL'* - sets the new remote
#### *git push -u origin master* - pushes changes to origin

*Notes*
##### *git diff* To show the files changes not yet staged
##### *git checkout .*  Revert back to the last committed version to the Git Repo
##### *git clone 'Remote Repo URL'* - to download the repo from remote to your working directory
##### *git pull origin master* - to make sure you get the most recent change from the master branch. Useful for collaborative projects
