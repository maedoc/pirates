# k8s 

k8s up based on kubeadm, centos & vagrant. 

```bash
tng-imac3:k8s duke$ make
...
tng-imac3:k8s duke$ KUBECONFIG=admin.conf kubectl get nodes
NAME                        STATUS    ROLES     AGE       VERSION
master.cluster.tvb-ins.fr   Ready     master    8m        v1.13.2
node1.cluster.tvb-ins.fr    Ready     <none>    7m        v1.13.2
node2.cluster.tvb-ins.fr    Ready     <none>    7m        v1.13.2
node3.cluster.tvb-ins.fr    Ready     <none>    6m        v1.13.2
node4.cluster.tvb-ins.fr    Ready     <none>    5m        v1.13.2
```

