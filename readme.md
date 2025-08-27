# Git learning repo

Just after installing git, there are some steps, called first-time-setup must be done, like developer email and name. Also it is better to check version

```
git --version

git config --global user.name "sbn amd"
git config --global user.email "sobhan.ahmady133@gmail.com"

git config --list
```

The 'config' used in above code is called a git verb, though if you need some help about a git verb you just need type code below

```
git help config
```
For tracking a local project , just type code below within directory of your project. to discontinue tracking, delete `.git` folder created.

```
git init
```

To check the latest status of project(staged or unstaged files or folders) type code below

```
git status
```

First nothing is staged. though you need add or generally speaking stage latest changes using code below. staging lets you to add changes one by one , and commit multiple times for each change

```
git add .
git add file.c
git add ./newfolder
```

To ignore some files of folders, the `.gitignore` must be created and those files or folders must be written in it.

To unstage a file or dir just use code below

```
git reset .gitignore
git reset ./newfolder
```

To see the log of commits, use code `git log`.


## Cloning remote project
Syntax for cloning
```
git clone <url> <where to download>
git clone <url> ./Desktop/project
```

The `git branch -a` shows all branches locally or remotely.
The `git diff` shows the lates difference beteem now and latest commit.

Remember to `git pull origin master` the repo before commit so you have the latest changes and then commit new changes
Then you can do `git push origin master` to upload your changes to remote repo

#### Note
If the remote repo is an active repo, meaning that it is not a bare (storage-only) repo, you can not push to the same active branch

## Creating branch
The syntax to create a branch and check it out, is like below
```
git branch develop
git checkout develop
```

## Pushing new branch to remote
For uploading new branches to remote repo, just use code below once and after that we can just use `git push` or `git pull`

```
git push -u origin local-branch
```

The `-u` option associates the local-branch to the remote

## Merging


