* https://resources.coreos.com/youtube-coreos-fest-2017/writing-a-custom-controller-extending-the-functionality-of-your-cluster
* https://github.com/kubernetes/ingress/tree/master/examples/custom-controller
* https://github.com/IanLewis/homepage/tree/master/cron
* https://github.com/aaronlevy/kube-controller-demo
* https://github.com/metral/memhog-operator
* https://docs.google.com/presentation/d/1wEW0qer3M9DtEY4I1xa5JNNZvi6wZ9m7LpTKLErsbuo/edit#slide=id.g1f294243e6_0_159

------------

## Step 1

Figure out the kubernetes/client-go package to use. For working with kubernetes 1.7, I will need atleast client-go 4.0.0-beta.0. So my glide.yaml looks like:
```
import:
- package: k8s.io/client-go
  version: v4.0.0-beta.0
```
References:
- https://github.com/kubernetes/client-go/blob/master/INSTALL.md
- https://github.com/kubernetes/client-go#compatibility-matrix

