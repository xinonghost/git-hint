## Branch

### Set tracking branch.
Branch tracking add extra info to current branch status and shows difference between current branch and remote one which current branch is tracking.
```sh
git branch -u <remote>/<branch>
```
<br />

### Unset tracking branch.
Remove tracking branch from current branch.
```sh
git branch --unset-upstream
```
<br />

### List branches merged in current branch.
Show list of branches which are already fully merged into current branch.
```sh
git branch --merged
```
<br />

### List branches not merged in current branch.
Show list of all branches which aren't fully merged into current branch.
```sh
git branch --no-merged
```
<br />

### Remove all merged branches.
Remove all local branches which already are fully merged into current branch. Useful for cleaning up the old useless branches. Could be aliased for convenience.
```sh
git branch --merged | grep -v $(git rev-parse --abbrev-ref HEAD) | xargs git branch -d
```
<br />

### Remove all remote merged branches.
Remove all remote merged branches which are fully merged to local current branch.<br/>
**Warning: It can remove remote master or any other critical branch.**
```sh
git branch -r --merged | grep -v master | sed 's/origin\//:/' | xargs -n 1 git push origin
```
