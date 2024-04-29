## Install
```
helm install -f values.yaml --set fullnameOverride=t4 t4 ./cipms/
```
## Upgrade
```
helm upgrade t4 ./cipms/ --atomic --cleanup-on-fail --set fullnameOverride=t4,replicaCount=3,repository=tuanldt
```

## Rollback
```
helm rollback t4 1
```

## Uninstall
```
helm uninstall pulsar-replica -n dmp
```