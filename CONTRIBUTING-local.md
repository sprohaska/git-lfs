Build in container:

```
docker run -it --rm --name git-lfs-godev \
  -v $(pwd):/go/src/github.com/git-lfs/git-lfs \
  --workdir /go/src/github.com/git-lfs/git-lfs \
  golang:1.10.1

./script/bootstrap -os darwin -arch amd64
```

Run on host:

```
./bin/releases/darwin-amd64/git-lfs-2.4.0/git-lfs
```
