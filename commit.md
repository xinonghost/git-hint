## Commit

### Add all tracked files and make new commit.
Make new commit including all changes to all tracked files in working directory. It's shortcut for `git add -u && git commit -m <message>`.
```sh
git commit -am "<message>"
```
<br />

### Change last commit message.
Change message of last commit.
```sh
git commit --amend -m "<message>"
```
<br />

### Append changes to last commit.
Append changes to last commit without changing commit message.
```sh
git commit -a --amend --no-edit
```
