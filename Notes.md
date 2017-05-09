# Source Control 101

##Why
* Allows tracking of versions of code, and collaborations for large teams

* Can work on the same file at once, as files are replicated locally.

* History of who changed what

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
* Hosts code publicly for free

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
* git status (then shows changes that will be committed, so it is in green rather than red)
* git commit -m "Commit message"
*

Once the file(s) have been committed, you then need to push them to the repo.


## Push

### Source tree push
* in the tool bar there is a button named push
* Clicking that you can choose branch etc
* Then click push again


### Using Git Bash

* Use git push origin master

## Forks

* Isolated server copy of the repository

* Useful if you don't have permission to push to the remote repository

* E.g. origin - this is a fork name used to the gitbash

* Useful for customising software, or testing features or just for security/permission reasons

##Pull requests

* Request to pull changes from our fork to the master repository
* Internally we use this for code reviews by other programmers to test the code and suggest changes to your changes
* Keep your pull requests small - limit changes to 5 to make your changes easy to review for others. Nobody wants to check 100+ file changes
* Can be many commits. Commit for incremental change and submit pull request when you have made a significant change you want to upload
* Can tag people and ask them to check/talk with them.
* Anyone can comment on public repos, people will often help or teach you things

## Merging and conflicts
* Merges and conflicts need to be resolved
* git needs your input, if two people change the same things

## Branching

* Master branch is the production/base/stable versions
* Can do feature branching, branching for release versions
* Main thing is to be consistent

## Resources
try.github.io
gitimmersion.com
git-scm.com/book/en/Getting-Started_Git-Basics
gitref.org.index.html
