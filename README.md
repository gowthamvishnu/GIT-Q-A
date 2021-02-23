# GIT-Q-A

1) what is git?
  * it is one of the source code management tool.it is an example of distributed version control system.
  * rather than have only one singe place for full version of the software as in comman place in once popular version control sytem 
    like CVS or SUBVERSION(also known as SVN).
  * in GIT every developer"s working copy the code is also a repositor that contain the full history of all changes.

2)what is DVCS(Distributed version control system)?
   * rather than have only one singe place for full version of the software as in comman place in once popular version control sytem 
    like CVS or SUBVERSION(also known as SVN).
   * In git ,every developer's working copy of the code is also a repository that can contain the full history of all changes.
   * in ddition being distributed ,git has been designed with performence,security and flexibilitu in mind.
   
3)why use git?
  * it is so fast.
  * you don't need access to a server.
  * Amazingly good at merzing simultaneous changes.

4)what are the uses of scm tools?
  * versioning 
  * overwriting capability(scm does not overwrite code)
  * scm maintain metadata( file name,changes,username,etc..)
  * scm provides rollback facility.
  * advantage of conccrent development(mutiple developing teams can work without distrubing others).

5)what is repository?
  * The database  storing the files.

6) SCM archtecture?
  * it works on two type architecture
  a)server: the database storing the repository.ex:Git hub,BIT bucket.
  b) client: it is a tool used to connect to the GIT server. ex: git bash

7)difference between centralized and distibuted version control sytems?
  a)CVS:
    *uses a central server to store all the versions of files.
    *No developer has a copy of all the files in the local system.
    * If the central server crashes,entire data of project will be lost.
  b)DVCS:
    *every developer ha s a copy of sll the versions of the code on their system.
    * improve the ability to work offline and does not rely on single location for backups
    8 there is no threat even if the server crashes.
 
8)what is git pull?
  * it is used to get the latest changes from the remote repository.
  cmd: git pull remote_repo_url

9)what is git fetch?
  * it will do the fetch (or). it will track (or) it will download the remote changes but it doesn't reflect on the local repository.
  cmd: git fetch remote_repo_url

10)what is  git merge?
  * if we want to reflect the remote changes in the local repository we will use the git merge followed by the git fetch.
  * we can say that git merge = git pull + git fetch.
    git merge source_branch_name
 Note:whenever you are merging you have to remember that you were always checkout in the destination branch.
 
11)git cherry-pick?
  * it is the act of picking a commit from a branch and apply it to another branch.
  * you can switch to the correct branch and cherry-pick the commit to where it should belong.

12) what is the process to revert a commit that has already been pushed and made public?
  * there are 2 processes through which you can revert a commit.
  a)remove or fix the bad file in a new commit and push it to the remote repository.then commit it to the remote repository using:
    git commit -m "commit msg"
  b)create a new commit that undergoes all the changes that were made in the bad commit.use the following commnd
    git revert <commit id>
    ex: git revert 568deo35f

13)what is meant by git reset?

14)what is meant by git revert ?

15)what is meant by git rebase?
a)this is also a way of combining the workflow between two branches.it can be used to make a linear sequence of commits.

16)what is meant by git stashing?

17)git index/git staging area?
a)it is a intermediate layer resides between workspace and the local repository.
  localworkspace -- index/staging area -- local repo 

18)what is meant by git branch?
a) copy of the current branch.
  cmd: git branch (branc_name)  --> To create a branch

19)what is meant by git commit?
a)to add the changes from staging area to remote directory we need to commit the changes with a commit message.
  cmd: git commit -m"commit msg"

20)what is meant by git log?
a)it will tell you total commits information like how many commites done,commitid,commited by whom,commit information etc..
 cmd: git log

21)what is meant by git add?
a)adding the files/code/changes to the staging area from local workspace/working area.
 cmd: git add filename -->To add a particular file
      git add ./*      --> to add all the files in that repo

22)what is meant by git status?
a) It will tell us that which files are added to the staging area from local repository and which are not.
   when ever we use this command,if the files are showing in red colour that means those files are not added to staging area.
   if the files are showing in green colour that means those files are added to staging area.
   cmd: git status
   
23)what is meant by git push?
a)To push the local changes to the remote repo we use git push.
  git push origin branchname

24)what is meant by git clone?
a)To clone the remote repo to local workspace.
  cmd: git clone remote_repo_url

25)explain git configuration?
a)i It is a git configuration file of git to introduce yourself to git.
git config --global user.name "examplename"
git config --global user.mail "example@mail"
To use the different username and password for a particular project.
change it inside the project
change the directory to particular directory.folling commands
git config user.name "examplename"(without global)
git config user.mail "example@mail"(without global)
 


