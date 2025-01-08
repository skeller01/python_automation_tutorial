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

### More on Branching 
#### Branching & Pull Requests

**Creating and Switching Branches**

* **List branches:**
  ```bash
  git branch
  ```

* **Create a new branch and switch to it:**
  ```bash
  git checkout -b name-of-feature 
  ```

* **Switch back to main (or master):**
  ```bash
  git checkout main
  ```
  **Note:** Some repos use `main`, some use `master`. Adjust accordingly.

* **Make changes on your feature branch, then stage and commit:**
  ```bash
  git add .
  git commit -m "Add new feature"
  ```

* **Compare changes between branches:**
  ```bash
  git diff main
  ```

**Making a Pull Request (PR)**

* **Push your feature branch to GitHub:**
  ```bash
  git push --set-upstream origin name-of-feature
  ```

* **Open a Pull Request on GitHub:**
    1. Go to your repo on GitHub.
    2. Click "Compare & pull request".
    3. Set the base branch to `main` and the compare branch to `name-of-feature`.
    4. Add a title and description.
    5. Create the PR.


**Merging Changes & Deleting a Branch**

* Merge on GitHub (after PR approval) or merge locally.
* **Pull the latest changes to your local `main`:**
  ```bash
  git checkout main
  git pull
  ```

* **Delete the branch locally (if you're done):**
  ```bash
  git branch -d name-of-feature
  ```


#### Updating Your Branch with Latest Changes

* **Switch to `main`:**
  ```bash
  git checkout main
  git pull
  ```

* **Switch back to your feature branch:**
  ```bash
  git checkout name-of-feature
  ```

* **Merge `main` into your branch:**
  ```bash
  git merge main
  ```

* **Resolve conflicts (if any), then stage and commit:**
  ```bash
  git add .
  git commit -m "Resolve merge conflicts" 
  ```


#### Fixing Mistakes

* **Undo local changes (unstaged):**
  ```bash
  git checkout -- <file>
  ```

* **Unstage files:**
  ```bash
  git reset <file> 
  ```

* **Move HEAD back one commit (soft reset, keeps changes in your working directory):**
  ```bash
  git reset HEAD~1
  ```

* **View commit history:**
  ```bash
  git log
  ```

* **Hard reset to a specific commit (dangerous if you've already pushed):**
  ```bash
  git reset --hard <commit-hash>
  ```


#### Working with Requirements File

* **Generate `requirements.txt` from your current environment:**
  ```bash
  pip freeze > requirements.txt
  ```

* **Install from `requirements.txt`:**
  ```bash
  pip install -r requirements.txt
  ```

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


