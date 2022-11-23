# python_automation_tutorial
Work through sets of examples of automation with python

# Visual Studio Virtual Environment - Windows  
## Command line Creation 
* "python -m venv .venv"
* navigate to the Activate.ps1 and it will run - ".\activate.ps1"
* create create a py or notebook (ipynb) file
* Make sure your ipynb file is running on the virtual environment. you might have to install things
* deactivate your virtual environment - "deactivate"

## Setting up a virtual environment with Git 
* "mkdir test-env && cd test-env" 
* "python3 -m venv env" 
* "source env/bin/activate" 
* "pip install pandas" 
* "deactivate" 
* "echo ‘env' > .gitignore" 
* Restart the virtual environment 
* "pip freeze > requirements.txt"
* NOW git init -  git add -  and git commit to station the changes 

You now have a notebook that has git controls and virtual environment

## Setting up virtual environment with ipython notebook 


## Github Tips 
It's often easier to instantiate your github repo first and then clone it to start working. You can use git init and make your README file locally and push it to an external repo. 

### Basic Functions 
git status 
git add . 
git commit -m "message" 
git push

### Branching 
git branch (tells you what branches exist)
git checkout -b name-of-feature  (creates new branch)
git branch (will show branches)
git checkout master (switches back to master)
git checkout name-of-feature (switches to new branch)

you can make changes and do the add, commit and push commands. 
git diff name-of-feature (shows differences)

Now you can push to github so you can have pull request 
git push --set upstream origin name-of-feature

We want this pulled into the master branch. You make a PR. Once its combined you 
You can merge on github and then you 
git pull 

Then delete branch 
git branch -d name-of-feature 

### Merging and Updating 
Sometimes the master will be changing and you want to keep your branch relevant. 
Switch to master 
git checkout and then git pull 
switch back to your branch and use git diff master and git merge master 
Fix conflicts and add/commit to current branch 

### Fixing mistakes 
* git reset 
* git reset HEAD ~1
* git log 
* git reset hash_of_commit_from_log

## Requirements File 
pip freeze > requirements.txt

## Install from Requirements File 
pip install -r requirements.txt

# Links to lectures 
* https://www.youtube.com/watch?v=PXMJ6FS7llk
* https://www.youtube.com/watch?v=s8XjEuplx_U


