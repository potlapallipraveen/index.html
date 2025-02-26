GIT: GLOBAL INFORMATION TRACKER.

VCS: VERSION CONTROL SYSTEM
it will keep the code separately for each version.

v-1	: 100 lines --- > store (repo-1)
v-2	: 200 lines --- > store (repo-2)
v-3	: 300 lines --- > store (repo-3)

REPO: It is a folder where we store our code.
index.html: it is a basic file for every application

v1 --- > index.html
v2 --- > index.html
v3 --- > index.html 


INTRO:
Git is used to track the files.
It will maintain multiple versions of the same file.
It is platform-independent.
It is free and open-source.
They can handle larger projects efficiently.
It is 3rd generation of vcs.
it is written on c programming
it came on the year 2005


CVCS: CENTRALIZED VERSION CONTROL SYSTEM
EX: SVN: it can store code on a single repo.

DVCS: DISTRIBUTED VERSION CONTROL SYSTEM
EX: GIT: it can store code on Multiple repo.


ROLLBACK: Going back to the previous version of the application.


STAGES:
WORKING DIRECTORY: where we write our source code.
STAGING AREA: we track files here.
REPOSITORY: where we store tracked source code


WORKING WITH GIT:
create a ec2 server:
mkdir swiggy
cd swiggy

yum install git -y  [yum=pkg manager, install=action, git=pkg name -y=yes]
git -v	: to check version
git init : to install .git (local repo)


To create file	: vim index.html (content is opt)
to check status	: git status
to track file	: git add index.html
to check status	: git status
to store file	: git commit -m "commit-1" index.html

create a file -- > add -- > commit 

to show commits	: git log
to show	last 2 commits: git log -2
to show commits in single line: git log -2 --oneline


=================================================

CONFIGURING USER AND EMAIL:

git config user.name "raham"
git config user.email "raham@gmail.com"


NOTE: this user and email will be replicated to new commits only.


Git show: used to show the files which are attached to commits.
git log --online
git show commit_id


BRANCHES:
It is a individaual line of developemt.
developers write the code on branches.
initally baraches we create on git.
after write source code on git we push to github.
Default barnch is Master.
Note: when we do a iniatl commit the only default branch will be created.

Dev -- > Git (Movies branch) -- > code -- > github


COMMNDS:
git branch		: to list the branches
git branch movies	: to create the branch movie
git checkout movies	: to switch blw the branches
git checkout -b dth	: to create and switch dth at same time
git branch -m old new	: to rename a branch
git branch -D recharge	: to delete a branch

NOTE: to recover the delete branch

GIT PULL: it will get the branch from github to git
git pull origin recharge
git checkout recharge




PROCESS:
git branch movies
git checkout movies
touch movies{1..5}
git add movies*
git commit -m "dev-1" movies*


NOW PUSH THE CODE TO GITHUB:
create a repo
git remote add origin https://github.com/nayakdebasish091/paytm.git

PUSH: to send files form git to github
local: .git & remote: paytm.git
git push origin movies
username:
password:

TOKEN GENERATION: 
account -- > settings -- >developer settings -- > PAT -- > Classic -- > Generate new token -- > classic -- > name: abcd -- > select 6 options -- > generate 

Note: it will be visible only once





create branch
switch to branch
files
add
commit
push

GIT IGNORE: it will not track the files which we want.
touch java{1..5}
vim .gitignore
j* -- > :wq
git status
you cant see the files now 


GIT RESTORE: to untrack the tracked file
touch raham
git status
git add
git status
git restore --staged raham
git status


GET BACK THE DELETED FILE:
Note: we can restore only tracked files.


