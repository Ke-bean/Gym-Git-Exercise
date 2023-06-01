#Gym-Git-Exercises

This is the history of all commands used in this exercise bundles.

## Bundle 1

### Exercise 1

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git init
Initialized empty Git repository in C:/Users/Kebean/Documents/Projects/Git Exercise Solutions/.git/
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
No commits yet

nothing to commit (create/copy files and use "git add" to track)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch master
No commits yet

nothing to commit (create/copy files and use "git add" to track)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git branch -M main
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch main

No commits yet

On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add README.md
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch main


Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commint -m "initial commit"

The most similar command is
        commit
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "initial commit"
[main (root-commit) 161d40c] initial commit
 1 file changed, 2 insertions(+)
 create mode 100644 README.md
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git remote add origin https://github.com/Ke-bean/Gym-Git-Exercise.git
error: remote origin already exists.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push --set-upstream origin main
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 285 bytes | 13.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
Switched to a new branch 'dev'
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/dev
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      dev -> dev
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b test
Switched to a new branch 'test'
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/test
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      test -> test
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git branch -D test
Deleted branch test (was 161d40c).
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin --deleted test
error: unknown option `deleted'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --verbose         be more verbose
    -q, --quiet           be more quiet
    --repo <repository>   repository
    --all                 push all refs
    --mirror              mirror all refs
    -d, --delete          delete refs
    --tags                push tags (can't be used with --all or --mirror)
    -n, --dry-run         dry run
    --porcelain           machine-readable output
    -f, --force           force updates
    --force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --force-if-includes   require remote updates to be integrated locally
    --recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --thin                use thin pack
    --receive-pack <receive-pack>
                          receive pack program
    --exec <receive-pack>
                          receive pack program
    -u, --set-upstream    set upstream for git pull/status
    --progress            force progress reporting
    --no-verify           bypass pre-push hook
    --follow-tags         push missing but relevant tags
    --signed[=(yes|no|if-asked)]
                          GPG sign the push
    -o, --push-option <server-specific>
    -4, --ipv4            use IPv4 addresses only

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
Your branch is up to date with 'origin/dev'.
nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push --delete test
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
Everything up-to-date
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout dev
Already on 'dev'
Your branch is up to date with 'origin/dev'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git branch -D test
error: branch 'test' not found.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin --delete test
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 - [deleted]         test
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

### Exercise 2

```bash
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git stash list
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status

  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git stash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git stash list
stash@{0}: WIP on main: 8efd933 updated readme
Saved working directory and index state WIP on main: 8efd933 updated readme
git: 'statsh' is not a git command. See 'git --help'.

The most similar command is
        stash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git stash list
stash@{0}: WIP on main: 8efd933 updated readme
stash@{1}: WIP on main: 8efd933 updated readme
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
Saved working directory and index state WIP on main: 8efd933 updated readme
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git stash pop 1
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
        new file:   about.html
        new file:   home.html

Dropped refs/stash@{1} (d4257932eeda65337d3eea82bd495ef5aa2ef518)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "added home and about page"
[main e341fee] added home and about page
 2 files changed, 24 insertions(+)
 create mode 100644 about.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 549 bytes | 183.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Ke-bean/Gym-Git-Exercise.git
   8efd933..e341fee  main -> main
stash@{0}: WIP on main: 8efd933 updated readme
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (63f3daee6a7b6a4b4bbd8e628df0b642a2f0725a)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git reset --hard
HEAD is now at e341fee added home and about page
```

## Bundle 2

### Exercise 1

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "Added services page"
[ft/bundle-2 bb56cc9] Added services page
 create mode 100644 services.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 477 bytes | 79.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/ft/bundle-2
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
```

### Exercise 2

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "modified service.html"
 1 file changed, 1 insertion(+)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Writing objects: 100% (3/3), 397 bytes | 44.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout main
Switched to branch 'main'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "modified service page"
[main 436747d] modified service page
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
Enumerating objects: 5, done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 396 bytes | 198.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Ke-bean/Gym-Git-Exercise.git
   4148efb..436747d  main -> main
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git diff main
diff --git a/services.html b/services.html
index 66aedfd..630d7ac 100644
--- a/services.html
+++ b/services.html
 <body>
     <p>These are our services</p>
