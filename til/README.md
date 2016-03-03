# Today I Learned

## GIT

### Serving a repo via HTTP

```
$ git clone --bare <original-repo> the_repo
$ cd the_repo
$ git update-server-info
$ # serve /the_repo using any http server
```

### Serving a repo via HTTP

## Docker

### Removing dangling images

```
docker images --quiet --filter=dangling=true | xargs --no-run-if-empty docker rmi
```