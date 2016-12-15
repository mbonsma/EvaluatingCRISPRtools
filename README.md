# EvaluatingCRISPRtools
A repository for code and documentation for the manuscript "Evaluating Tools for Metagenomic Analysis of CRISPR loci".

The manuscript text can be found [here](https://github.com/mbonsma/EvaluatingCRISPRtools/tree/master/manuscript).

## How to contribute

### On your first visit

* **Fork** this repository by clicking the 'Fork' button in the top right corner of the page. This creates your own copy of the repository on GitHub.
* **Clone** your forked copy of the repository. On the main page of the repository (`github.com/yourusername/EvaluatingCRISPRtools`), click the green 'Clone or download' button on the right. Copy the link under 'Clone with HTTPS'. In your favourite command line tool (I recommend Git Bash if you're on Windows), navigate to a directory in which you want this project to live. Once there, type the following command, where `mbonsma` is replaced with your GitHub username.
```
git clone https://github.com/mbonsma/EvaluatingCRISPRtools.git
```
You now have a copy of your fork on your local machine, where you can make changes to it. 

* Type `ls` to confirm that the `EvaluatingCRISPRtools` folder was created. Then `cd Evaluating CRISPR tools` to enter the folder, and check the status with `git status`.

* Add a reference to the original repo with the following command:
```
git remote add upstream https://github.com/mbonsma/EvaluatingCRISPRtools.git
git fetch upstream
```

### Making changes
When you make local changes to anything in the `EvaluatingCRISPRtools` folder, git will notice the changes you've made and allow you to track them.
* The following cycle of commands is what you'll use to add your changes to git's record.
```
git status #shows any unsaved changes, newly added changes, etc.
git add <filename> #stages changes to that file to be committed
git commit -m "A description of your change" #saves your changes to history with a descriptive message
```
* After you've made changes, sync them with your fork on GitHub by typing 
```
git push origin master
```
* To sync your changes with the original repository, submit a Pull Request *from* your GitHub account *into* `mbonsma/EvaluatingCRISPRtools`. Check [the GitHub help on Pull Requests](https://help.github.com/articles/using-pull-requests/).


**Note**: It's best to create a new branch for each pull request you make.  For
example, if you want to clean up some bits of the repo, you can follow a
workflow such as this:

```
## Good to name the branch to reflect what you are doing.
git checkout -b cleaningUp 
## Make edits/changes/cleaning up
git add files-changed
git commit
git push origin cleaningUp
```

You can now make a pull request **of the `cleaningUp` branch**.  Once the pull
request has been completed, you can delete the now old branch via:

```
git checkout master ## Move back to main branch
git branch --delete cleaningUp
## If you want to delete the remote branch too do:
git push origin --delete cleaningUp
## Update your main branch from the new upstream branch
git pull upstream master
```

Instructions modified from [UofTCoders](https://github.com/UofTCoders/studyGroup/blob/gh-pages/CONTRIBUTING.md).
