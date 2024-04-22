# Gym-Git-Exercise-Solutions

## Bundle 1

### Exercise 1

``` bash
Honorine@Tuyishime-PC MINGW64 ~
$ mkdir GitBundle1

Honorine@Tuyishime-PC MINGW64 ~
$ cd GitBundle1

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1
$ git init
Initialized empty Git repository in C:/Users/honor/GitBundle1/.git/

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (main)
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (main)
$ git branch -m Main

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ touch index.html

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ ls
index.html

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ code index.html

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git add index.html

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git commit -m "Add index.html"
[Main (root-commit) 4e28d4b] Add index.html
 1 file changed, 11 insertions(+)
 create mode 100644 index.html

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git remote add origin git@github.com:tuyishimehono/GitBundle1.git

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git status
On branch Main
nothing to commit, working tree clean

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git push
fatal: The current branch Main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin Main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git push --set-upstream origin Main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 384 bytes | 384.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      Main -> Main
branch 'Main' set up to track 'origin/Main'.

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git push
Everything up-to-date

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git branch dev

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git branch
* Main
  dev

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git checkout dev
Switched to branch 'dev'

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git branch test

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git branch
  Main
* dev
  test

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git checkout Main
Switched to branch 'Main'
Your branch is up to date with 'origin/Main'.

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git branch
* Main
  dev
  test

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (Main)
$ git checkout dev
Switched to branch 'dev'

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/dev
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git branch
  Main
* dev
  test


Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git checkout test
Switched to branch 'test'

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/test
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      test -> test

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git branch -D test
Deleted branch test (was 4e28d4b).

Honorine@Tuyishime-PC MINGW64 ~/GitBundle1 (dev)
$ git push origin --delete test
To github.com:tuyishimehono/GitBundle1.git
 - [deleted]         test

