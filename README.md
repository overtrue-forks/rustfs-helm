# rustfs-helm

You can use this helm chart to deploy rustfs on k8s cluster.

## Requirement

* Helm V3
* RustFS >= 1.0.0-alpha.56

## Installation

Running the command:

```
helm install rustfs -n rustfs --create-namespace ./
```

Check the pod status

```
kubectl -n rustfs get pods -w
NAME       READY   STATUS    RESTARTS        AGE
rustfs-0   1/1     Running   0               2m27s
rustfs-1   1/1     Running   0               2m27s
rustfs-2   1/1     Running   0               2m27s
rustfs-3   1/1     Running   0               2m27s
```

## Uninstall

Uninstalling the rustfs installation with command,

```
helm uninstall rustfs -n rustfs
```
