icon: simple/argo

## Retrieve Argo CD admin Password

```
kubectl -n {namespace} get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
```