# aks-cka-training

## Networking 

<img src="net.png">

## TO access application running in the pod 

### case 1 : when we are k8s client 

```
kubectl port-forward  ashupod1  1234:80 
Forwarding from 127.0.0.1:1234 -> 80
Forwarding from [::1]:1234 -> 80

```

### case2 : when we are not k8s client (we are end users)

<img src="network.png">

### container network Interface (CNI)

<img src="cni.png">

### CNI more details 

<img src="cni1.png">

### NEtwork bridge by CNI -- for pod networking 

<img src="podbridge.png">


