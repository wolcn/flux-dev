### First test environment
One environment, one namespace and one repo

Once a tenant and a sync are configured, push a change and wait a couple of minutes for it to get reconciled

If `yq` is installed, a useful way to check for updates is:
```
kubectl -n dev get deploy kcheck -oyaml | yq .metadata.generation
```
