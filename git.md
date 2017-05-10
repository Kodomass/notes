# git commands

Show last commit's `diff`

```git
git show
```
it is an alias for `git diff @~..@`.

Set and remove remote upstream link
```git
git branch --set-upstream-to origin/some_remote

git branch --unset-upstream
```

Checkout previous branch
```git
git checkout -
```
which is an alias of `git checkout @{-1}`.