-    <p>This section will include  all new  services that our company offer to our custom and premium clients worldwide</p>
+    <p>This section will include all the services that our company offer to our custom and premium clients worldwide</p>
 </body>
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions>
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/service-redesign
Merge branch 'main' into ft/service-redesign
You have unmerged paths.
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   services.html
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit
[ft/service-redesign eb515ac] Merge branch 'main' into ft/service-redesign
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/service-redesign
Your branch is ahead of 'origin/ft/service-redesign' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 329 bytes | 164.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Ke-bean/Gym-Git-Exercise.git
   4dfd525..eb515ac  ft/service-redesign -> ft/service-redesign
```

## Bundle 3

### Exercise 1

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "added new team page"
[ft/team-page 6e21f28] added new team page
 create mode 100644 team.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 478 bytes | 12.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      ft/team-page -> ft/team-page
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/team-page
Switched to branch 'ft/team-page'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>

    added new team page

commit 6de757abb8e388d236f442325cc25bc4cfdbf641 (origin/main, main, ft/contact-page)
Author: kebean <chenqiua@gmail.com>
Date:   Tue May 30 15:49:07 2023 +0300

    #bundle 2 #Exercise 2
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>
Date:   Tue May 30 15:49:07 2023 +0300

    #bundle 2 #Exercise 2
commit 436747ded1c80b11b9f3ddd27ce47df685320191
Author: kebean <chenqiua@gmail.com>
Date:   Tue May 30 15:22:29 2023 +0300

    modified service page
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git cherry-pick 6e21f284badf728c9042e90a0
[ft/contact-page 13b173a] added new team page
 Date: Thu Jun 1 10:06:27 2023 +0300
 1 file changed, 12 insertions(+)
 create mode 100644 team.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 10:06:27 2023 +0300
    added new team page

commit 6de757abb8e388d236f442325cc25bc4cfdbf641 (origin/main, main)
Author: kebean <chenqiua@gmail.com>
Date:   Tue May 30 15:49:07 2023 +0300

On branch ft/contact-page
nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/contact-page
Untracked files:
        contact.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/contact-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   contact.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "Contact page added"
[ft/contact-page f260f4e] Contact page added
 1 file changed, 12 insertions(+)
 create mode 100644 contact.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push --set-upstream origin ft/contact
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Writing objects: 100% (6/6), 753 bytes | 376.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/ft/contact-page
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
Your branch is up to date with 'origin/ft/contact-page'.

nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "FAQ page added"
[ft/faq-page 685a404] FAQ page added
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push --set-upstream origin ft/faq-pag
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Writing objects: 100% (3/3), 472 bytes | 157.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/ft/faq-page
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>

    FAQ page added

commit f260f4e1a151a7a8e872b40bcee7abda6b82a971 (origin/ft/contact-page, ft/contact-page)
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 10:40:06 2023 +0300

    Contact page added
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/team-page
Switched to branch 'ft/team-page'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
ge)
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 10:06:27 2023 +0300

    added new team page

commit 6de757abb8e388d236f442325cc25bc4cfdbf641 (origin/main, main)
Author: kebean <chenqiua@gmail.com>
Date:   Tue May 30 15:49:07 2023 +0300

    #bundle 2 #Exercise 2
    PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git revert 6e21f284badf728c9042e90a0df5806f355f89c9
[ft/team-page 393dcc4] Revert "added new team page"
 delete mode 100644 team.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout
ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.
[ft/faq-page 1f9ae25] Revert "added new team page"
 1 file changed, 12 deletions(-)
 delete mode 100644 team.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin ft/faq-pafe
error: src refspec ft/faq-pafe does not match any
error: failed to push some refs to 'https://github.com/Ke-bean/Gym-Git-Exercise.git'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin ft/faq-page       in ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 271 bytes | 54.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Ke-bean/Gym-Git-Exercise.git
   685a404..1f9ae25  ft/faq-page -> ft/faq-page
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions>
```

### Exercise 2

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>

    Revert "added new team page"

    This reverts commit 6e21f284badf728c9042e90a0df5806f355f89c9.

