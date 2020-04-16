## Connect github

jimkwon@uracil:~$ mkdir homepage

jimkwon@uracil:~$ cd homepage/

jimkwon@uracil:~/homepage$ git init
Initialized empty Git repository in /casa/jimkwon/homepage/.git/

jimkwon@uracil:~/homepage$ git remote add origin https://github.com/jimkwon/chullab.github.io

jimkwon@uracil:~/homepage$ git remote -v
origin  https://github.com/jimkwon/chullab.github.io (fetch)
origin  https://github.com/jimkwon/chullab.github.io (push)

jimkwon@uracil:~/homepage$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 2492 (delta 1), reused 0 (delta 0), pack-reused 2484
Receiving objects: 100% (2492/2492), 50.26 MiB | 11.88 MiB/s, done.
Resolving deltas: 100% (1102/1102), done.
From https://github.com/jimkwon/chullab.github.io
 * [new branch]      fix-teaching -> origin/fix-teaching
 * [new branch]      master       -> origin/master
 * [new branch]      read-more    -> origin/read-more
 * [new tag]         0.8.0        -> 0.8.0
 * [new tag]         v0.8.1       -> v0.8.1
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> master

jimkwon@uracil:~/homepage$ ls

jimkwon@uracil:~/homepage$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

jimkwon@uracil:~/homepage$ git clone https://github.com/jimkwon/chullab.github.io
Cloning into 'chullab.github.io'...
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (8/8), done.
remote: Total 2492 (delta 1), reused 0 (delta 0), pack-reused 2484
Receiving objects: 100% (2492/2492), 50.26 MiB | 10.59 MiB/s, done.
Resolving deltas: 100% (1102/1102), done.

jimkwon@uracil:~/homepage$ ls
chullab.github.io

# I modified some files

jimkwon@uracil:~/homepage/chullab.github.io$ git add *
jimkwon@uracil:~/homepage/chullab.github.io$ git commit -m "test1"
[master ffeb1ab] test1
 1 file changed, 15 insertions(+)
 create mode 100644 _publications/2015-10-01-paper-title-number-4.md

jimkwon@uracil:~/homepage/chullab.github.io$ git push origin master
Username for 'https://github.com': jimkwon
Password for 'https://jimkwon@github.com':
Counting objects: 4, done.
Delta compression using up to 32 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 624 bytes | 312.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/jimkwon/chullab.github.io
   12bf281..ffeb1ab  master -> master

jimkwon@uracil:~/homepage/chullab.github.io$


## Useful documents

https://kramdown.gettalong.org/quickref.html#block-attributes
https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet
https://jekyllrb.com/docs/collections/
https://mmistakes.github.io/minimal-mistakes/post%20formats/post-gallery/
https://github.com/mmistakes/minimal-mistakes/tree/master/test/_portfolio
https://learn.cloudcannon.com/jekyll/photo-gallery/
