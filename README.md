## Git shortcut commands.

### # branch

Set tracking branch.
```sh
git branch -u <remote>/<branch>
```

Unset tracking branch.
```sh
git branch --unset-upstream
```

### # checkout

Create branch and checkout to it.
```sh
git checkout -b <branch>
```

### # commit

Add all tracked files and make new commit.
```sh
git commit -am "<message>"
```

Change last commit message.
```sh
git commit --amend -m "<message>"
```

Add change to last commit without changing commit message.
```sh
git commit -a --amend --no-edit
```

### # log

Prettify log output.

```sh
git log --graph --pretty=format:'%Cred%h%Creset %Cgreen(%an)%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%Creset' --abbrev-commit --date=relative
```

### # push

Push new branch and set tracking the branch.
```sh
git push -u <remote> <branch>
