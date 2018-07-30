# Table of contents
- [Git tutorial](#git-tutorial)
	- [Install on windows](#install-on-windows)
	- [Creating your first git repository](#creating-your-first-git-repository)
	  - [Create a git folder for your repositories](#create-a-git-folder-for-your-repositories)
	  - [Create a local repository](#create-a-local-repository)
	- [How to get Started with GitHub](#how-to-get-started-with-github)
	  - [Create a GitHub account](#create-a-github-acccount)
	  - [Generating SSH key](#generating-an-ssh-key)
	- [Resources](#resources)

# Git tutorial
## Install on Windows
1) Download git from [here](https://git-scm.com/downloads)
2) Go through the installer steps. It is recommended to look at every step, but if you do not understand a 100%, the default settings are OK
3) You have installed git

> __NOTE__: The following parts all use the commandline. Windows users are recommended to install a decent terminal. If you do not have one, the Git Bash terminal will work as well 

## How to get started with GitHub
Go to [GitHub](https://github.com) and create an account

### Generating an SSH key
On your command line, type the following
```bash
git config --global user.email "email@example.com"
git config --global user.name "Mona Lisa"

ssh-keygen -t rsa -C "email@example.com"

cp ~/.ssh/id_rsa.pub > /dev/clipboard 
```

Now that you have copied your public SSH key to your keyboard, in GitHub go to Settings -> SSH and GPG keys and add your key with a nice label

## Creating your first git repository
It is good practice to have your git repositories in one place.
For the following paragraphs, our git folder will be in `C:\Users\user\Documents\`

### Create a git folder for your repositories
Open up the terminal and enter the following commands

```bash
cd ~\Documents
mkdir git
cd git
```

### Create a local repository
Go to the [repository for this course](https://github.com/atos-datascience/data-analytics-and-science) and press the Fork button in the top right

This will fork the repository and create a local copy on your GitHub account. This copy can be edited, removed, destroyed, ruined I do not care.
On that copy, Press clone or download and copy the URL you see.

Next, inside your git folder use the following command
```bash
git clone git@github.com:<your_name_here>/data-analytics-and-science.git
```

It will create a data-analytics-and-science folder for you

```bash
cd data-analytics-and-science
git status
git remote -v
```

## Making your first change
Make a change, open a jupyter note book, do something cool.

```bash
# See the changes
git status

# Add changes to file tracker
git add .

# Add all changes to the tree
git commit -m "Add making your first change to README"

# Push changes to master on origin
git push origin master
```

## Opening a pull request

## Updating local repository and keeping your fork in sync

## Resources
- [Git cheat sheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)
- [What is Git](https://www.atlassian.com/git/tutorials/what-is-git)