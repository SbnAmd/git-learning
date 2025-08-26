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
