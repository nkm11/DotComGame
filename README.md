DotComGame
==========

From headFirst
git config --global user.name nkm11
git config --global user.email "nkm11@github.com"
git config --list
git config user.name

**START
$ mkdir -p ~/gitrepo
$ cd ~/gitrepo
$ git init DotComGame
Initialized empty Git repository in /home/nmadhyas/gitrepo/DotComGame/.git/

$ cd DotComGame/
$ git status
# On branch master
#
# Initial commit
#
nothing to commit (create/copy files and use "git add" to track)
#

#COPIED TWO FILES(CREATED)
$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	GameHelper.java
#	SimpleDotTest.java
nothing added to commit but untracked files present (use "git add" to track)
$

**ADD ONE FILE
$ git add SimpleDotTest.java
nmadhyas@mandara:~/gitrepo/DotComGame$ git status
# On branch master
#
# Initial commit
#
# Changes to be committed:
#   (use "git rm --cached <file>..." to unstage)
#
#	new file:   SimpleDotTest.java
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#	GameHelper.java
$

$ git commit GameHelper.java -m "Into repo"
[master (root-commit) 4e58050] Into repo
 1 file changed, 15 insertions(+)
 create mode 100644 GameHelper.java
$

Two questions: What have you changed but not yet staged? And what have you staged that you are about to commit? 

git remote add origin https://github.com/nkm11/DotComGame.git
git push -u origin master
