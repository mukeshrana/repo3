create a new repository on the command line
echo "# repo3" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/mukeshrana/repo3.git
git push -u origin main

…or push an existing repository from the command line
git remote add origin https://github.com/mukeshrana/repo3.git
git branch -M main
git push -u origin main

mukesh.rana@INND3LTC9LMDB3 MINGW64 /c/projects/test/testdir (master)
$ git config --global user.name="mukesh.rana"
$ git config --global user.email=mukesh.rana@ihsmarkit.com
$ git init
Initialized empty Git repository in C:/projects/test/testdir/.git/

$ touch a.txt
$ notepad a.txt

$ git status
On branch master
No commits yet
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        a.txt
nothing added to commit but untracked files present (use "git add" to track)

$ git add .
$ git status
On branch master
No commits yet
Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   a.txt

$ git commit -m "first commit"
[master a3334d5] first commit
 Committer: Mukesh Rana <mukesh.rana@ihsmarkit.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:
    git config --global user.name "Your Name"
    git config --global user.email you@example.com
After doing this, you may fix the identity used for this commit with:
    git commit --amend --reset-author
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md

//make remote connection
$ git remote -v
origin  https://github.com/mukeshrana/repo3.git (fetch)
origin  https://github.com/mukeshrana/repo3.git (push)

$ git push -u origin master
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 324 bytes | 324.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/mukeshrana/repo3.git
   0652aa9..97b1439  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

git config = configure username, repo and email
git init = initialize local git repo
git clone = clone the remote repo to local folder
git add = add one or more files to staging area
git diff = view changes made in file
git commit commit to head, not to remote report
git reset = undo local changes to state of get repo
get status = state of working dir and staging area
git merge = merge a branh into active branch
git push = upload changes from local repo to remote repo
git pull = fetch and download from remote repo to local repo
git remote add origin = New Repo

