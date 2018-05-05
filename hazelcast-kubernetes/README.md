# Hazelcast clustering for Kubernetes

It delete username and password of default from source without verification.

If you want to open verification or use more variate please log into the source web



## Quickly start

```bash
kubectl create namespace hazelcast

# Employ the authority of RBAC ， Kubernetes 1.6+
# Create Role And Create RoleBinding
kubectl -n hazelcast   create -f  https://github.com/klzsysy/k8s-images/raw/master/hazelcast-kubernetes/hazelcast-RBAC.yaml

# create hazelcast deployment
kubectl  -n hazelcast  create -f https://github.com/klzsysy/k8s-images/raw/master/hazelcast-kubernetes/hazelcast-k8s.yaml

```

## info
Assume KUBERNETES MASTER api is https://kubernetes.default.svc.cluster.local ,The default value, If not, please add a custom variable KUBERNETES_MASTER for k8s api url




## Sources

- https://github.com/pires/hazelcast-kubernetes-bootstrapper