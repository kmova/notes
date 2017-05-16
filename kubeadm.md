### Ubuntu based K8s setup using kubeadm 

#### Issues seen with K8s 1.6.2

##### kubeadm init intermittently fails

There is some relationship with the network speed. Have been able to resolve this by downloading the required packages (docker images) prior to issuing the kubeadm init
- https://github.com/kubernetes/kubeadm/issues/226
  (localhost mapping to 10.0.2.3 seems to be causing the issue)

#### machine reboot (minion) - services come up after a long time

#### machine reboot (minion) - weave network goes into crash loop

#### flexvolume under the default directory is not getting registered 

