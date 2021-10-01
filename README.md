# COGS 108 Final Project #

***NOTE:*** name subject to change

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

***NOTE:*** As the project progresses, we may need to run an install command from a package manager. This is not important now

## Making Edits ##

If you want to begin editing make sure to pull from within the repository just to make sure everything is up to date.
If you wnat to update master, checkout then pull from master.
```
$ git checkout master
$ git pull 
```
Aditionally, git has recently removed account password as a valid autentication method. 
If pushing asks you for Github username and Github password, the username is the same but the password is now an access token.
this access token may be asked of you every time you push, so make sure to save it!
Read Here for creating an access token on github: 
```
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
```
To save the accss token, you can use credential helper, which saves an unencryped version of the access token and username
```
$ git config credential.helper store
$ git push
<your username entered here will be stored>
<your password entered here will be stored>
```

If you are making a new feature, create a new branch with the naming convention user/feature-name
```
$ git branch shan/data-analysis
```
and checkout to work in that banch
```
$ git checkout shan/data-analysis
```

Since you just created that branch, it doesnt exist on the Github Repo yet
This command allows you to push a new branch and add tracking history to the Github Repo if it didnt exist before:
```
$ git push -u origin shan/data-analysis
```
You can push that branch to the GitHub repo again after more commits with:
```
$ git push
```

When the changes are complete and you think that they should be merged to master we will make Pull Requests (PRs):
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

***TL;DR:*** We will make new changes with new branches named like [ developer-name/feature-title ], push them as sepateate branches to the repo, and then merge to master only on github after a pull request.
