## Log

### Show short log.
Show short and aggregated log.
```sh
git shortlog
```
<br />

### Prettify log output.
Show log in pretty way with colors and additional commit info.
```sh
git log --graph --pretty=format:'%Cred%h%Creset %Cgreen(%an)%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%Creset' --abbrev-commit --date=relative
```
<br />

### Show logs of certain author.
Show logs of certain author by it's name.
```sh
git log --author=<name>
```
<br />

### Show only logs of file status.
Show logs of files changes, what files was involved in commit and what type of changes were made.
```sh
git log --name-status
```
