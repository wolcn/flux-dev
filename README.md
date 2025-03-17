### First test environment
One environment, one namespace and one repo

If `yq` is installed:
```
kubectl -n dev get deploy kcheck -oyaml | yq .metadata.generation
```