HISTORY:

 1  df -h
    2  cd cd
    3  cd /
    4  cd /
    5  du -sh
    6  ll
    7  cd
    8  yum install git maven docker httpd tree htop -y
    9  touch file{1..10
   10  rm -rf file\{1..10
   11  rm -rf file\{1..10}
   12  ll
   13  touch file{1..10}
   14  vim file1
   15  rm -rf *
   16  mkdir paytm
   17  cd paytm/
   18  ls -al
   19  git init
   20  touch index.html
   21  git add index.html
   22  git config user.name "raham"
   23  git config user.email "raham@gmail.com"
   24  git commit -m "commit-1" index.html
   25  git branch
   26  git branch movies
   27  git branch
   28  git checkout movies
   29  touch movies{1..5}
   30  git add movies*
   31  git commit -m "dev-1" movies*
   32  git remote add origin https://github.com/RAHAMSHAIK007/1045paytm.git
   33  git push origin movies
   34  git branch
   35  git branch train
   36  git branch
   37  git checkout train
   38  git branch
   39  touch train{1..5}
   40  git add train*
   41  git commit -m "dev-2" train*
   42  git push origin train
   43  ll
   44  git branch
   45  git checkout -b dth
   46  git branch
   47  ll
   48  touch dth{1..5}
   49  git add dth*
   50  git commit -m "dev-3" dth*
   51  git push origin dth
   52  git checkout -b recharge
   53  touch recharge{1..5}
   54  git add recharge*
   55  git commit -m "dev-4" recharge*
   56  git push origin recharge
   57  ll
   58  git status
   59  touch java{1..5}
   60  git status
   61  vim .gitignore
   62  git status
   63  vim .gitignore
   64  git status
   65  ll
   66  git add *
   67  ll
   68  git status
   69  touch python{1..5}
   70  git status
   71  vim .gitignore
   72  git status
   73  ll
   74  git branch
   75  git branch -m master raham
   76  git branch
   77  git branch -m raham main
   78  git branch
   79  git branch -m main master
   80  git branch
   81  ll
   82  git push origin movies
   83  git branch
   84  git branch -D recharge
   85  git checkout movies
   86  git branch -D recharge
   87  git branch
   88  git pull origin recharge
   89  git branch
   90  git checkout recharge
   91  git branch
   92  ll
   93  git branch
   94  git branch -D movies
   95  git branch
   96  git pull origin movies
   97  ll
   98  git branch
   99  git checkout movies
  100  git branch
  101  touch raham
  102  git status
  103  git add raham
  104  git status
  105  git restore --staged raham
  106  git status
  107  git add raham
  108  git status
  109  git restore --staged raham
  110  git status
  111  rm -f raham
  112  git restore raham
  113  ll
  114  git status
  115  cd
  116  mkdir abcd
  117  cd abcd/
  118  touch file1
  119  git add file1
  120  git init
  121  git add file1
  122  ll
  123  rm -f file1
  124  git restore file1
  125  ll
  126  touch file2
  127  git status
  128  rm -f file
  129  rm -f file2
  130  git restore file2
  131  ll
  132  touch file{1..100}
  133  git status
  134  git add *
  135  git status
  136  rm -f *
  137  git restore *
  138  ls
  139  cd
  140  cd paytm/
  141  git push origin train
  142  git push origin master movies
  143  history

=================================================
MERGE:
adding the files blw one branch to another branch
git merge branch_name

REBASE:
adding the files blw one branch to another branch
git rebase branch_name


MERGE VS REBASE:
merge will show files, rebase will not show files
merge will not show branches, rebase will show branches
merge will show entire history, rebase will not.


STASH: to hide the files which are not comitted.
note: file need to be tracked but not comitted


touch file2
git stash
git stash apply
git stash list
git stash clear
git stash pop (clears last stash)



HISTORY:

 1  cd p
    2  ll
    3  cd swiggy/
    4  ll
    5  git branch
    6  git branch -D master
    7  git branch -D dth
    8  ll
    9  git branch
   10  git pull origin dth
   11  cd
   12  git clone https://github.com/RAHAMSHAIK007/1045paytm.git
   13  ll
   14  cd 1045paytm/
   15  git branch
   16  git checkout train
   17  git branch
   18  git checkout dth
   19  git branch
   20  git checkout recharge
   21  ll
   22  git branch
   23  git branch -D dth
   24  git branch
   25  git pull origin dth
   26  git checkout dth
   27  git branch
   28  cd
   29  mkdir abcd
   30  cd abcd/
   31  git init
   32  ll
   33  touch java1
   34  git add java1
   35  git commit -m "java commits" java1
   36  ll
   37  touch java2
   38  git status
   39  git add java2
   40  git status
   41  ll
   42  git stash
   43  ll
   44  git stash apply
   45  ll
   46  git stash
   47  ll
   48  git stash apply
   49  ll
   50  git stash list
   51  git stash clear
   52  git stash list
   53  git stash -h
   54  git stash --help
   55  git stash list
   56  git stash
   57  git stash list
   58  history

==================================================================

MERGE CONFLICT:
when we try to merege 2 branches with same file and Different content
then conflict will raise.
so we need to reslove the conflict manually


CHERRY-PICK: 
we can merge only specific files from one branch to another
with the help of commit_id
git cherry-pik commit_id

SHOW:
to show the commits for a file
git show commit_id

git log --patch
git log --stat


REVERT: to undo the merging
git revert branc_name

HISTORY:

53  rm -rf *
   54  mkdir paytm
   55  cd paytm/
   56  yum install git -y
   57  git init
   58  touch file1
   59  vim file1
   60  git add file1
   61  git commit -m "one" file1
   62  git branch
   63  git branch -m master branch-1
   64  git branch
   65  cat file1
   66  git checkout -b branch-2
   67  vim file1
   68  git add file1
   69  git commit -m "two" file1
   70  cat file1
   71  git checkout branch-1
   72  vim file1
   73  git add file1
   74  git commit -m "three" file1
   75  cat file1
   76  git merge branch-2
   77  vim file1
   78  git add file1
   79  git commit -m "conflicts"
   80  git status
   81  git merge branch-2
   82  git branch
   83  touch java{1..5}
   84  git add java*
   85  git commit -m "java commits" java*
   86  touch python{1..5}
   87  git add python*
   88  git commit -m "python commits" python*
   89  touch php{1..5}
   90  git add php*
   91  git commit -m "php commits" php*
   92  git log --oneline
   93  git checkout branch-2
   94  ll
   95  git cherry-pick e300a84
   96  ll
   97  git cherry-pick df00587
   98  ll
   99  git logs
  100  git log
  101  git show 8b156541691925614eb6e083b6277e823fd340f0
  102  git show python1
  103  ll
  104  git diff python1
  105  vim python1
  106  git add python1
  107  git commit -m "new python" python1
  108  git diff python1
  109  vim python1
  110  git add python1
  111  git commit -m "new python file" python1
  112  git diff python1
  113  git show python1
  114  vim python1
  115  git add python1
  116  git commit -m "nwe pyt commits" python1
  117  git show python1
  118  diff --git a/python1 b/python1
  119  git diff python1
  120  git log --stat
  121  git log --patch
  122  git merge branch-1
  123  ll
  124  git revert
  125  git revert branch-1
  126  ll
  127  git clone https://github.com/torvalds/linux.git

INTERVIEW QUESTIONS:
what is git & why to use ?
Explain stages of git ?
Diff blw CVCS & DVCS ?
How to check commits in git ?
Explain branches ?
What is .gitingore ?
Diff blw git pull vs git push ?
Diff blw git pull vs git fetch ?
Diff blw git merge vs git rebase ? 
Diff blw git merge vs git cherry pick ?
Diff blw git clone vs git pull ?
Diff blw git clone vs git fork ?
Diff blw git revert vs git restore ?
merge conflict & how to resolve ?
what is git stash ?
