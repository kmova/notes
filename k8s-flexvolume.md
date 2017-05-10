The following error keeps repeating, with the flexvolume driver that was working in k8s 1.5.5

```
May 10 03:36:55 kubeminion-01 kubelet[1234]: I0510 03:36:55.026850    1234 reconciler.go:231] VerifyControllerAttachedVolume operation started for volume "openebs/openebs-iscsi/demo-vsm1-vol1" (spec.Name: "demo-vsm1-vol1") pod "6f157797-352f-11e7-9a8b-021c6f7dbe9d" (UID: "6f157797-352f-11e7-9a8b-021c6f7dbe9d")
May 10 03:36:55 kubeminion-01 kubelet[1234]: E0510 03:36:55.027144    1234 nestedpendingoperations.go:262] Operation for "\"openebs/openebs-iscsi/demo-vsm1-vol1\"" failed. No retries permitted until 2017-05-10 03:36:59.027104161 +0000 UTC (durationBeforeRetry 4s). Error: Volume "openebs/openebs-iscsi/demo-vsm1-vol1" (spec.Name: "demo-vsm1-vol1") pod "6f157797-352f-11e7-9a8b-021c6f7dbe9d" (UID: "6f157797-352f-11e7-9a8b-021c6f7dbe9d") has not yet been added to the list of VolumesInUse in the node's volume status
```

Changes that are causing the error:
- https://github.com/kubernetes/kubernetes/issues/20262



Options Tried to Fix the issue:

(1) Diasable the kubelet flag  ( --enable-controller-attach-detach=false ), this will rollback to the old way of attaching the volumes by the kubelet. 

Add the parameters to the service start configuration:

```
ubuntu@kubeminion-01:~$ sudo cat /etc/systemd/system/kubelet.service.d/10-kubeadm.conf 
[Service]
Environment="KUBELET_KUBECONFIG_ARGS=--kubeconfig=/etc/kubernetes/kubelet.conf --require-kubeconfig=true"
Environment="KUBELET_SYSTEM_PODS_ARGS=--pod-manifest-path=/etc/kubernetes/manifests --allow-privileged=true"
Environment="KUBELET_NETWORK_ARGS=--network-plugin=cni --cni-conf-dir=/etc/cni/net.d --cni-bin-dir=/opt/cni/bin"
Environment="KUBELET_DNS_ARGS=--cluster-dns=10.96.0.10 --cluster-domain=cluster.local"
Environment="KUBELET_AUTHZ_ARGS=--authorization-mode=Webhook --client-ca-file=/etc/kubernetes/pki/ca.crt"
Environment="KUBELET_VOL_ARGS=--enable-controller-attach-detach=false"
ExecStart=
ExecStart=/usr/bin/kubelet $KUBELET_KUBECONFIG_ARGS $KUBELET_SYSTEM_PODS_ARGS $KUBELET_NETWORK_ARGS $KUBELET_DNS_ARGS $KUBELET_AUTHZ_ARGS $KUBELET_VOL_ARGS $KUBELET_EXTRA_ARGS
ubuntu@kubeminion-01:~$ 
```

Restart the kubelet

```
ubuntu@kubeminion-01:~$ sudo systemctl daemon-reload
ubuntu@kubeminion-01:~$ sudo systemctl restart kubelet
```

Verify that --enable-controller-attach-detach=false is set on the kubelet

```
ubuntu@kubeminion-01:~$ ps -auxwww | grep kubelet
root      4238  7.9  6.9 487768 70416 ?        Ssl  17:21   0:00 /usr/bin/kubelet --kubeconfig=/etc/kubernetes/kubelet.conf --require-kubeconfig=true --pod-manifest-path=/etc/kubernetes/manifests --allow-privileged=true --network-plugin=cni --cni-conf-dir=/etc/cni/net.d --cni-bin-dir=/opt/cni/bin --cluster-dns=10.96.0.10 --cluster-domain=cluster.local --authorization-mode=Webhook --client-ca-file=/etc/kubernetes/pki/ca.crt --enable-controller-attach-detach=false

```
