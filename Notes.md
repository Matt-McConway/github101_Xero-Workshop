# <b>Source Control 101</b>

<i>Presented by <b>Suraksha Setty</b> and <b>Luke Ryan</b> (Xero)</i>

---

## Why Use Source Control?
* Tracking of a code base, and collaboration for large teams.
* Many people can work on the same file at once, as the files are replicated
  locally.
* History of who changed what.
* Ease of auditing - accountability for mistakes and attribution for features
  etc.
* Backups - online repository in the cloud, stores any number of versions.
* Removes the need for commented out code when testing features - just make a
  dev branch for a feature. if it doesn't work, you can always revert!
* Automation - especially for deployment of large applications e.g. deploying to
  multiple environments and platforms. Can also be used for linting for errors.

## How?
* Repository - folder containing code
* Commit - transaction for code changes. Time stamped with your name, recorded
  as a hash.

## What is Git?
* A distributed source control method, rather than centralised. This allows
  offline work as connection to a central server is not required!
* Clones a local copy of the codebase.
* Can push code to remote server repository if your changes work.
* Written by Linus Torvalds - in 3 weeks!!!

## What is Github?
* An online implementation of git.
* Allows pull requests and issue creation for social coding.
    * Include people in projects.
    * Submit changes.
    * Tag people.
    * Teaching/learning platform.
* Strong open source community!
* Hosts code publicly for free.

## Examples of Git Clients
* Git Bash - Using CLI rather than GUI.
* Github client for Windows/Mac.
* SourceTree.
* Git extensions.

<b>We are using SourceTree and Git Bash in the workshop today.</b>

* SourceTree has a GUI.
* gitbash use a CLI.

## Creating a Repository
1. Log in, then go to https://github.com/new
2. Enter the repository name.
3. Enter a description.
4. Specify whether the repository is public or private.
5. Initialize it with a README to save creating one later.
6. Add .gitignore items and a license if applicable.
7. Finally click create repository.

## Cloning
The URL for cloning repository is found on github. Use the green clone/download
button when on the github page for that repository.

### Using SourceTree to Clone:
* Use the url to clone the repository e.g.
  https://github.com/Matt-McConway/github101_Xero-Workshop.git
  (usually there will be a button to clone the repository).



### Using Git Bash to Clone:
    git clone https://github.com/Matt-McConway/github101_Xero-Workshop.git

## Commits
* Each commit has a unique hash.
* Saves changes to many files.
* Represents a piece of work from one person. (Contained in the hash alongside
  a timestamp).
* Can comment on changes. It is good practice to include:
    * Issue numbers.
    * What was changed.
    * Files that were changed.
    * Goals of the change.
* A diff shows the changes made by that person (+ and -'s) from additions,
  removal and changes made within the files.

<b>How commits work:</b>

Working directory --(git add)--> staging area --(git commit)--> repository

The staging area is where the files that are staged for the commit. Useful for
triple checking changes.

### Making a Commit in SourceTree:
* Make the change.
* Add to staged area.
* Make sure you add a description!
* Then commit the change to the repository.


### Making a Commit with Git Bash:
    git status
* Shows that working tree is clean, or lists changes otherwise.


    git add .
* To add everything or use git add --all or git add *


    git status
* Should now show the changes that will be committed. They should be in green
  rather than red.


    git commit -m "Commit message"
* Commit the change to the repository. The commit message is the description of
  the changes you made.

<b>Once the file(s) have been committed, you then need to push them to the
repository!</b>


## Push

### Pushing Changes with SourceTree
1. In the toolbar there is a button named push.
2. Clicking that you can choose branch, etc.
3. Then click push again to push your changes to the repository.


### Pushing Changes with Git Bash
    git push origin master
* Origin is the name of the remote, that is the alias for the local version of
the repository.
* Master is the name of the branch. You can name branches whatever you like.


## Forking a Branch
* Isolated server-side copy of the repository.
* Control permissions by allowing users to only push to certain branches.
* E.g. origin - this is a fork name used in the Git Bash command used earlier.
* Useful for customizing software by forking other peoples projects, or testing
  features or just for security/permission reasons.

## Pull Requests
* Request to pull changes from our fork back into the master repository.
* Internally Xero uses this for code reviews by other programmers to test the
 code and suggest changes to your changes.
* Keep your pull requests small - limit changes to ~5 to make your changes easy
  to review for others.
  * Nobody wants to check 100+ file changes!
* Can be many commits. Commit for incremental change and submit a pull request
  when you have made a significant change you want to integrate back into the
  codebase.
* Can tag people and ask them to check/talk with them about your code.
* Anyone can comment on public repos, people will often help or teach you
  things!

## Merging and Conflicts
* Merges and conflicts need to be resolved before a branch is integrated.
* Git needs your input, if two people change the same lines or file for
  something. i.e. It needs to know which changes it should use.

## Branching
* Master branch is the production/base/stable version of your code.
* Can branch for features and/or different release versions.
* The main thing is to be consistent!

## Further Resources
* https://try.github.io/
* http://gitimmersion.com/
* https://git-scm.com/book/en/v2/Getting-Started-Git-Basics
* http://gitref.org/