commit 685a4045456ebcc17e0c56a0652bdd2e204d25a9
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 10:48:11 2023 +0300
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 11:24:33 2023 +0300

commit e852828f6908b56b975eab192d1a7a0c16423cb4
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 11:19:23 2023 +0300

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/home-page-redesign
nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "new content added"
[ft/home-page-redesign ce5c944] new content added
 1 file changed, 1 insertion(+)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 329 bytes | 164.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/ft/home-page-redesign
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
```

## Bundle 4

### Exercise 1

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git remote add git-copy https://github.com/Ke-bean/Gym-git-clone.git
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git remote
git-copy
origin
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "style file added"
 1 file changed, 1 insertion(+)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Ke-bean/Gym-Git-Exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git pull
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 703 bytes | 4.00 KiB/s, done.
From https://github.com/Ke-bean/Gym-Git-Exercise
   b087116..8c363af  main       -> origin/main
Auto-merging home.html
Merge made by the 'ort' strategy.
 home.html | 1 +
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 635 bytes | 105.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
To https://github.com/Ke-bean/Gym-Git-Exercise.git
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push git-copy
Counting objects: 100% (64/64), done.
Delta compression using up to 4 threads
Compressing objects: 100% (62/62), done.
Writing objects: 100% (64/64), 12.20 KiB | 567.00 KiB/s, done.
Total 64 (delta 32), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (32/32), done.
To https://github.com/Ke-bean/Gym-git-clone.git
 * [new branch]      main -> main
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin
Everything up-to-date
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
```

### Exercise 2

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/footer
Switched to a new branch 'ft/footer'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        footer.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "footer page added"
 create mode 100644 footer.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/footer
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   footer.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add footer.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/footer
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   footer.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "new content added"
[ft/footer 6d4364d] new content added
 1 file changed, 12 insertions(+)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 691 bytes | 1024 bytes/s, done.
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      ft/footer -> ft/footer
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/footer
Switched to branch 'ft/footer'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>

    new content added

commit 261077fba356a8bc8ecd6a05486ef4c60d77ae9f
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 12:20:33 2023 +0300
    footer page added
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git checkout ft/squashing
Switched to branch 'ft/squashing'
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git merge --squash ft/footer
Updating b899f8b..6d4364d
 footer.html | 12 ++++++++++++
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html
On branch ft/squashing
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   footer.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add footer.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "footer changes squashing"
[ft/squashing 9ee740b] footer changes squashing
 1 file changed, 12 insertions(+)
 create mode 100644 footer.html
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git log
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 12:34:45 2023 +0300
    footer changes squashing

commit b899f8bca698b878e08a723d8942242509938002 (origin/main, main)
Author: kebean <chenqiua@gmail.com>
Date:   Thu Jun 1 12:17:02 2023 +0300
    readmefile modified
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch ft/squashing
nothing to commit, working tree clean
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push oring ft/squashing
fatal: 'oring' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push origin  ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 460 bytes | 230.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Ke-bean/Gym-Git-Exercise/pull/new/ft/squashing
remote:
To https://github.com/Ke-bean/Gym-Git-Exercise.git
 * [new branch]      ft/squashing -> ft/squashing
```

## Bundle 5

### Exercise 1

```bash
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git add .
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git status
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    home.html -> index.html

PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git commit -m "renamed home to index"
[main bd252cd] renamed home to index
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)
PS C:\Users\Kebean\Documents\Projects\Git Exercise Solutions> git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 231 bytes | 115.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Ke-bean/Gym-Git-Exercise.git
   4138c25..bd252cd  main -> main
```

### Exercise 2

```bash
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\Kebean\Documents\Projects\git-cafe-exercise> git add index.html
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   index.html

PS C:\Users\Kebean\Documents\Projects\git-cafe-exercise> git commit -m "modified index.html"
[main fb40918] modified index.html
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\Kebean\Documents\Projects\git-cafe-exercise> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 315 bytes | 39.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Ke-bean/git-cafe-exercise.git
   d1d3f9c..fb40918  main -> main
PS C:\Users\Kebean\Documents\Projects\git-cafe-exercise>
```
