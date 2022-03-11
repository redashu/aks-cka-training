# aks-cka-training

## POd Designing 

<img src="pod1.png">

### creating pod and checking 

```
 ls
ashupod1.yaml
fire@ashutoshhs-MacBook-Air k8syamls % kubectl  apply -f ashupod1.yaml --dry-run=client 
pod/ashupod-1234 created (dry run)
fire@ashutoshhs-MacBook-Air k8syamls % 
```

### sending request to apiserver for pod deployment 

```
 kubectl  apply -f ashupod1.yaml 
pod/ashupod-1234 created
fire@ashutoshhs-MacBook-Air k8syamls % kubectl get  pods               
NAME           READY   STATUS    RESTARTS   AGE
ajeetpod       1/1     Running   0          17s
ashupod-1234   1/1     Running   0          2s
fire@ashutoshhs-MacBook-Air k8syamls % 
```

