# git commands

Show differences:
-----------------

Show last commit's `diff`:

```git
git show
```
it is an alias for `git diff @~..@`.

Show diff for a praticular commit hash:
```git
git diff COMMIT^ COMMIT
```

Show all branches that contain commits from `branch-to-delete`:
```git
git branch --contains branch-to-delete
```

Show commits that are in `old-branch` but not in `new-branch`:
```git
git log new-branch..old-branch
```

Show `diff` by these commits (note 3 dots!):
```
git diff new-branch...old-branch
```

Show all branches which can be safely deleted, since those branches are
fully contatined in HEAD
```git
git branch --merged
```


Work with branches:
-------------------

Set and remove remote upstream link:
```git
git branch --set-upstream-to origin/some_remote_branch

git branch --unset-upstream
```

Checkout previous branch:
```git
git checkout -
```
which is an alias of `git checkout @{-1}`.


Clean branches:
---------------

Show all local branches and all local references to remote branches:
```git
git branch -a
```

Show all local references to remote branches:
```git
git branch -r
```

Show all the branches on the remote, including those that are not
tracked locally and even those that have not yet been fetched.
```git
git remote show origin
```

Show remote branches:
```git
git ls-remote --heads origin
```

Clean local references to remote branch
```git
git remote prune origin --dry-run

git remote prune origin
```
