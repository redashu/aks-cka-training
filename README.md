# aks-cka-training

## Creating and setup Namespace 

```
 20  kubectl create  ns  ashu-project 
   21  kubectl config  set-context --current --namespace=ashu-project 
   22  kubectl  config get-contexts  
```

### testing one more Ingress rule 

```
kubectl run  ashupod1  --image=dockerashu/cka:v1 --port 80 
pod/ashupod1 created
[root@control-plane ~]# kubectl get po
NAME       READY   STATUS    RESTARTS   AGE
ashupod1   1/1     Running   0          4s
[root@control-plane ~]# 
[root@control-plane ~]# kubectl expose pod  ashupod1  --port 80 --name ashulb1 
service/ashulb1 exposed
[root@control-plane ~]# kubectl get  svc 
NAME      TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)   AGE
ashulb1   ClusterIP   10.108.101.23   <none>        80/TCP    6s
[root@control-plane ~]# 


```

