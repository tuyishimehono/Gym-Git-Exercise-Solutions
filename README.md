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

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/bundles-2)
$ git checkout main
Switched to branch 'main'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 916 bytes | 229.00 KiB/s, done.
From github.com:tuyishimehono/GitBundle1
   4e28d4b..3baa726  Main       -> origin/Main
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git add services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git commit -m "Updating services"
[ft/service-redesign 787d4dc] Updating services
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 470 bytes | 235.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/ft/service-redesign
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git add services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git commit -m "Updating services again"
[main 13423a6] Updating services again
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git push --set-upstream origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 478 bytes | 478.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'main' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/main
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git diff main ft/service-redesign
diff --git a/services.html b/services.html
index 615bc76..8cbcac4 100644
--- a/services.html
+++ b/services.html
@@ -7,6 +7,6 @@
 </head>
 <body>
     <h1>These are Services</h1>
-    <p>Another new service</p>
+    <p>A new service</p>
 </body>
 </html>
\ No newline at end of file

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git add services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git push
Everything up-to-date

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git add services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git push
Everything up-to-date

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git add services.html


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git push
Everything up-to-date

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git checkout ft/service-redesign
Already on 'ft/service-redesign'
M       services.html
Your branch is up to date with 'origin/ft/service-redesign'.


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git merge main
error: Your local changes to the following files would be overwritten by merge:
  services.html
Merge with strategy ort failed.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git add services.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git commit -m "modified services"
[ft/service-redesign c5a69a2] modified services
 1 file changed, 1 deletion(-)

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 325 bytes | 325.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:tuyishimehono/GitBundle1.git
   787d4dc..c5a69a2  ft/service-redesign -> ft/service-redesign

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git add services.html


Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign|MERGING)
$ git commit -m "modified services"
[ft/service-redesign 6f0cd0f] modified services

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git merge main
Already up to date.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git push
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 218 bytes | 109.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:tuyishimehono/GitBundle1.git
   c5a69a2..6f0cd0f  ft/service-redesign -> ft/service-redesign

```

## Bundle 3

### Exercise 1

``` bash

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ touch team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ code team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ git add team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ git commit -m "Adding team page"
[ft/team-page 0f3a3f9] Adding team page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 486 bytes | 486.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/ft/team-page
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ git log
commit 0f3a3f9f489493bdbf536eff5ce5c4034fd8f4dd (HEAD -> ft/team-page, origin/ft/team-page)
Author: tuyishimehono <tuhonori1@gmail.com>
Date:   Mon Apr 22 16:20:04 2024 +0200

    Adding team page

commit 13423a6a05d82af1e9aa96c5534032add16f8c8d (origin/main, main, ft/contact-page)
Author: tuyishimehono <tuhonori1@gmail.com>
Date:   Mon Apr 22 15:27:56 2024 +0200

    Updating services again

commit 4e28d4b660efefe7f35d2dc3bc3f7a75b9e4a223
Author: tuyishimehono <tuhonori1@gmail.com>
Date:   Mon Apr 22 12:07:22 2024 +0200

    Add index.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/contact-page)
$ git cherry-pick 0f3a3f9f489493bdbf536eff5ce5c4034fd8f4dd
[ft/contact-page 8716111] Adding team page
 Date: Mon Apr 22 16:20:04 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/contact-page)
$ git add contact.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/contact-page)
$ git commit -m "Adding Contact page"
[ft/contact-page b16d056] Adding Contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 755 bytes | 755.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/ft/contact-page
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git add faq.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git commit -m "Adding a FAQ page"
[ft/faq-page e4df0b7] Adding a FAQ page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 463 bytes | 463.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/tuyishimehono/GitBundle1/pull/new/ft/faq-page
remote:
To github.com:tuyishimehono/GitBundle1.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git revert 0f3a3f9f489493bdbf536eff5ce5c4034fd8f4dd
[ft/faq-page b3f2087] Revert "Adding team page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git add .

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Honorine@Tuyishime-PC MINGW64 ~/gitBundle1 (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 275 bytes | 275.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:tuyishimehono/GitBundle1.git
   e4df0b7..b3f2087  ft/faq-page -> ft/faq-page

```

### Exercise 2

```bash

