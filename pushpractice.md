KBS1@kbs-pc MINGW64 ~
$ cd push

KBS1@kbs-pc MINGW64 ~/push (master)
$ touch pushpractice.txt

KBS1@kbs-pc MINGW64 ~/push (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        pushpractice.txt

nothing added to commit but untracked files present (use "git add" to track)

KBS1@kbs-pc MINGW64 ~/push (master)
$ git add pushpractice.txt

KBS1@kbs-pc MINGW64 ~/push (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   pushpractice.txt


KBS1@kbs-pc MINGW64 ~/push (master)
$ git commit -m "practice"
[master 93ed597] practice
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 pushpractice.txt

KBS1@kbs-pc MINGW64 ~/push (master)
$ git push origin master
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 682 bytes | 341.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote:   https://github.com/BYEONGSEOKKIM/git_pushpractice.git
To https://github.com/BYEONGSEOKKIM/push.git
   25bb975..93ed597  master -> master

KBS1@kbs-pc MINGW64 ~/push (master)
$