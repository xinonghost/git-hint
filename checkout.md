## Checkout

### Create branch and checkout to it.
This is shortcut for commands `git branch <name>` and `git checkout <name>`.
```sh
git checkout -b <branch>
```
<br />

### Discard all changes.
Forgot all changes which were made for specific file and use state from last commit of HEAD.
```sh
git checkout -- <filename>
```