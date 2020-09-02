# week-02-day-1
user@DESKTOP-RT23FHQ MINGW64 ~
$ cd Desktop

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop (master)
$ mkdir first_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop (master)
$ cd first_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git init
Initialized empty Git repository in C:/Users/user/Desktop/first_repo/.git/

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git clone https://github.com/amitkumarau13/cc3.git
Cloning into 'cc3'...
warning: You appear to have cloned an empty repository.

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ touch readme.md

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        cc3/
        readme.md

nothing added to commit but untracked files present (use "git add" to track)

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git add .
error: 'cc3/' does not have a commit checked out
fatal: adding files failed

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git add readme.md

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   readme.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        cc3/


user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git commit -m"file added"
[master (root-commit) cdc1320] file added
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 readme.md

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git log
commit cdc1320ce00d1aecdb9a0dbc2c73e9a033777972 (HEAD -> master)
Author: Amit kumar <duter.duter@gmail.com>
Date:   Wed Sep 2 21:38:43 2020 +0530

    file added

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git remote add origin https://github.com/amitkumarau13/cc3.git

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 210 bytes | 210.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/amitkumarau13/cc3.git
 * [new branch]      master -> master

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ cd ..

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop (master)
$ mkdir second_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop (master)
$ cd second_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo (master)
$ git clone https://github.com/amitkumarau13/cc3.git
Cloning into 'cc3'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 190 bytes | 0 bytes/s, done.

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo (master)
$ ls
cc3/

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo (master)
$ cd cc3

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ ls
readme.md

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ start readme.md

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ git commit-m"file changed"
git: 'commit-mfile changed' is not a git command. See 'git --help'.

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ git commit -m"file changed"
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ git log
commit cdc1320ce00d1aecdb9a0dbc2c73e9a033777972 (HEAD -> master, origin/master,
origin/HEAD)
Author: Amit kumar <duter.duter@gmail.com>
Date:   Wed Sep 2 21:38:43 2020 +0530

    file added

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ git pull origin first_repo
fatal: couldn't find remote ref first_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo/cc3 (master)
$ cd ..

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/second_repo (master)
$ cd ..

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop (master)
$ cd first_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git pull origin first_repo
fatal: couldn't find remote ref first_repo

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git pull origin cc2
fatal: couldn't find remote ref cc2

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ git pull origin master
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 632 bytes | 3.00 KiB/s, done.
From https://github.com/amitkumarau13/cc3
 * branch            master     -> FETCH_HEAD
   cdc1320..c9b94fc  master     -> origin/master
Updating cdc1320..c9b94fc
Fast-forward
 readme.md | 1 +
 1 file changed, 1 insertion(+)

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$ ^C

user@DESKTOP-RT23FHQ MINGW64 ~/Desktop/first_repo (master)
$



