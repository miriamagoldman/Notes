# Git_notes


Git is a way of keeping track of verision control when many people are working on the same code, or for yourself. The README.md document is the document that appears in the git folder and displays automatically. In order to work in git first you have a git account and make a repository. Then you clone the repository with the command below.

```bash
$ cd ~/git
$ git clone git@github.com:miriamagoldman/Notes.git
$ cd Notes
```
This makes a clone of the folder on git on the computer. This will be a copy of the master branch from git. In order to work with that code but not change the actaul code. You can make a new branch from that branch. 

```bash
$ git branch note_branch
```
This command makes a new branch for you to work with locally. Next a new fork is made to make a new place to put whatever changes will be made locally, this is done with the command. 

```bash
$ git remote add note_fork git@github.com:miriamagoldman/Notes.git
```
To make sure that worked you can use the command,

```bash
$ git remote -v
```
. 
As well as anytime to check up on status the command, 

```bash
$ git status
```
, can be used.

Now in order to actually change the code move the folder to your branch. 

```bash
$ git checkout note_branch
```
Make whatever changes that need to be made and when ready use command add to add the document to git. Then use commit to commit it, and last push it from your branch with your fork to make sure it does not change the master in the cloud.  

```bash
$ git add ~/git/Notes/git_notes.Rmd
$ git commit -m "Adding R Markdown git notes"
$ git push note_fork note_branch
```
Then finally you can request to put the changes to the real document through git hub. 
sys.call
