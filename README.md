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
