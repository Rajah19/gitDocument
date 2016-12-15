# Git notes.

#  Global configuration.
-	Git config --global user.name “Your name”
-	Git config –global user.email your email

-  Initialize => git init , git clone
  
-	To add files             => git add .    or   git add <filename> or  git add directory/
-	To commit              => git commit –m “”
-	To add and commit  => git commit –am “”
-	To delete file            =>   git rm <filename>
-	To get status             =>   git status

# Git log
-	Git help log
-	View all                    => git log,
-	View number of log  => git log -n 1
-	View since                => git log - -since= 2014-05-15
-	View until                 => git log - -until= 2005-05-25
-	 View by author        => git log - - author=””
-	 Grep by word           => git log - -grep=”hi”
-	  Get online info        => git log - -oneline
-	 Git show log

# To rename file  
-	git mv oldFilename  newFilename  
-	 git mv oldFilename    directory/newFileName


# Different from file and branches 
-	To get all: Git diff
-	Base on file: git diff - - base <filename>
                        ** git diff - -color -words <filename>
-	Preview changes, before merging: git diff <sourcebarnch> <targetbranch>
                      **Git diff –color-words <branchName>.. <branchName>
-	 Find different form stage   :              git diff - - staged 
-	Press q to exit from different. 
-	Use F and B for forward and backward.

 # Changes    
-	Undo changes in file :  *Git checkout - - <filename> 
-	Undo stage                : git reset HEAD <filename>
-	Amend commit         : git commit - - amend –m “get the previous commit”
-	Revert old one           : git checkout 20ea6a53a4f2 - - filename
-	Revert commit           : git revert sha

# Branch 
-	Create branch: git branch nameOfbranch
-	View Branch:  git branch or git branch –a or git branch –r
-	Switch Branch:  git checkout branchName
-	Delete branch : git branch –d branchName

# Merge
To merge branch, you must go main branch, and 
-	Git merge branchName
-	Git branch - -merged
-	Git branch - - no-merge


# Remote
Add remote repository
   git remote add origin https://github.com/rajah10/sqlAndMySql.git



# Create a remote branch 

-	git remote –u repositoryName localBranch
-	git branch –a 
-	git branch –r => only show remote branch
-	git push remoteBanchName
-	git fetch nameOfTheRepository or remoteBranchName
-	git merge origin/BranchName


# To delete remote branch 

-	git push origin : branchName



# Clone repository to local machine

-	Git clone path
-	git remote
-	git remote –v  (view repository )
-	git remote rm repositoryName  ( remove repository )



# My work Flow
	Git checkout master
	Git fetch
	Git merge origin/master
	Git checkout –b newBranchName
	Git commit –m “ “
	Git fetch
	Git push –u origin barnchName

# Collaborator view
	Git checkout master
	Git fetch
	Git merge origin/master
	Git checkout –b branchName origin/branchName
	Git log
	Git show 84521d
	Git commit –am “”
	Git fetch
	Git push

 
# Again my work
	Git fetch
	Git log –p branchName..origin/branchName
	Git merge origin/branchName
	Git checkout master
	Git fetch
	Git merge origin/master
	Git merge branchName
	Git push



