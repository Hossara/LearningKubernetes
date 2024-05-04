# Kubernetes namespaces

### Namespaces file
You apply and import your namespaces by creating namespace config file:
```yaml
---
apiVersion: v1
kind: Namespace
metadata:
  name: development
---
apiVersion: v1
kind: Namespace
metadata:
  name: production

```

Now you can import, change and delete your namespaces using this file:

#### Import, update
```bash
kubectl -- apply -f namespace.yaml
```


#### Delete
```bash
kubectl -- delete -f namespace.yaml
```

To see your namespaces:
```bash
kubectl -- get namespaces
```

