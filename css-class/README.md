Git Tutorial

This tutorial covers the basic Git commands used to initialize a repository, add files, create commits, create branches, connect a local repository to GitHub, and push your code.

1. Initialize an Empty Git Repository

To initialize a new Git repository in your project folder, use:

git init


This creates a hidden .git folder that Git uses to track changes in your project.

2. Add Files to the Repository

To add all files in the current directory to the staging area:

git add .


The . means all files and folders in the current directory.

You can also add a specific file:

git add filename.html

3. Commit Your Changes

To save the staged changes with a message:

git commit -m "first commit"

What does -m mean?

The -m flag stands for message. It allows you to provide a description of the changes you are committing.

Example:

git commit -m "Added CSS tutorial"

4. Create/Rename the Main Branch

To create or rename the current branch to main:

git branch -M main


The main branch is commonly used as the primary branch of a Git repository.

5. Connect Your Local Repository to a Remote Repository

To connect your local Git repository to a remote repository such as GitHub:

git remote add origin repo_url


Replace repo_url with the URL of your GitHub repository.

For example:

git remote add origin https://github.com/username/my-project.git


Here:

origin is the name given to the remote repository.
repo_url is the URL of your remote GitHub repository.
6. Push Your Code to the Remote Repository

To upload your local code to the main branch:

git push -u origin main


The -u flag sets origin/main as the upstream branch. After this, you can usually push future changes simply with:

git push

Complete Git Workflow

Here is the complete sequence of commands for a new project:

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin repo_url
git push -u origin main

Quick Reference
Command	Purpose
git init	Initialize a Git repository
git add .	Add all files to the staging area
git commit -m "message"	Commit changes with a message
git branch -M main	Rename the current branch to main
git remote add origin repo_url	Connect local repository to a remote repository
git push -u origin main	Push the main branch to the remote repository
Basic Git Workflow

The basic Git workflow can be remembered as:

Working Directory
       ↓
   git add .
       ↓
Staging Area
       ↓
git commit -m "message"
       ↓
Local Repository
       ↓
git push
       ↓
Remote Repository


Tip: Always write meaningful commit messages so you can easily understand what changed in your project later.