# k8s-argocd

Repository of all the argocd application manifests

# Installing argoCD

When deploying argoCD, we need to enable `--enable-helm` too.

```yaml
apiVersion: v1
kind: ConfigMap
metadata:
  name: argocd-cm
  namespace: argocd
data:
  kustomize.buildOptions: --enable-helm
```

**Important**
Github repository should be configured beforehand with argocd cli if the repository is not public since authentication will be required.

Order:
- 1password first for secrets

