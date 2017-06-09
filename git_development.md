# Documentation
[Here's some documentation on for Git.](https://git-scm.com/)

# Clone the repository
In your terminal, go to a folder you'd like to develop in. For example, `Documents/repos`. Clone the repo into your account.
```
git clone https://github.com/YATDA/YATDA
```

This is all the setup you need for development.

# Terminology

Before we get into development, lets go over some quick terminology:

Local Repository - the repository you cloned onto your hard drive. You make changes to it and then push those changes to the online repository.

Main/GitHub/Online Repository - The repository that everyone can see. After you make changes, you push to this repository 

Project directory - This is the base folder if your repository. It has a `package.json` file in it, as well as a `Readme.md` file.
# The Development Process

1. `git checkout master` - This may be unnecessary (especially if you just cloned the repository), but you should do this to make sure you're not on a branch (if you don't know what a branch is, more on that later).
2. `git pull origin master` - always start with this. It will pull down any updates to the main repo since you last did any development.
3. `git checkout -b username-branchname` - replace "username-branchname" with your username something that makes sense to you. Usually, something related to the task you're working on e.g. `idlewinn-gitdevelopment`. This will create a new branch in the local repository. Any changes you make will not be reflected in the master branch.
4. Development - do some work on your task(s).
5. `git add .` from the project directory. This will add all changes you made to your LOCAL repository.
6. `git commit` from the project directory. This will commit all changes that you've added to the LOCAL repository.
7. Repeat steps 4-6 often so it's easy to revert changes. When you're ready to push your changes to master, proceed to step 8.
8. `git push origin username-branchname` - this will push all changes on your current branch to the same branch on the GitHub repository. At this point, you can look at the online repository and there should be an option to submit a pull request.