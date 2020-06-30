# One time setup
```
go mod init
go get sigs.k8s.io/kustomize/kyaml
```

# Build the binary
```
go build .
```

# test the binary
```
kpt fn source config/ | kpt fn run --enable-exec --exec-path ./set-namespace -- namespace=test-ns
```
