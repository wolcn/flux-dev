### First test environment
One environment, one namespace and one repo

Once a tenant and a sync are configured, push a change and wait a couple of miutes for it to get reconciled

If `yq` is installed:
```
kubectl -n dev get deploy kcheck -oyaml | yq .metadata.generation
```
