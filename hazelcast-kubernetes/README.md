# Hazelcast clustering for Kubernetes

It delete username and password of default from source without verification.

If you want to open verification or use more variate please log into the source web



## Quickly start

```bash
kubectl create namespace hazelcast

kubectl create -f  -n hazelcast https://github.com/klzsysy/k8s-images/raw/master/hazelcast-kubernetes/hazelcast-k8s.yaml

```

If the namespace is other,please modify POD_NAMESPACE of variate





## Employ the authority of rabc ， Kubernetes 1.6+

 Need make serveaccount default possess the authority of reading of endpoints of namespace

Create Role And Create RoleBinding

 If the namespace is other,please modify namespace of variate



```bash
kubectl create -f -n hazelcast   https://github.com/klzsysy/k8s-images/raw/master/hazelcast-kubernetes/hazelcast-RBAC.yaml

```

## Sources

- https://github.com/pires/hazelcast-kubernetes-bootstrapper