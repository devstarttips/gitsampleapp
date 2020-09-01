**GIT**

**GITHUB ACCOUNTS**

Dev Center Personal Github: jarondevcenter password: Glory27!

DevStart Github devstarttips password: Glory27!

Portfolio Github: jaronmanyama password: Glory27!


**CONFIG GIT AT USER LEVEL**

git config --global user.name "jaronmanyama" (setting username)
git config --global user.email "jaron.manyama@sap.com"

**TO SEE CHANGES**
git config --list


**TO RETRIVE INFO FROM CONFIG FILE**
git config user.name (will retrieve username)
git config user.email (will retrieve email)


**CREATE DIRECTORY AND FILES**

mkdir foldername (create directory)
touch filename (create file)

**INITIALIZE A FOLDER AS AN EMPTY GIT REPO**
1. cd into the directory you want
2. git init (creates a git file in folder)


**TO ADD A FILE:**

git add filename or git add . (for all files)

TO UNSTAGE A FILE:

git reset filename


**CREATE A REMOTE REPOSITORY ON GITHUB**
1. Click New Repository
2. Give it a name
3. Click Create a Repository

4. git commit -m "first commit"
5. git remote add origin https://github.com/jaronmanyama/Blog-For-Thought.git (example repo name)
6. git push -u origin master



**FORK REPO FROM GITHUB**

CLONE A REPOSITORY:

git clone https://github.com/jaronmanyama/Blog-For-Thought.git



**AFTER FORKING A REPO, TO PROPOSE CHANGES TO THE ORIGINAL REPOSITORY,**
**CONFIGURE GIT TO PULL AND SUBMIT CHANGES TO AND FROM THE ORIGINAL(UPSTREAM) REPO,**
**FROM YOUR FORKED REPO, SO THAT THEY ARE IN SYNC:**

1. cd TO THE FORKED REPO

2. git remote -v (origin fetch and origin push version of repo will apppear)
fetch will retrieve changes; push will send changes

3. git remote add upstream https://github.com/jaronmanyama/Blog-For-Thought.git (initializing forked repo as an upstream repo)

4. git remote -v (upstream fetch and upstream push version of repo will now appear)


TO PULL UPDATES DOWN TO YOUR LOCAL REPOSITORY:

1. git pull 

**TO PUSH CHANGES TO TO THE FORKED REPOSITORY:
1. git push



**CREATING A GIT BRANCH**

BRANCH- An independent line of development, because you don't want to commit your changes to the main branch

1. git branch login (branch name is login in this example)

2. git checkout login (will switch to login branch)

AFTER COMMITTING CHANGES TO THE FEATURE BRANCH, MERGE BY:

3. git merge login (will merge feature branch to master branch)


**CREATE GITIGNORE FILE**

A file used by git to determine which files or directories to ignore when performing a commit

Cloned repositories will inherit the gitignore when this file is committed

1. Make sure gitignore file is in the same directory as files you want to ignore

2. touch .gitignore

3. type name of file in gitignore file


**TO VIEW GIT LOGS**

git log (will show all commits done)

TO QUIT THE LOG VIEW:

q (will clear the screen)

git log -n5(will show the last number of commits displayed)

git log --since=2020-09-1 (will show all commits since that day)


**HEAD**

Is a reference to a commit object

Each head has a name

By default every repo has a head called a Master

A repo can contian several heads

The current active head is always in capitals HEAD


**TO CHECK WHAT THE CURRENT HEAD IS:**  

cat .git/HEAD