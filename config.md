## Config

### Set oneline log.
Set oneline log on permanent basis.
```sh
git config format.pretty oneline
```
<br />

### Cache credentials.
Cache access credentials for specific time.
```sh
git config credential.helper 'cache --timeout=<seconds>'
```
<br />

### Forgot credentials.
Remove credentials cache and forgot access credentials.
```sh
git credential-cache exit
```
