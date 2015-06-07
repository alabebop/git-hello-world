# Learn to git-it!

This repository is a learning project created as I went along with the git-it workshop (https://github.com/jlord/git-it) found in nodeschool (http://nodeschool.io/#workshoppers) by [Jessica Lord @jlord](http://jlord.us/).

It was easy and welcoming to follow, informative, and also great fun. I was excited to see the robot merged my branch and thrilled to see my github ID appear in the page of people who completed (http://jlord.us/patchwork/). Great incentive!

Now it is only logical to review what I've learnt, put them down to words and let them sink in, before the weekend's gone and before my memories fade.


## Learning notes

Following is what I've picked up on the way through the eleven chapters of the workshop. 

1. GET GIT - configure git
	* To check git number
	```
	$ git --version
	```

	* To configure user name and email
	```
	$ git config --global user.name "Xiaoli Shen"
	$ git config --global user.email "alabebop@gmail.com"
	```

2. REPOSITORY
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

3. COMMIT TO IT
	* To add a file to git
	```
	$ git add readme.txt
	```
	(But I tend to use
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
	``








