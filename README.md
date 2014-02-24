git-practice
============

This is a Git playground repository to practice in a real environment but without catastrophic consequences.

This is a playground, so you're free to play around with it: fork, clone, commit, push, pull, accept pull requests...


Git Exercise Example:
----

- Fork the repository
- Clone
- Create a branch
- Add files or modify files and add your name to the Contributors list
- Check differences
- Commit the changes
- Push it the repository
- Pull request to the master branch in pyladies-bcn organization

How to solve the exercise?
----

### 1. Fork the repository

To fork this project, click the "Fork" button in the GitHub.com repository.

### 2. Clone the repository

Type in your terminal:

	$ git clone https://github.com/{username}/git-practice.git

Change directory:

	$ cd git-practice

### 3. Create a branch

To create a branch

	# Creates a new branch called "mybranch"
	$ git branch mybranch

	# Makes "mybranch" the active branch
	$ git checkout mybranch

### 4. Modify Files

Open the file you want to modify with your favorite text editor (vim, emacs, Sublime...)

With vim, for example:
	
	vim Contributors.md

Example: Add your name to the list and save the document.

### 5. Check differences

If you do `git status` you can see that the Contributors.md file has been modified but not committed yet.

	$ git status
	# On branch mybranch
	# Changes not staged for commit:
	#   (use "git add <file>..." to update what will be committed)
	#   (use "git checkout -- <file>..." to discard changes in working directory)
	#
	#	modified:   Contributors.md
	#
	no changes added to commit (use "git add" and/or "git commit -a")

You can also do `git diff` to see the difference between documents.

	$ git diff

### 6. Commit the changes

First you'll have to add the changes with:

	$ git add Contributors.md

If you do `git status` now, you'll see the following:
	
	$ git status
	# On branch mybranch
	# Changes to be committed:
	# (use "git reset HEAD <file>..." to unstage)
	#
	# modified:   README.md

And then commit the changes

	$ git commit -m "Your message for the commit"

### 7. Push it the repository

To push it back to your repository:

	$ git push origin mybranch

### 8. Pull request

To merge your changes into the pyladies-bcn git-practice. Check the info on github on [Pull requests](https://help.github.com/articles/using-pull-requests).

Or just go to your repo and you should see a green button saying `Merge and pull request`
