# Learn to git-it!

This repository is a learning project created as I went along with the git-it workshop (https://github.com/jlord/git-it) found in nodeschool (http://nodeschool.io/#workshoppers) by [Jessica Lord @jlord](http://jlord.us/).

It was easy and welcoming to follow, informative, and also great fun. I was excited to see the robot merged my branch and thrilled to see my github ID appear in the page of people who completed (http://jlord.us/patchwork/). Great incentive!

Now it is only logical to review what I've learnt, put them down to words and let them sink in, before the weekend's gone and before my memories fade.


## Learning notes

Following is what I've picked up on the way through the eleven chapters of the workshop. 

### 1. GET GIT - configure git

* To check git number

	```
	$ git --version
	```


* To configure user name and email

	```
	$ git config --global user.name "Xiaoli Shen"
	$ git config --global user.email "alabebop@gmail.com"
	```


### 2. REPOSITORY

* To make a new folder and go into it

	```
	$ mkdir hello-world
	$ cd hello-world
	```


* To create a new Git instance for a project

	```
	$ git init
	```


* To check if a Git repo instance initiated and if there's change

	```
	$ git status
	```


### 3. COMMIT TO IT

* To add a file to git

	```
	$ git add readme.txt
	```

	(But I tend to use

	```
	$ git add .
	```

	to save some typing, or 

	```
	$ git add -A
	```

	which adds everything changed in the entire working tree, not only the current directory)


* To commit the changes to the repository's history

	```
	$ git commit -m "does something..."
	```


* To view differences made from the last commit

	```
	$ git diff
	```
	
	And to get out of the compare view, press

	```
	q
	```
	(To find out this I've headed to stackoverflow 눈_눈)


### 4 GITHUBBIN

* To add your github username to git configuration

	```
	$ git config --global user.username alabebop
	```


### 5 REMOTE CONTROL

* To add a remote location to local project

	Given that you've created an empty project on github to sync with your local work, to connect local project to this remote project location on github server, first let your local git know of the remote location:
	
	```
	$ git remote add origin https://...<URL OF YOUR GITHUB PROJECT>
	```

	Here you've added a remote location "origin" (as a norm for projects on github, the main remote location is to be named "origin") and linked it to the remote project URL from github. Each local project can have multiple remote locations.

	If you've already had an automatically added remote location named "origin", as is the case when using GitHub for Windows, use the following command to set its URL:

	```
	$ git remote set-url origin https://...<URL OF YOUR GITHUB PROJECT>
	```

* To push local work to remote

	```
	$ git push origin master
	```

	Here you're sending your "master" branch to your remote location "origin". If you have another branch whose changes you want to sync to "origin", replace "master" with this branch's name.

* To pull in remote changes to local copy

	```
	$ git pull origin master
	```

* To view remote connections

	```
	$ git remote -v
	```


### 6. FORKS

* To create your own version of someone else's project or to contribute fixes or features to a project that owned by other github users, you need to first fork the project (click the FORK button in the github project page)

* To clone a forked project to your local computer

	```
	$ git clone https://<forked project URL>
	```

* To connect cloned local copy to the original remote project (of someone else)

	```
	$ git remote add upstream https://<URL to the original project>
	```

	Here you named the remote location of the original project "upstream" - also a github norm.

	If you view your local project's remote connections now

	```
	$ git remote -v
	```
	you'd see both your fork and the original project on github.


### 7. BRANCHES AREN'T JUST FOR BIRDS

It's common practice to create a branch when you start to make changes (for a fix or a new feature), and keep all the changes in this branch until they are ready to be merged back into "master". In this way the master branch is kept stable and always ready to deploy.


Note: Github will host and serve automatically website files in branches named "gh-pages". All sites like this can be found using this pattern for the URL:

```
http://githubusername.github.io/repositoryname
```

* To create a branch

```
$ git branch <BRANCHNAME>
```

* To go in a branch and work on it

```
$ git checkout <BRANCHNAME>
```

* Or to create and move into a new branch at the same time

```
$ git checkout -b <BRANCHNAME>
``

* To push local changes in a branch to remote

```
$ git push origin <BRANCHNAME>
```

* To see which branch you are currently in

```
$ git status
```

* To list all branches

```
$ git branch
```

* To rename current branch

```
$ git branch -m <NEWBRANCHNAME>

```



















