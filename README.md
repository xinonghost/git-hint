## Git shortcut commands.

[Add](add.md)<br />
[Branch](branch.md)<br />
[Checkout](checkout.md)<br />
[Config](config.md)<br />
[Diff](diff.md)<br />
[Rev-Parse](rev-parse.md)

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
