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
```

### Exercise 2

```bash

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ touch home.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ code home.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git add home.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ touch about.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ code about.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git add about.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ touch team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ code team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git add team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 4e28d4b Add index.html
stash@{1}: WIP on dev: 4e28d4b Add index.html
stash@{2}: WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 4e28d4b Add index.html
stash@{1}: WIP on dev: 4e28d4b Add index.html
stash@{2}: WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (bbeb41b58a3c17bd49b26a257fe39af507e1fb10)

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 4e28d4b Add index.html
stash@{1}: WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (d668b36b09909afa970dca2da1a103948a7eb99b)

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 4e28d4b Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git commit -m "Adding home and about pages"
[dev e8054b7] Adding home and about pages
 2 files changed, 33 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ ls
about.html  home.html  index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is ahead of 'origin/dev' by 2 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (01e83c011fac298e9d2f66b0436f8c8d5daeb8a7)

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git log --oneline
d7fd906 (HEAD -> dev) Adding home and about pages
e8054b7 Adding home and about pages
4e28d4b (origin/dev, origin/Main, Main) Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git reset d7fd906

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git log --oneline
d7fd906 (HEAD -> dev) Adding home and about pages
e8054b7 Adding home and about pages
4e28d4b (origin/dev, origin/Main, Main) Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 2 commits.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 803 bytes | 803.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To github.com:tuyishimehono/GitBundle1.git
   4e28d4b..d7fd906  dev -> dev

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git reset --hard
HEAD is now at d7fd906 Adding home and about pages

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git add -all
error: did you mean `--all` (with two dashes)?

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git add --all

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git push
Everything up-to-date

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

```

## Bundle 2

### Exercise 1

``` bash

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (dev)
$ git checkout -b ft/bundles-2
Switched to a new branch 'ft/bundles-2'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ touch services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ code services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ git add services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ git commit -m "Add services page"
[ft/bundles-2 7305714] Add services page
 2 files changed, 22 insertions(+)
 create mode 100644 services.html
 create mode 100644 team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ git push
fatal: The current branch ft/bundles-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundles-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ git push --set-upstream origin ft/bundles-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 583 bytes | 583.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/bundles-2' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/ft/bundles-2
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      ft/bundles-2 -> ft/bundles-2
branch 'ft/bundles-2' set up to track 'origin/ft/bundles-2'.

```
### Exercise 2

```bash


