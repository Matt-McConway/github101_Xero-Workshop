# Source Control 101

##Why
* Allows tracking of versions of code, and collaborations for large teams

* Can work on the same file at once, as files are replicated locally.

* History of whi changed what

* Ease of auditing - accountability 

* Backups - online repository in the cloud, backs up major versions

* Removes the need for commented out code when testing stuff - just make a dev branch for a feature. if it doesn't work, you can always revert

* Automation - especially regarding deployment for large applications. Linting also. e.g. deploying to multiple environments and platforms

## How

Repository - folder with code
Commit - transaction for code changes. time stamped with your name

## Git
* Distributed source control vs centralised. git is distributed, which allows offline work
* You have a local copy
* Can push to remote server repository if your change works
* Written by Linus Torvalds - in 3 weeks

## Github
* Online version of git
* Pull requests for social coding. Can include people, submit changes
* Strong open source community
* Hosts code publically for free

##Git Clients
Git Bash
Github for windows/mac
source tree
git extensions

Using sourcetree and gitbash today

Sourcetree has a gui, gitbash being CLI 


## Cloning

The url for the repo is found on github. Use the green clone/download button when on the github page

Use GUI to clone: Use the url to repo https://github.com/Matt-McConway/github101_Xero-Workshop.git

usually there will be a button to clone the repo.



bash: git clone https://github.com/Matt-McConway/github101_Xero-Workshop.git

## Commits
* Has a unique hash,
* Saves changes to many files
* Represents a piece of work from one person. Contained in the hash
* Has a comment can include issue numbers, what was changed etc
* A diff shows the changes made by that person + - s from additions, removal changes
* 

Working directiory ---(git add) --> staging area ----(git commit) ----> repository

staging area is where the files that are staged for commit. 

### How to make a change in source tree

* make the change
* Add to staged area
* Make sure you add a description
* Then commit it
* 

### Using CLI

* git status  - shows that working tree is clean (if it is clean, or lists changes otherwise)
* git add . (to add everything) or git add --all  or git add *
* git status (then shows changes that will be commited, so it is in green rather than red)
* git commit -m "Commit message"
*

Once the file(s) have been commited, you then need to 