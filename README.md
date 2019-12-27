## Git shortcut commands.

[Branch](branch.md)

### # checkout

Create branch and checkout to it.
```sh
git checkout -b <branch>
```

List branches merged in current branch.
```sh
git branch --merged
```

List branches not merged in current branch.
```sh
git branch --no-merged
```

Remove all merged branches.

```sh
git branch --merged | grep -v $(git rev-parse --abbrev-ref HEAD) | xargs git branch -d
```

Remove all remote merged branches.

**Warning: It can remove remote master or any other critical branch.**
```sh
git branch -r --merged | grep -v master | sed 's/origin\//:/' | xargs -n 1 git push origin
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

Show logs of certain author.
```sh
git log --author=<name>
```

Show only logs of file status.
```sh
git log --name-status
```

### # push

Push new branch and set tracking the branch.
```sh
git push -u <remote> <branch>
```

## Other

Get current branch name you are on.
```sh
git rev-parse --abbrev-ref HEAD
```
