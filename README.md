# COGS 108 Final Project #

NOTE: name subject to change

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
$ cd Documents
```

clone the repository
```
$ git clone https://github.com/stjohnfinn/cogs-108-final-project.git
```

Thats It! You now have the project cloned to your local workspace to get inside and start making edits
```
$ cd cogs-10-final-project
```

NOTE: As the project progresses, we may need to run an install command from a package manager. This is not important now

## Making Edits ##

If you want to begin editing make sure to pull from within the repository just to make sure everything is up to date
```
$ git checkout master
$ git pull 
```

If you are making a new shan/analysis make a new branch with the naming convention user/feature-name
```
$ git branch shan/data-analysis
```
and checkout to get there
```
$ git checkout shan/data-analysis
```

You can push any branch to the repo at any time 
```
$ git push
```

Aditionally, git has recently removed account password as a valid autentication method. 
If pushing asks you for Github username and Github password, the username is the same but the password is now an access token.
Read Here for creating an access token on github: 
```
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
```
this access token may be asked of you every time you push, so make sure to save it!

When the changes are complete and you think that they should be merged to master:
1. Final commit and push your changes
```
$ git commit -m "new changes"
$ git push
```
2. On Github go to the repository.
3. Select Pull Requests
4. Open a new pull request comparing your user branch (the branch you made is the compare) to the master branch (the master branch is the base).
5. Write a short desciption of what you did and request for review.
6. Add someone to review your code, it doesnt matter who. [elliot, shan, hinn, isa, finn]
7. Comments on the changes can be added by the reviewer
	- if there are edits that need to be made, the developer can go back resolve these suggestions by making edits, commits and pushing again.
8. After reviewer has approved the edits, we can merge it with master!

TL;DR: We will make new changes with new branches named like [ developer-name/feature-title ], push them as sepateate branches to the repo, and then merge to master only on github after a pull request.
