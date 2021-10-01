# COGS 108 Final Project #

**_NOTE: _** name subject to change

## Authors: ##
- Finn St John
- Elliot Lee
- Shantelle Serafin
- Hinn Zhang
- Isa Vidanes

## Getting Started ##
this tutorial uses the git command line, as it is easiest to explain through the readme, and the simplest to get started with.
make sure git command line tools are installed.

go to the folder that you want to install this repository into
```
cd Documents
```

clone the repository
```
git clone https://github.com/stjohnfinn/cogs-108-final-project.git
```

Thats It! You now have the project cloned to your local workspace to get inside and start making edits
```
cd cogs-10-final-project
```

**_NOTE: _** As the project progresses, we may need to run an install command from a package manager.

## Making Edits ##
A branch for each developer has already been created. They are 
- shan
- hinn
- isa
- finn
- elliot

If you want to begin editing make sure to pull from within the repository
```
git pull 
```

When making edits, checkout your user branch. consider your user branch your main branch.
All your edits should be merged here.
```
git checkout shan
```

If you are making changes or a new feature/analysis make a new branch with the naming convention user/feature-name
```
git branch shan/data-analysis
```
and checkout to get there
```
git checkout shan/data-analysis
```

When your edits are complete merge to your user branch
```
git checkout shan
git merge shan/data-analysis
```
then push to github
```
git push
```

1. On the github go to the repository.
2. Select Pull Requests
3. Open a new pull request comparing your user branch to the master branch (the master branch is the base)
4. Write a short desciption of what you did and request for review.
5. Add someone to review your code, it doesnt matter who.
6. Comments on the changes can be added by the reviewer, and new changes and commits to resolve these suggestions can be easily pushed again.
7. After review and edits, we can merge it with master!

