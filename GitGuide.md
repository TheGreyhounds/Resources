# A Guide to git and its Common Commands
This list is nowhere near complete, but it includes the commands you'll be
using most with git. To understand the context behind these commands,
you also have to understand the workflow of git, and so I reccommend checking out
[this detailed guide](http://dh.newtfire.org/explainGitShell.html) to get a better
understanding of what it means to stage, commit, and to push our code.

```
git init
```
Initialize git in your current working directory. This directory will be considered the
root of your repository, and any directories above it in the directory tree will be considered
outside of the git repository. I.E, if you used git init in the directory "/home/root/Desktop/my_folder",
then anything created inside "my_folder" will be inside the repository, while anything in the "Desktop"
folder will be outside of the repository.

```
git clone url
```
Clones a git repository from "url" into the current working directory. This is often to
clone repositories from GitHub, and so you can get the repository url by going to the GitHub
page where the repository is hosted, clicking the green button on the right that says "Clone
or Download", and then copying the url to the terminal.

```
git status
```
Gives a comprehensive status of the state of the local repository, i.e. what needs to be staged,
what needs to be committed, etc.

```
git add filename
```
Adds "filename" to the staging area

```
git add --all
```
Adds every file that has not been staged in the the local git repository to the staging area.

```
git diff
```
Shows the DIFFerence between the working directory and the staging area. If nothing has been added
to the staging area since the last commit, this command will show the difference between the code
in the current working directory and the last commit.

```
git diff --staged
```
Shows the DIFFerence between the staging area and the last commit. If no new code has been added
to the staging area since the last commit, this command will show no output, because there is no
difference.

```
git commit
```
Commits all the files added to your staging area to a new commit. It will prompt you for a commit
message in your default text editor.

```
git commit -m "message"
```
Same as the "git commit" command except that it doesn't prompt you with your default text editor for
a commit message, you give it the message in the command. Make sure to include the quotation marks.

```
git log
```
Prints out the repository's history of commits to the terminal, along with their commit messages, author
details, and time of the commit.


# TERMS TO KNOW:
- Working Directory = The stuff on your computer you've been doing that you have staged or commited yet.
- Staging Area = Where you put your code before you want to commit it, so for instance if you write really 2 commits worth of code, you can stage them separately and commit them separately.
- Commit = Git's unit of work. A single commit represents a single significant change to your project, and so each commit is a snapshot of your project, saved as a whole. This allows you to make risky changes knowing you revert your project back to an earlier commit if something goes horribely wrong.
- Repository = Your project, and the history of all its commits
- Local Repository = Your project as it has been updated and changed on your computer. It's updated with the command git pull
- Remote Repository = Your project as it has been updated and changed on a remote server, like GitHub, through the command git push
